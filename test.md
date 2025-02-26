
# überschrift
##
###

```bash
sudo apt-get update && sudo apt-get upgrade
ifconfig 
ssh arek@<ipadresse> #um über das Windows Terminal auf das Linux Terminal eine verbindung zu etablieren.
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
cat / cowsay 
grep <keyword> <filename> #sucht nach dem bestimmten
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

# Docker Befehle
```bash
## Docker Container und Image Befehle
docker --version #Zeigt aktuelle Version an
docker pull <image> #lädt ein Docker image aus Registry runter
docker build -t <name> #Baut ein Docker image aus einem Dockerfile im Aktuellen Verzeichnis
docker run <image> #Startet einen Container im interaktiven Modus (bspweise Shell)
docker ps -a #Zeigt alle Container(auch gestoppte) an
docker stop <container_id> #Stoppt einen laufenden Container
docker start <container_id> #Staretet einen gestoppten Container
docker restart <container_id> #restartet Container
docker rm <container_id> #entfernt einen Container

## Management und Logs
docker exec -it <container_id> bash #Öffnet eine Bash-Shell in einem laufenden Container
docker logs <container_id> #Zeigt die Logs eines Containers an
docker inspect <container_id> #Zeigt detailierte informationen zu einem Container

## Netzwerke und Volumes
docker network ls #Listet alle Docker-Netze auf
docker volume ls # Listet alle Docker-Volumes auf
docker network create <network_name> #Erstellt ein neues Docker Netzwerk
docker volume create <volume_name> #Erstellt ein neues Docker Volume
docker run -v <volume_name>:/pfad/in/container <image> #Verwendet ein Volume beim

## Docker Compose
docker-compose --version #Zeigt die Version von Docker #compose an
docker-compose up #startet alle Container in einem Docker Compose Projekt
docker-compose down #Stoppt und entfernt alle Container eines Docker Compose Projekts
docker-compose logs #Zeigt die Logs für alle Container eines Docker Compose Projekts an
docker-compose build #Baut die Docker Images für ein Projekt basierend auf der docker-compose.yml
```