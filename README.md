tcpdump -vvv -i(interface) eth1 -q '(tcp port 443) or (tcp port 80)' -0 (kompletter paketinhalt -w /path.tcp.dump 
firewall

firewall-cmd --state # if active
			--get-active-zones #aktive zonen (dmz, internal...)

firewall -cmd --permanent --add-interface=eth1 --zone=public
						  --add-service = http
						  --add-port = 3389/tcp --zone=public

firewall-cmd --reload

firewall-cmd --list-all 	#blockt alles
firewall-cmd --panic-on/off

/etc/firewalld/firewald.com
/etc/firewalld/zones
			  /services

firewall-config



754 root execute and read

chmod u+x, chmod g+x

useradd -m  /etc/passwd
passwd      /etc/shadow


un/mounten hieratchisch

fdisk parted schnibbeln

mkfs -t ex4 path formatieren

mount -a alles mounten

fsck -y überprüfen




