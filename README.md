# SoftHome
Sistema domestico di gestione energetica ed internet

Il primo file "stricmd" è praticamente l'eseguibile posizionato in /etc/init.d/; è il servizio.
Il secondo file "stricm" è uno script posizionato in /usr/sbin che viene richiamato dal primo script servizio.

E' inoltre necessario creare link simbilici del primo file nelle apposite directory

ln -s /etc/init.d/stricmd /etc/rc2.d/S98stricmd
ln -s /etc/init.d/stricmd /etc/rc3.d/S98stricmd
