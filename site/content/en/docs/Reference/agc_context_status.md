---
date: 2024-09-19T19:40:28-04:00
title: "agc context status"
slug: agc_context_status
---
## agc context status

Show the status for the deployed contexts in the project

### Synopsis

status is for showing the status for the deployed contexts in the project. 

Output of the command has following format:
INSTANCE: ContextName ContextReason ContextStatus IsDefinedInProjectFile


```
agc context status [flags]
```

### Examples

```

/code agc context status
```

### Options

```
  -h, --help   help for status
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

