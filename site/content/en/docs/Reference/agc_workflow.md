---
date: 2024-09-19T19:40:28-04:00
title: "agc workflow"
slug: agc_workflow
---
## agc workflow

Commands for workflows.
Workflows are potentially-dynamic graphs of computational tasks to execute.

### Synopsis

Commands for workflows.
Workflows are potentially-dynamic graphs of computational tasks to execute.

Workflow specifications are files whose content specify a workflow to execute 
given a particular set of input parameters to use. Workflow specifications are 
typed according to which workflow definition language they use (e.g. WDL).


### Options

```
  -p, --awsProfile string   Use the provided AWS CLI profile.
  -h, --help                help for workflow
```

### Options inherited from parent commands

```
      --format string   Format option for output. Valid options are: text, table, json
      --silent          Suppresses all diagnostic information.
  -v, --verbose         Display verbose diagnostic information.
```

### SEE ALSO

* [agc]({{< relref "agc" >}})	 - 🧬 Launch and manage genomics workloads on AWS.
* [agc workflow describe]({{< relref "agc_workflow_describe" >}})	 - Show the information for a specific workflow in the current project
* [agc workflow list]({{< relref "agc_workflow_list" >}})	 - Show a list of workflows related to the current project
* [agc workflow output]({{< relref "agc_workflow_output" >}})	 - Show the output for a workflow run in the current project.
* [agc workflow run]({{< relref "agc_workflow_run" >}})	 - Run a workflow
* [agc workflow status]({{< relref "agc_workflow_status" >}})	 - Show the status for workflow run(s) in the current project.
* [agc workflow stop]({{< relref "agc_workflow_stop" >}})	 - Stop the workflow with the specified workflow instance id.

