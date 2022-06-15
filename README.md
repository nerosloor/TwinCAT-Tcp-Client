# Twincat-Tcp-Client

## Beckhoff TwinCAT 3 TCP Client

Dieser FB baut eine `Socketverbindung` mittels des Beckhoff eigenen Sublements `TF6310` auf.
Dabei handelt es sich um einen TCP/IP-Server, der TCP managed.
Via TCP können Messages an einen Ziel-Server gesendet werden. 
Messages von dem Ziel-Server können dann empfangen werden.
Es handelt sich also um einen `TCP-Client`.
```
Benötigte Bibliotheken:
* Tc2_TcpIp
* Tc2_Utilities
	
Benötigte Lizenzen:
* TF6310
```
Weiteres:
Außerdem wird das Sublement `TF6310-TCP-IP.exe` benötigt.
Dahinter verbirgt sich ein Server, der die Kopplung zu den verwendeten Sockets vornimmt.
Der Server kann von der Beckhoff Seite herunter geladen werden.
Danach sollte der Server auch gestartet werden. Die exe ist zu finden unter `C:\TwinCAT\Functions\TF6310-TCP-IP\Win32\Server`
