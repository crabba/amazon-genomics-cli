---
date: 2024-09-19T19:40:28-04:00
title: "agc logs workflow"
slug: agc_logs_workflow
---
## agc logs workflow

Show the task logs of a given workflow

### Synopsis

Show the task logs of a given workflow.
If the --run flag is omitted then the latest workflow run is used.

```
agc logs workflow workflow_name [-r run_id] [--failed_tasks] [flags]
```

### Options

```
      --all-tasks          Show logs of all tasks in the given workflow run
  -e, --end string         A date to stop displaying logs.
                           Supports most date formats, such as mm/dd/yy or yyyy-mm-dd-07:00.
                           Times respect the system timezone.
      --failed-tasks       Only show logs of tasks that have not exited cleanly.
  -f, --filter string      Match terms, phrases, or values in the logs.
                           Filters are case sensitive and multiple terms combine with AND logic.
                           Use a question mark for OR, such as "?ERROR ?WARN". Filter out terms with a minus, such as "-INFO".
  -h, --help               help for workflow
  -l, --look-back string   A period of time to look back from now, such as "2h45m".
                           Valid time units are "s", "m", and "h".
  -r, --run string         The ID of a workflow run to retrieve.
  -s, --start string       A date to begin displaying logs.
                           Supports most date formats, such as 2021/03/31 or 8/8/2021 01:00:01 PM.
                           Times respect the system timezone.
  -t, --tail               Follow the log output.
      --task string        The ID of a single task to retrieve.
```

### Options inherited from parent commands

```
  -p, --awsProfile string   Use the provided AWS CLI profile.
      --format string       Format option for output. Valid options are: text, table, json
      --silent              Suppresses all diagnostic information.
  -v, --verbose             Display verbose diagnostic information.
```

### SEE ALSO

* [agc logs]({{< relref "agc_logs" >}})	 - Commands for various logs.

