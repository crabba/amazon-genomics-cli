---
date: 2024-09-19T19:40:28-04:00
title: "agc configure"
slug: agc_configure
---
## agc configure

Commands for configuration.
Configuration is stored per user.

### Synopsis

Commands for configuration.
Configure local settings and preferences to customize the CLI experience.

### Options

```
  -p, --awsProfile string   Use the provided AWS CLI profile.
  -h, --help                help for configure
```

### Options inherited from parent commands

```
      --format string   Format option for output. Valid options are: text, table, json
      --silent          Suppresses all diagnostic information.
  -v, --verbose         Display verbose diagnostic information.
```

### SEE ALSO

* [agc]({{< relref "agc" >}})	 - 🧬 Launch and manage genomics workloads on AWS.
* [agc configure describe]({{< relref "agc_configure_describe" >}})	 - Shows current configuration of the AGC setup for current user
* [agc configure email]({{< relref "agc_configure_email" >}})	 - Sets user email address to be used to tag AGC resources created in the account
* [agc configure format]({{< relref "agc_configure_format" >}})	 - Sets default format option for output display of AGC commands. Valid format options are 'text', 'table', or 'json'

