# check_teamspeak3
Nagios/Icinga(2) Check for **Teamspeak™ 3 Server** via "voice" port


This perl script is a check script for Nagios™ & Icinga(2) for probing the status of a Teamspeak™ 3 server via its "voice" port *(default: 9987/udp)*.

The check is using a fixed packet sequence including the magic string `TS3INIT` to initialize a connection und waiting for a valid response. It is useful, if you don't have access to the "serverquery" port *(default: 10011/tcp)*, which allows to do telnet queries, or you really want to know, if the Teamspeak™ 3 server is (really) reachable from external.


**Warning: ANY USE OF THE SOFTWARE IS ENTIRELY AT YOUR OWN RISK** (because it's using a hacky predefined data stream which is usually not the way to go)
