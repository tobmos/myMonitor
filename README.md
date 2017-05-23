# myMonitor
Host monitoring

## Was ist myMonitor ??

MyMonitor ist ein Komplettmonitoring die vollversion ermöglicht es Server mit und ohne zugriff bestmöglichst zu überwachen, bestehend aus dem Monitorserver(ms) und den Monitorcients(mc für server mit zugriff). Der ms ermöglicht es spezifische Hostdaten in einer mongoDB basierten DB abzulegen und dessen Daten in einem Webinterface auf dem ms auszuwerten. 

Zusätzlich ermöglicht der ms regelmäßige nmap scans zu hinterlegen, somit realisiert man eine Überwachung von UP and Down times, Offene Ports, Dienste und deren Versionierungen. 

Es gibt drei mögliche installations Varianten. 

## 1. Only Monitoring 

sh ./myMonitor

Dieses Paket beinhaltet die installations von MongoDB, Apache und Nmap. Nach erfolgreichem abschluss der installation sollten sie das Webinterface über IP:80 ereichen können. Nun können sie mit der eingabe der IP oder domain neue Hosts hinzufügen.
Über die voreinstellungen können sie die gewünschten hostdaten und scan intervalle einstellen. Die nun hinzugefügten Hosts werden nun auf dem maintable dargestellt.

## 2. Monitoring von Server mit zugriff 

ms -> sh ./myMonitor
mc -Y sh ./myClient ID // z.B.: sh ./myClient 1

