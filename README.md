# server-check

A bash script written to gather data about a server. Using sysstat (sar reports),
it aims to provide average memory and cpu usage for a device as well as other
relevant details about the server.

Originally written by Sam Sharpe ( https://github.com/samjsharpe ) He has asked 
that this be dedicated to "all the Rackers past and present whose ideas I probably 
stole while making the original script." A dedication I heartily second as someone
that cobbles together one liners when I see cool stuff other people are doing. ;)

Currently supports Redhat variants (ES, CentOS, Fedora) and Debian/Ubuntu.

Others may be added at a future date.

Usage: /path/to/binary/server-check

Example:

[darke@pinja server-check]$ ./server-check 

CPU Installed    : 1 x Intel(R) Core(TM) i5-2500 CPU @ 3.30GHz (4 cores per proc)
Peak CPU Usage   : 10.90 %
Avg. CPU Usage   : 8.15 %

Ram Installed    : 16 GB
Peak RAM Usage   : 14.03 %
Avg. RAM Usage   : 13.60 %

Filesystem Usage :
   /                    50G        24% used
   /boot                477M       36% used
   /home                172G       2% used
   /home/darke          917G       48% used

OS Version       : Fedora 20 (Heisenbug)
PHP Version      : 5.5.21
MySQL Version    : 5.5.41-MariaDB

