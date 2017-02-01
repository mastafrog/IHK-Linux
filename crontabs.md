##Cronjobs

`crontab -l[-u <user>] ` > Anzeige periodisch wiederkehren der Aungaben.
`crontab` -e - Modifizieren % % % (vi)

>`Debian:  /var/spool/cron/tabs`
>`SLES /var/spool/cron/tabs`

Verzeichnis, in dem sich die Dateien mit den wiederkehrenden Aufgaben für jeden user befinden.

`SLES /var/spool/cron/tabs`
`man 5 crontabs`Manpages

![](https://jumpcloud.com/assets/glossary/crontab/001-8932bb3fb07f73dfd0a6c0c779f349b1.gif)

__Example:__
+ `/bin/tar cf /var/tmp/save.tar /etc/*conf ` _Tar wird täglich um 10:45 Uhr ausgeführt_
+ `0-59/4 * * * * *` /bin/tar ... _Viertelstündige Ausführung_