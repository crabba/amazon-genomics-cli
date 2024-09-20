---
date: 2024-09-19T19:40:28-04:00
title: "agc workflow run"
slug: agc_workflow_run
---
## agc workflow run

Run a workflow

### Synopsis

run is for running the specified workflow in the specified context.
This command prints a run Id for the created workflow instance.


```
agc workflow run workflow_name --context context_name [flags]
```

### Examples

```

Run the workflow named "myworkflow", against the "prod" context,
using input parameters contained in file "/home/ec2-user/myproj/workflows/myworkflow/myworkflow.inputs.json"
/code $ agc workflow run myworkflow --context prod --inputsFile workflows/myworkflow/myworkflow.inputs.json
```

### Options

```
  -c, --context string       Name of context
  -h, --help                 help for run
  -i, --inputsFile string    Inputs File Path
  -o, --optionsFile string   Options file to use.
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

