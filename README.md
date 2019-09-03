# bind
A powerful DNS server

# Contents
1) named.conf.option is the essential configuration of a private DNS server. 
2) bind9 is the file at which settings determine whether the DNS software works under IPv4 or IPv6 model.

# How to use
Install bind9, then edit the files under `/etc/bind` and `/etc/default`, respectively.

#Notice
After completion of your editing, make sure to run the command `sudo named-checkconf` to check if something pertinent to configuration is wrong.
