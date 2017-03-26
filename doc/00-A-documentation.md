# Documentation kobmon-check
The kobmon-check contains primerly checks for Linux OS systems. It is a collection of checks that I created, because non of the available checks (around 2000..) satisfy me.  

I used some technic to visualize things, that you usually couldn't visualize with PNP, like hostnames or MD5 sums.
# The checks
All my checks have the name the prefix check_kobmon. The following checks contains only a short description. Detail information in the corresponding documentation page.
## [check_kobmon_hostname](40-A-check_kobmon_hostname.md)
This check is for checking hostnames and things around it.
## [check_kobmon_disku](40-A-check_kobmon_disku.md)
Checks the diskusage. Enables limit in percentage and additional infos around the used filesystem.
## [check_kobmon_eping](40-A-check_kobmon_eping.md)
Extend and faster ping. It is based on the os ping.
## [check_kobmon_uload](40-A-check_kobmon_uload.md)
Checks the load and gives more infos the the classic check_load.
## [check_kobmon_ntpq](40-A-check_kobmon_ntpq.md)
Checks the used timeserver.
## [check_kobmon_prg](40-A-check_kobmon_prg.md)
Checks for a programm under linux.
## [check_kobmon_prg](40-A-check_kobmon_vmstat.md)
Checks OS with the command vmstat under linux.