# bind
A powerful DNS server

# Contents
1) named.conf.option is the essential configuration of a private DNS server. 
2) bind9 is the file at which settings determine whether the DNS software works under IPv4 or IPv6 model.

# How to use
Install bind9, then edit the files under `/etc/bind` and `/etc/default`, respectively.

# To validity the DNSSec function
Use the dig command to verify the status of DNSSec function. Replace the DNS server's IP address to your own DNS server's. Pay meticulous attention to the last `.` after the domain you want to check.

Example, 
`dig @8.8.8.8 www.apnic.net. A +dnssec +multiline`

As for exemplifying, my test result is in attached file `dig.test.recursive.DNSSec`.

# Notice
1) After completion of your editing, make sure to run the command `sudo named-checkconf` to check if something pertinent to configuration is wrong. 
2) This setting enables DNSSec function.
