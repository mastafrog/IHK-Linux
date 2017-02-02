###Konfigurations Dateeien

`etc/hosts`
`/etc/nsswitch.conf` definiert die Reihenfolge der DNS
`/etc/resolv.conf` definiert Domäne und Nameserver
`/etc/netgroup`		konfig der Netzwerkgruppen aus verschiedenen Rechners

<div class="left">
#### Server1 
ssh-keygen -t rsa
scp ~/.ssh/id_rsa.pub user@server:/path

ssh user@server
</div>
<div class="right">
#### Server 2
su -user 
cat key.pub >> .ssh/authorized_keys
</div>
<style>
.left {
    width: 50%;
    }
.right {
    width: 50%;
    float: right;
    }
</style>