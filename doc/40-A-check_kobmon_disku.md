# Documentation check_kobmon_disku ([back](00-A-documentation.md))

This check is for posix	filesystem.

## What is the check for?

* Filesystem usage on block level
* Free inodes
* Blocksize
* Mountpoint check
* Filesystem type (TODO)

## Options

| Option |  Info |
|---|---|
| *-V* | Show the programm version. |
| *-p* | Required. Define the path to test. |
| *-x* | Flag, if the path must be a mount point. Default not set. |
| *-s* | Flag, if the underlying filesystem is a snapshot. E.g. an NFS-filesystem from a NetApp.
| *-T* | Type of the underlying filesystem (TODO)|
| *-w* | Warning in percent. Default is 10%. |
| *-c* | Critical in percent. Default is 5.1%. |

## Use case

You want to check if a filesystem is a mount point. Simply add the flag option *-x*.

## Examples

Test the home partition that it is a separate mountpoint. Set the warning on 28.5% and the critical on 15%

```
check_kobmon_disku -p /home -x -w 28.5 -c 15
```

## Requirement for check_kobmon_disku

The check runs on linux. The check requires the command *df*, *stat*, *md5sum* in the search path. The checked path should be readable, otherwise a critical state is reported.

## Costs for running check_kobmon_disku

The time cost for the check is fast and run in milliseconds. The check could stock if a remote filesystem do not respond. E.g. a hard mounted NFS filesystem.
