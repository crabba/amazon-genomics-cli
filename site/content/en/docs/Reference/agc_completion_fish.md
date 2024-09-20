---
date: 2024-09-19T19:40:28-04:00
title: "agc completion fish"
slug: agc_completion_fish
---
## agc completion fish

generate the autocompletion script for fish

### Synopsis


Generate the autocompletion script for the fish shell.

To load completions in your current shell session:
$ agc completion fish | source

To load completions for every new session, execute once:
$ agc completion fish > ~/.config/fish/completions/agc.fish

You will need to start a new shell for this setup to take effect.


```
agc completion fish [flags]
```

### Options

```
  -h, --help              help for fish
      --no-descriptions   disable completion descriptions
```

### Options inherited from parent commands

```
      --format string   Format option for output. Valid options are: text, table, json
      --silent          Suppresses all diagnostic information.
  -v, --verbose         Display verbose diagnostic information.
```

### SEE ALSO

* [agc completion]({{< relref "agc_completion" >}})	 - generate the autocompletion script for the specified shell

