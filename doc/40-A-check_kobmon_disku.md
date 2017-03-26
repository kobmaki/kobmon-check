# Documentation check_kobmon_disku ([back](00-A-documentation.md))

This check is for posix	filesystem.

## What is the check for?

* Filesystem usage on block level
* Free inodes
* Blocksize
* Mountpoint check
* Filesystem type

## Options

| Option | Info |
|---|---|
| -V | Show the programm version. |
| -p |  Require. Define the path to test.|
| -x | Flag, if the path must be a mount point |
| -s | Flag, if the underlying filesystem is a snapshot. E.g. an NFS-filesystem from a NetApp.
| -w | Warning in percent. Default is 10%. |
| -c | Critical in percent. Default is 5%. |


## Use case

TODO

## Examples

Test the home partition that it is a separate mountpoint. Set the warning on 28.5% and the critical on 15%

```
check_kobmon_disku -p /home -x -w 28.5 -c 15
```
