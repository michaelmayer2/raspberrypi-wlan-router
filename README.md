#Raspberry Pi as WLAN router

## Config files

* '/etc/hostapd/hostapd.conf' : Host Access Point Daemon main config file. Please change WLAN passphrase and ssid 
* '/etc/dhcpd.conf' : DHCP Server config
* '/etc/rc.local' : Routing workaround - Please APPEND this file to /etc/rc.local
* '/etc/iptables.ipv4.nat' : Setting up NAT (used by /etc/rc.local) - Make sure the device names are correct


## Software needed

* hostapd
* isc-dhcp-server

## Result

* WLAN router ready to take connections 
* WLAN network 192.168.99.0/24
* Uplink via NAT and default route set
