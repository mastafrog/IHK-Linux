Systemmeldungen
===============

``/var/log/messages``  –  die Datei, die alle Betriebssystemeseitigen Fehler enthölt \(System-v Standard\)

``journalctl  ``                 – Systeme, die mit systemd arbeiten halten alle logs binär vor, mit "journlactl" kännen die Mitteilungen angeziegt werden.   
  
__Examples:__
___a)___``journalctl -b -u sshd -f``  – Aanzeie aller meldungen den sshd betreffend \(-u sshd\) seit letzten Bot \(-b\)

(-f\) Bleibt offen, nachfolgende Meldungen werden aktuallisiert
___b)___``journalctl --since "2017-01-29" --until "2017-02-01"``  Zeitraum Anzeige.

___c)___``journalctl -lab > /tmp/meldungen`` (a) Alle Meldungen in ausführlicher Form (l) seit letztem Boot (b)

___d)___ ``_PID=XXX, UID=XX`` Meldungen für spezifische Prozesse, User.


``dmesg`` – kernelmessages
``root-mail`` – Cronjobs