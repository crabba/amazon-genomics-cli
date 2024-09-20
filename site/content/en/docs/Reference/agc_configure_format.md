---
date: 2024-09-19T19:40:28-04:00
title: "agc configure format"
slug: agc_configure_format
---
## agc configure format

Sets default format option for output display of AGC commands. Valid format options are 'text', 'table', or 'json'

```
agc configure format output_format [flags]
```

### Options

```
  -h, --help   help for format
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

