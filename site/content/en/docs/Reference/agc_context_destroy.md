---
date: 2024-09-19T19:40:28-04:00
title: "agc context destroy"
slug: agc_context_destroy
---
## agc context destroy

Destroy contexts in the current project.

### Synopsis

destroy is for destroying one or more contexts. 
It destroys AGC resources in AWS.

```
agc context destroy {context_name ... | --all} [flags]
```

### Examples

```

/code agc context destroy context1 context2
```

### Options

```
      --all               Destroy all contexts in the project
  -c, --context strings   Names of one or more contexts to destroy
      --force             Destroy context and stop running workflows within context
  -h, --help              help for destroy
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

