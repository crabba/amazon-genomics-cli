---
date: 2024-09-19T19:40:28-04:00
title: "agc context describe"
slug: agc_context_describe
---
## agc context describe

Show the information for a specific context in the current project

### Synopsis

describe is for showing information about the specified context.

Output of the command has following format:
CONTEXT: MaxVCpus Name RequestSpotInstances Status StatusReason
INSTANCETYPE: Value
OUTPUTLOCATION: Url
WESENDPOINT: Url


```
agc context describe context_name [flags]
```

### Examples

```

/code agc context describe myCtx
```

### Options

```
  -c, --context string   Names of one or more contexts to deploy
  -h, --help             help for describe
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

