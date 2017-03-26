# Documentation check_kobmon_hostname ([back](00-A-documentation.md))

This check is usefull in cluster environment.

## What is the check for?

* Know if a domain is set on a host
* Where is a cluster ip?
* Do you have a wrong IP on a machine

## Options

| Option | Info |
|---|---|
| -V | show the version |
| -d | domain to check |
| -s | short name of the host |
| -i | ip of the machine |

## Examples

TODO

## Use case

The domain should be set on every host. The Default behavior is, that no domain name gives a warning.

## Use case: Where is my IP?

In a cluster you switch an IP. Sometimes you want to know on which host is your ip. Run this check agains the cluster ip and you see where it is.
