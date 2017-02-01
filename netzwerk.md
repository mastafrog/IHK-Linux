### Netzwerk

`ifconfig -a` -- Anzweige aller NIC's (Network Interface Card)
> Fnerster &nbsp &nbsp &nbsp &nbsp . &nbsp &nbsp &nbsp &nbsp . Gang
  10 &nbsp 20 &nbsp 30.  &nbsp 40&nbsp &nbsp .
. &nbsp &nbsp &nbsp &nbsp . &nbsp &nbsp &nbsp &nbsp . &nbsp &nbsp &nbsp &nbsp . 

`if congi eth1` outputs
> `192.168.050` 
`netmask 255.255.255.0`
`mtu 1500`
`up`

`ping -b`

`arp -a` - ARP protocol
`ifdown etc`

>`# The loopback network interface
auto lo
iface lo inet loopback 

# The primary network interface
allow-hotplug eth0
iface eth0 inet dhcp
iface eth1 inet static
address 192.168.20.100
netmask 255.255.255.0
broadcast 192.168.20.255
`

#####Alt -> RHEL
`_ifconfg-eth1:_
 &nbsp &nbsp BOOTPROTO='static'
 &nbsp &nbsp IPADDR='192...'
 &nbsp &nbsp NETMASK='255....'
 _ifcfg-eth90:
 &nbsp &nbsp BOOTPROTO='dhcp'
`
`ifdown eth 1 ` deactivate
`ifup eth 1 ` activate

