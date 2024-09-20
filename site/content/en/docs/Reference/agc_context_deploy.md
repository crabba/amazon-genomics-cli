---
date: 2024-09-19T19:40:28-04:00
title: "agc context deploy"
slug: agc_context_deploy
---
## agc context deploy

Deploy contexts in the current project

### Synopsis

deploy is for deploying one or more contexts. 
It creates AGC resources in AWS.

Output of the command has following format:
DETAIL: AccessLogGroupName BucketLocation EngineLogGroupName Status StatusReason WesLogGroupName WesUrl
SUMMARY: IsSpot MaxVCpus Name
ENGINE: Engine Type
FILESYSTEM: FSType
FSCONFIG: FSProvisionedThroughput
STRING


```
agc context deploy {context_name ... | --all} [flags]
```

### Examples

```

/code agc context deploy context1 context2
```

### Options

```
      --all               Deploy all contexts in the project
  -c, --context strings   Names of one or more contexts to deploy
  -h, --help              help for deploy
```

### Options inherited from parent commands

```
  -p, --awsProfile string   Use the provided AWS CLI profile.
      --format string       Format option for output. Valid options are: text, table, json
      --silent              Suppresses all diagnostic information.
  -v, --verbose             Display verbose diagnostic information.
```

### SEE ALSO

* [agc context]({{< relref "agc_context" >}})	 - Commands for contexts.
Contexts specify workflow engines and computational fleets to use when running a workflow.

