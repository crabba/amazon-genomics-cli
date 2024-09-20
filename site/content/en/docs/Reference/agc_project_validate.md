---
date: 2024-09-19T19:40:28-04:00
title: "agc project validate"
slug: agc_project_validate
---
## agc project validate

Validate an agc-project.yaml file

### Synopsis

Determines if the current project specification follows the required format and lists any syntax errors. 
The current project specification is determined to be the agc-project.yaml file in the current working directory or a parent of the current directory
Output of the command has following format:
PROJECT: Name
DATA: Location ReadOnly


```
agc project validate [flags]
```

### Examples

```

/code agc project describe
```

### Options

```
  -h, --help   help for validate
```

### Options inherited from parent commands

```
      --format string   Format option for output. Valid options are: text, table, json
      --silent          Suppresses all diagnostic information.
  -v, --verbose         Display verbose diagnostic information.
```

### SEE ALSO

* [agc project]({{< relref "agc_project" >}})	 - Commands to interact with projects.

