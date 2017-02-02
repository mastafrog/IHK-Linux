###Konfigurations Dateien

`etc/hosts`
`/etc/nsswitch.conf` definiert die Reihenfolge der DNS
`/etc/resolv.conf` definiert Domäne und Nameserver
`/etc/netgroup`		konfig der Netzwerkgruppen aus verschiedenen Rechners

#### Server1 
ssh-keygen -t rsa
scp ~/.ssh/id_rsa.pub user@server:/path

ssh user@server

#### Server 2
su -user 
cat key.pub >> .ssh/authorized_keys


## Tunnel
ssh -X -L 13389: windowshost:3389 -l userAufTunnelServer 


Notebook --ssh--> tunnel server --> Zielserver:port
< ------------- ssh map on local port --------------


