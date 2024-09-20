---
date: 2024-09-19T19:40:28-04:00
title: "agc workflow status"
slug: agc_workflow_status
---
## agc workflow status

Show the status for workflow run(s) in the current project.

```
agc workflow status [flags]
```

### Options

```
  -c, --context-name string    show status of workflow runs in a specific context
  -h, --help                   help for status
      --limit int              maximum number of workflow instances to show (default 20)
  -r, --run-id string          show status of specific workflow run
  -n, --workflow-name string   show status of workflow runs for a specific workflow name
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

