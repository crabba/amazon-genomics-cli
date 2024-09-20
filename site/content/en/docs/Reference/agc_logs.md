---
date: 2024-09-19T19:40:28-04:00
title: "agc logs"
slug: agc_logs
---
## agc logs

Commands for various logs.

### Synopsis

Commands for various logs.
Logs can currently be listed for workflows, workflow engines, 
and various AGC infrastructure parts.
You can also show the content of any CloudWatch log stream that you have
access rights to.

### Options

```
  -p, --awsProfile string   Use the provided AWS CLI profile.
  -h, --help                help for logs
```

### Options inherited from parent commands

```
      --format string   Format option for output. Valid options are: text, table, json
      --silent          Suppresses all diagnostic information.
  -v, --verbose         Display verbose diagnostic information.
```

### SEE ALSO

* [agc]({{< relref "agc" >}})	 - 🧬 Launch and manage genomics workloads on AWS.
* [agc logs access]({{< relref "agc_logs_access" >}})	 - Show workflow access logs for a given context.
* [agc logs adapter]({{< relref "agc_logs_adapter" >}})	 - Show workflow adapter logs for a given context.
* [agc logs engine]({{< relref "agc_logs_engine" >}})	 - Show workflow engine logs for a given context.
* [agc logs workflow]({{< relref "agc_logs_workflow" >}})	 - Show the task logs of a given workflow

