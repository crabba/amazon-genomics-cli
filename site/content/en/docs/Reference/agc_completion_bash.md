---
date: 2024-09-19T19:40:28-04:00
title: "agc completion bash"
slug: agc_completion_bash
---
## agc completion bash

generate the autocompletion script for bash

### Synopsis


Generate the autocompletion script for the bash shell.

This script depends on the 'bash-completion' package.
If it is not installed already, you can install it via your OS's package manager.

To load completions in your current shell session:
$ source <(agc completion bash)

To load completions for every new session, execute once:
Linux:
  $ agc completion bash > /etc/bash_completion.d/agc
MacOS:
  $ agc completion bash > /usr/local/etc/bash_completion.d/agc

You will need to start a new shell for this setup to take effect.
  

```
agc completion bash
```

### Options

```
  -h, --help              help for bash
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

