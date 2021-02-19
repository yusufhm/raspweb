# PiMedia configuration
Contains the various configurations (common docker instances, etc..) for the Raspberry Pi webserver.

## dnsmasq
`resolvconf` is required on the Pi for the proper configuration of dnsmasq.

```
sudo apt install -y resolvconf
```

Then configure it with the following:
```
echo 'nameserver 127.0.0.1' | sudo tee --append /etc/resolvconf/resolv.conf.d/head
sudo resolvconf -u
```
