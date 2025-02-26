
# überschrift
##
###

```bash
sudo apt-get update && sudo apt-get upgrade
```
# Verzeichnisse und Dateien handlen
```bash
mkdir /<test>
mkdir -p /<test>
# -p um direkt eine datei am ende des Pfades zu erstellen
rmdir #löscht ein leeres Verzeichnis
rm #löscht datei aus einem Verzeichnis
rm -r #löscht Verzeichnis oder datei
cat <dateiname> #zeigt inhalt einer datei
nano <dateiname> #öffnet die datei im nano editor
cp <dateiname> #kopiert datei aus einem Verzeichnis
mv #verschiebt oder benennt Dateien oder Verzeichnisse um
touch <neuedateiname> #Erstellt eine Datei.
```

# Zurechtfindung
```bash
ls #zeigt files im directory an
ls -l #detailiert-a
ls -a #auch versteckte datein
pwd #zeigt den aktuellen Arbeitsverzeichnis-Pfad an
cd #wechselt verzeichnis
cd /<pfad>/<zum>/verzeichnis>
find . -name "dateiname" #sucht nach Dateien im Verzeichnisstree(nur nötig bei Komplexeren verzeichnissen)
whoami #zeigt aktuellen benutzer an

```

# Benutzerverwaltung / Rechte
```bash
sudo #führt den Befehl mit Admin rechten aus
chmod #ändert datei berechtigung
chown #ändert den Besitzer einer Datei
useradd #fügt hinzu 
usermod #ändert
userdel #löscht
passwd #ändert das Passwort des Benutzers


```

# Systeminformationen und Prozesse
```bash
top #Zeigt laufende Prozesse und Systemressourcen an
ps #Zeigt laufende Prozesse an
ps aux #Zeigt Prozesse alle an
df #zeigt Festplattenplatz an
free #zeigt Speichernutzung an
uptime #Zeigt an, wie lange das Betrieb läuft
ping 8.8.8.8 #Testet verbindung zu einer Adresse, hier als beispiel google
ifconfig #Zeigt Netzwerkschnittstellen um IP-Adresse an.
ip a #         |^|
netstat #Zeigt aktive Netzverbindungen und offene Ports
wget #Lädt Dateien aus dem Internet Herunter
curl #holt inhalte von einer URL oder sendet HTTP-Anfragen
```

