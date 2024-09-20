---
date: 2024-09-19T19:40:28-04:00
title: "agc context list"
slug: agc_context_list
---
## agc context list

List contexts in the project

### Synopsis

list is for showing a combined list of contexts specified in
the project specification.

Output of the command has following format:
CONTEXTSUMMARY: EngineName Name


```
agc context list [flags]
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

* [agc context]({{< relref "agc_context" >}})	 - Commands for contexts.
Contexts specify workflow engines and computational fleets to use when running a workflow.

