---
date: 2024-09-19T19:40:28-04:00
title: "agc account deactivate"
slug: agc_account_deactivate
---
## agc account deactivate

Deactivate AGC in an AWS account.

### Synopsis

Deactivate AGC in an AWS account.
AGC will use your default AWS credentials to remove all core AWS resources
it has created in that account and region. Deactivation may take up to 5 minutes to complete and return.
Buckets and logs will be preserved.

```
agc account deactivate [flags]
```

### Examples

```

Deactivate AGC in your AWS account.
/code $ agc account deactivate
```

### Options

```
  -f, --force   Force account deactivation by removing all resources associated with AGC.
                This includes project and context resources, even if they are running workflows.
                If not specified, only the core resources will be deleted if possible.
  -h, --help    help for deactivate
```

### Options inherited from parent commands

```
  -p, --awsProfile string   Use the provided AWS CLI profile.
      --format string       Format option for output. Valid options are: text, table, json
      --silent              Suppresses all diagnostic information.
  -v, --verbose             Display verbose diagnostic information.
```

### SEE ALSO

* [agc account]({{< relref "agc_account" >}})	 - Commands for AWS account setup.
Install or remove AGC from your account.

