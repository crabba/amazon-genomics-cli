---
date: 2024-09-19T19:40:28-04:00
title: "agc configure describe"
slug: agc_configure_describe
---
## agc configure describe

Shows current configuration of the AGC setup for current user

### Synopsis

Running this command reads current configuration file for AGC and prints out it content
Output of the command has following format:
CONFIG:
FORMAT: Name
USER: Email Id


```
agc configure describe [flags]
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

* [agc configure]({{< relref "agc_configure" >}})	 - Commands for configuration.
Configuration is stored per user.

