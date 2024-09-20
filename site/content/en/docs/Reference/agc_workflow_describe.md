---
date: 2024-09-19T19:40:28-04:00
title: "agc workflow describe"
slug: agc_workflow_describe
---
## agc workflow describe

Show the information for a specific workflow in the current project

### Synopsis

describe is for showing details on the specified workflow.
It includes workflow specification and list of recent instances of that workflow.
An instance is created every time we run a workflow.

Output of the command has following format:
WORKFLOW: Name Source TypeLanguage TypeVersion


```
agc workflow describe workflow_name [--max_instances] [flags]
```

### Options

```
  -h, --help   help for describe
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

