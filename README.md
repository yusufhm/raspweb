# Raspweb configuration
Contains the various configurations (common docker instances, etc..) for the Raspberry PI webserver.

## dnsmasq
The `/etc/resolvconf.conf` needs to be modified to allow `127.0.0.1` as a nameserver for `dnsmasq` to work; the following line needs to be uncommented:
```
name_servers=127.0.0.1
```
