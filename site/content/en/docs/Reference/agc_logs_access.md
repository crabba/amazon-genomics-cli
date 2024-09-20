---
date: 2024-09-19T19:40:28-04:00
title: "agc logs access"
slug: agc_logs_access
---
## agc logs access

Show workflow access logs for a given context.

### Synopsis

Show workflow access logs for a given context.
If no start, end, or look back periods are set, this command will show logs from the last hour.

```
agc logs access -c context_name [-f filter] [-s start_date] [-e end_date] [-l look_back] [-t] [flags]
```

### Examples

```

/code agc logs access -c myCtx -s 2021/3/31 -e 2021/4/1 -f ERROR
```

### Options

```
  -c, --context string     Name of context
  -e, --end string         A date to stop displaying logs.
                           Supports most date formats, such as mm/dd/yy or yyyy-mm-dd-07:00.
                           Times respect the system timezone.
  -f, --filter string      Match terms, phrases, or values in the logs.
                           Filters are case sensitive and multiple terms combine with AND logic.
                           Use a question mark for OR, such as "?ERROR ?WARN". Filter out terms with a minus, such as "-INFO".
  -h, --help               help for access
  -l, --look-back string   A period of time to look back from now, such as "2h45m".
                           Valid time units are "s", "m", and "h".
  -s, --start string       A date to begin displaying logs.
                           Supports most date formats, such as 2021/03/31 or 8/8/2021 01:00:01 PM.
                           Times respect the system timezone.
  -t, --tail               Follow the log output.
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

