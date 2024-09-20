---
date: 2024-09-19T19:40:28-04:00
title: "agc project init"
slug: agc_project_init
---
## agc project init

Initialize current directory with a new empty AGC project for a particular workflow type.

### Synopsis

Initialize current directory with a new empty AGC project for a particular workflow type.
Project specification file 'agc-project.yaml' will be created in the current directory.

```
agc project init project_name --workflow-type {cwl|nextflow|snakemake|wdl} [flags]
```

### Examples

```

Initialize a new project named "myProject".
/code $ agc project init myProject --workflow-type my_workflow_type
```

### Options

```
  -h, --help                   help for init
  -w, --workflow-type string   uses the specified workflow type for the default context. Valid values include [cwl nextflow snakemake wdl]
```

### Options inherited from parent commands

```
      --format string   Format option for output. Valid options are: text, table, json
      --silent          Suppresses all diagnostic information.
  -v, --verbose         Display verbose diagnostic information.
```

### SEE ALSO

* [agc project]({{< relref "agc_project" >}})	 - Commands to interact with projects.

