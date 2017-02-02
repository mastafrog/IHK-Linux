### Bonding


zwei karten werden zu einer logischer einheit zusammengefasst. Gedacht als ausfall Sicherheit. Macht sinn '


In: `__/et/sysconfig/networkifcfg-bond0__`

> `BONDING_MASETER='yes'
  BONDING_MODULE_OPTS='mode=active-bachup'
  BONDING_SLAVE0='eth2'
  BONDING_SLAVE1='eth3'
  BOOTPROTO='static'
  IPADDR=
  NETMASK=
  STARTMODE='auto'`
  

---------------
    
`mode=active-backup __mode 1__ <– 1 aktive NIC (SLAVE0), 1NIC IM Standby (Slave1)
       balance-rr (Mode 0) <- 2 aktive NIC (round robin)
       802.3ad 	  (Mode 4) <– 2 physische 1GB Verbindung werden zu 1em logischen 2Gb Verbindugn zusammengefasst
       LACP - Link Aggregation Control porotokoll) `
  ---------------


### Debian-Bounding
`apt-get nstall ifenslave
vi /etc/network/interfaces:
	auto bond0
	iface bond0 inet static
	...
	wiki.debian.org/Bonding`

-------------------
`BOOTPROTO='static'
ETHERNETDEVICE=bond


iface lo ninet loopback`

### The primary network interface
`allow-hotplg eth0
auto eth1
iface eth0 inet dhcp
iface eth1 inet static
address 192.168.20.100
netmask 255.255.255.0
broadcast 192.168.20.255

auto eth1:vl10
iface eth:vl10 inet static
address 
netmask 
broadcast 92.168.20.255

auto eth2
iface eth2 inet dhcp
auto eth3
iface eth3 


ifup bond0`

