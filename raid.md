`mdadm --create /dev/md0 --raid-devices=2 --level=1 /dev/sdc7 /dev/sdc8`

`cat /proc/mdstats`

`mdadm -D /dev/md0`

`mkfs -t ext4 /dev0/testvol`

`mkdir /home/tag4`

`vi /etc/fstab`

`grep tag4 /etc/fstab`

`/dev/vg9/tesetvol /home/tag4 ext defaluts 0 1 `trägt den device in den verzeichnissbaum

0 für keine logs

1 für nacht dem crash checken erst nach system vol

`mount -a`

`df -h /home/tag4 #glech mounten`

`lvextend -L #48M #`

`dd if=0`

`lvdisplay /dev/vg0/testvol  #sollte vergrösserte Vol zeigen`

`df -h /home/tag4  
`

`resize2fs /dev/vg0/testvol`



### Spiegel erstellen

Raid 2 aus sdc5 & 6

`mdadm --create /dev/md0 --raid-devices=2 --level=1 /dev/sdc5 /dev/sdc6`

Check

`cat /proc/mdstat ` in vol rein packe

`vgextend vg9 /dev/md1`

Kopieren

`dd ....`

rausschmeißen  
`vgreduce vg0 &dev/md0`



### Snapshots

`vgs` status abfrage

`lvcreate -L +50M`

`df /home/tag4`

`lvconvert --merge /dev/vg0/testsnap`

`ls /home/tag4/kartoffel`

`unount /home/tag4`

`lvchange -a n /dev/vg0/testsnap `\#unmount \#war vorher schon gemountet

`lvchange -a y /dev/vg0/testsnap `\#mount

