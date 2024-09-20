---
date: 2024-09-19T19:40:28-04:00
title: "agc completion zsh"
slug: agc_completion_zsh
---
## agc completion zsh

generate the autocompletion script for zsh

### Synopsis


Generate the autocompletion script for the zsh shell.

If shell completion is not already enabled in your environment you will need
to enable it.  You can execute the following once:

$ echo "autoload -U compinit; compinit" >> ~/.zshrc

To load completions for every new session, execute once:
# Linux:
$ agc completion zsh > "${fpath[1]}/_agc"
# macOS:
$ agc completion zsh > /usr/local/share/zsh/site-functions/_agc

You will need to start a new shell for this setup to take effect.


```
agc completion zsh [flags]
```

### Options

```
  -h, --help              help for zsh
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

