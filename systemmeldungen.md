Systemmeldungen
===============
```/var/log/messages```  –  die Datei, die alle Betriebssystemeseitigen Fehler enthölt \(System-v Standard\)

```journalctl  ```                 – Systeme, die mit systemd arbeiten halten alle logs binär vor, mit "journlactl" kännen die Mitteilungen angeziegt werden.   
  
__Example:__
```journalctl -b -u sshd -f```  – Aanzeie aller meldungen den sshd betreffend \(-u sshd\) seit letzten Bot \(-b\)
(-f\) Bleibt offen, nachfolgende Meldungen werden aktuallisiert




