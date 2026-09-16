# ToDo-Applikation mit Node.js und Docker


# Materialien

Für die Installation und Ausführung des Projekts werden folgende Programme benötigt:

Git
Node.js
npm
Docker Desktop
Visual Studio Code


# 1. Repository klonen

Zuerst muss das GitHub-Repository auf den eigenen Computer geklont werden.

Das Repository kann mit folgendem Befehl in Terminal von VS-Code geklont werden:


git clone https://github.com/DEIN-BENUTZERNAME/docker-nodejs-sample.git



Anschließend in das Projekt wechseln:


cd docker-nodejs-sample


# 2. Projekt öffnen

Das Projekt kann anschließend geöffnet werden.



Danach sollte die Projektstruktur ungefähr so aussehen:


docker-nodejs-sample
─ spec
─ src
─ .gitignore
─ package-lock.json
─ package.json
─ README.md


# 3. Node.js und npm überprüfen

Vor der Installation sollte überprüft werden, ob Node.js und npm installiert sind.
In Terminal folgendes eingeben:

node --version


und:


npm --version


Wenn beide Befehle eine Versionsnummer ausgeben, sind Node.js und npm verfügbar.


# 4. Abhängigkeiten installieren

Die benötigten Node.js-Pakete werden mit npm installiert.

Im Hauptverzeichnis des Projekts folgenden Befehl ausführen:


npm install


# 5. Anwendung testen

Vor der Containerisierung sollte die Anwendung getestet werden.

Ordner wechseln zu C:\Users\DEIN BENUTZERNAME\Desktop\VS-Code\docker-nodejs-sample mit folgendem befehl:

cd docker-nodejs-sample

Dazu kann der Entwicklungsserver mit folgendem Befehl gestartet werden:


npm run dev


Wenn die Anwendung erfolgreich startet, kann sie über die im Terminal angegebene Adresse aufgerufen werden.

Zum Beenden des Servers folgendes drücken:


Ctrl + C


# 6. Docker installieren

Für die Containerisierung wird Docker benötigt.

Dazu muss Docker Desktop installiert werden.

Nach der Installation sollte überprüft werden, ob Docker funktioniert:


docker --version



Docker Desktop muss während der Arbeit gestartet sein.


# 7. Docker-Dateien erstellen

Für die Containerisierung werden folgende Dateien benötigt:

text
docker-nodejs-sample/
├── Dockerfile
├── .dockerignore
├── package.json
├── package-lock.json
├── src/
├── spec/
└── README.md


# 8. Docker Image erstellen

Nachdem die Docker-Dateien erstellt wurden, wird das Docker-Image erstellt.

In Terminal folgendes eingeben:


docker build -t todo-app .


# 9. Docker Container starten

Der Container kann anschließend mit folgendem Befehl gestartet werden:


docker run -p 3000:3000 todo-app

Die Anwendung kann anschließend im Browser aufgerufen werden:

http://localhost:3000


# 10. Laufende Container überprüfen

Mit folgendem Befehl können alle aktuell laufenden Docker-Container angezeigt werden:


docker ps


Dadurch kann überprüft werden, ob die ToDo-Applikation erfolgreich als Container ausgeführt wird.

# Wichtige befehle

cd C:\Users\Novak\Desktop\VS-Code\docker-nodejs-sample

npm run dev

docker compose up --build

ctrl + c

docker compose down

http://localhost:3000

--------------------------------------

git status
git add .
git commit -m "Aktualisierungen"
git push

**Novak Jocic**
