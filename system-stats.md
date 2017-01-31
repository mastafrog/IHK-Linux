# Systemzustände

runlevel     \_\_\_Anzeige des Runlevels \_\_\_

init &lt;runlevel&gt;     Ändern des runlevels

0         Rechner ausschalten

1         Single Usermode \(console\)

3        Multiuser + Netzwerk

5         % XServer

6         Rechner rebooten

/etc/inittab     Definitieon des Default runlevels

/etc/init.d    enthält skripte für dienste

chk config -l ssh     zeigt an, welchen Runleveln ssh gestartet wird

* ssh     ssh dienst wird dem aktuellen Runlevel hinzugefügt

rcssh start/stop/status     service steuerung

service statrt/stop/status     das gleiche unter debian

