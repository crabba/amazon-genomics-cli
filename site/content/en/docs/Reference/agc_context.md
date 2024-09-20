---
date: 2024-09-19T19:40:28-04:00
title: "agc context"
slug: agc_context
---
## agc context

Commands for contexts.
Contexts specify workflow engines and computational fleets to use when running a workflow.

### Synopsis

Commands for contexts.
Contexts specify workflow engines and computational fleets to use when running a workflow.
Users can quickly switch between infrastructure configurations by specifying a 
particular context.

### Options

```
  -p, --awsProfile string   Use the provided AWS CLI profile.
  -h, --help                help for context
```

### Options inherited from parent commands

```
      --format string   Format option for output. Valid options are: text, table, json
      --silent          Suppresses all diagnostic information.
  -v, --verbose         Display verbose diagnostic information.
```

### SEE ALSO

* [agc]({{< relref "agc" >}})	 - 🧬 Launch and manage genomics workloads on AWS.
* [agc context deploy]({{< relref "agc_context_deploy" >}})	 - Deploy contexts in the current project
* [agc context describe]({{< relref "agc_context_describe" >}})	 - Show the information for a specific context in the current project
* [agc context destroy]({{< relref "agc_context_destroy" >}})	 - Destroy contexts in the current project.
* [agc context list]({{< relref "agc_context_list" >}})	 - List contexts in the project
* [agc context status]({{< relref "agc_context_status" >}})	 - Show the status for the deployed contexts in the project

