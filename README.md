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

![Alt text](screenshot/servercheckSS.png?raw=true "Example usage")
![Alt text](screenshot/servercheckSS2.png?raw=true "Example usage")

Output is configurable with flags, run `server-check -h` for details

# Testing

There is a [Vagrant](https://www.vagrantup.com) box setup for this repository,
just in case you develop on a platform (like OSX) which isn't supported by the
script. Assuming you have `vagrant` installed you can:

```
export VAGRANT_OS=redhat # also accepts debian
vagrant up
vagrant ssh

[vagrant@localhost ~]$ sudo yum -y install sysstat
[vagrant@localhost ~]$ sudo /vagrant/server-check
```
