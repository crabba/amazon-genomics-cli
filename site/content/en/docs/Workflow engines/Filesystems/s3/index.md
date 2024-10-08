---
title: "S3 Workflow Filesystem"
date: 2022-03-11T14:37:50-05:00
draft: false
---

## Amazon S3 Workflow Filesystem

Some workflow engines deployed by Amazon Genomics CLI can use S3 as their shared "filesystem". Because S3 is not a POSIX
compliant filesystem and most of the applications run by workflow tasks will require POSIX files, inputs will be localized
from Amazon S3 and outputs will be delocalized to Amazon S3.

### Advantages

1. Inputs are read into each task's container and are not available by a common container mount so there is no possibility of containers on the same host over-writing or accessing another tasks inputs
2. No shared file system needs to be provisioned for a contexts compute environment thereby reducing ongoing costs.
3. All intermediate task outputs and all workflow outputs are persisted to the S3 bucket provisioned by Amazon Genomics CLI and this bucket will remain after contexts are destroyed and even after Amazon Genomics CLI is deactivated in the account.
4. Container hosts use an auto-expansion strategy for their local EBS volumes so disk sizes don't need to be stated.

### Disadvantages

1. Container hosts running multiple tasks may exhaust their aggregate network bandwidth (see below).
2. It is assumed that no other external process will be making changes to the S3 objects during a workflow run. If this does happen, the run may fail or be corrupted.

### Network Bandwidth Considerations

During workflows with large numbers of concurrent steps that all rely on large inputs you may observe that the localization
of inputs to the containers will become very slow. This is because a single EC2 container host may have multiple containers
all competing for limited bandwidth. In these cases we recommend the following possible mitigations:

1. Consider using a shared filesystem such as EFS for your engine or an engine that supports EFS
2. Configure your `agc-project.yaml` such that a context is available that uses instance types that are [network optimized](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/general-purpose-instances.html#general-purpose-network-performance). 
For example used `m5n` instance types rather than `m5` and use instance types that offer sustained throughput rather than 
[bursting throughput](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/general-purpose-instances.html#general-purpose-network-performance) such as instances with more than 16 vCPU.
3. Consider modifying your workflow to request larger memory and vCPU amounts for these tasks. This will tend to ensure 
AWS Batch selects larger instances with better performance as well as placing fewer containers per host resulting in less competition for bandwidth.

These mitigations may result in the use of more expensive infrastructure but can ultimately save money by completing
the workflow quicker. The best price-performance configuration will vary by workflow.

### Supporting Engines

The [Cromwell]( {{< relref "../../cromwell/index.md" >}} ) and [Nextflow]( {{< relref "../../nextflow/index.md" >}} ) engines both support the use of Amazon S3 as a filesystem.
Contexts using these engines will use this filesystem by default.