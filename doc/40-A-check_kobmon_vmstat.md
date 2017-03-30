# Documentation  [back](00-A-documentation.md)
TODO
([back](00-A-documentation.md))

This check is for system usage overview..

## What is the check for?

* Usage IO
* Usage system time
* Idle time
* Wait time
* Stolen time

## Options

| Option |  Info |
|---|---|
| *-V* | Show the programm version. |
| *-w* | Warning in percent. Default is 10%. |
| *-c* | Critical in percent. Default is 5.1%. |

## Use case

TODO

## Examples

```
check_kobmon_vmstat
```

## Requirement for check_kobmon_vmstat

The check runs on linux. The check requires the command *vmwstat* in the search path.

## Costs for running check_kobmon_disku

The time cost for the check is fast and run in 10 seconds.
