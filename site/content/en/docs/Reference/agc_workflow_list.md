---
date: 2024-09-19T19:40:28-04:00
title: "agc workflow list"
slug: agc_workflow_list
---
## agc workflow list

Show a list of workflows related to the current project

### Synopsis

list is for showing a combined list of workflows defined in the project specification
and workflow instances that were run in this AWS account.

Output of the command has following format:
WORKFLOWNAME: Name


```
agc workflow list [flags]
```

### Options

```
  -h, --help   help for list
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

