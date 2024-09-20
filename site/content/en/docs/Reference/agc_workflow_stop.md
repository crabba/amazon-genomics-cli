---
date: 2024-09-19T19:40:28-04:00
title: "agc workflow stop"
slug: agc_workflow_stop
---
## agc workflow stop

Stop the workflow with the specified workflow instance id.

### Synopsis


Stop the workflow with the specified workflow instance id. Signals to the workflow engine that all running tasks of the
workflow instance should be stopped and any pending tasks should be cancelled.

```
agc workflow stop workflow_instance_id [flags]
```

### Examples

```

agc workflow stop ae12347654329
```

### Options

```
  -h, --help   help for stop
```

### Options inherited from parent commands

```
  -p, --awsProfile string   Use the provided AWS CLI profile.
      --format string       Format option for output. Valid options are: text, table, json
      --silent              Suppresses all diagnostic information.
  -v, --verbose             Display verbose diagnostic information.
```

### SEE ALSO

* [agc workflow]({{< relref "agc_workflow" >}})	 - Commands for workflows.
Workflows are potentially-dynamic graphs of computational tasks to execute.

