PROJEKTPLANNER MASTER 1.3 – IPHONE-WEB-APP (PWA)

ENTHALTEN
index.html, manifest.webmanifest, service-worker.js, icons/icon-180.png, icons/icon-192.png, icons/icon-512.png

INSTALLATION AUF DEM IPHONE
1. Gesamten Inhalt dieses ZIP entpacken.
2. Den Ordnerinhalt UNVERÄNDERT in ein HTTPS-Webverzeichnis hochladen (z. B. privater Webspace oder passwortgeschütztes Hosting). Die Dateien müssen nebeneinander liegen, icons/ im Unterordner.
3. Die URL zu index.html in Safari auf dem iPhone öffnen.
4. In Safari: Teilen > Zu Home-Bildschirm hinzufügen > (ggf. Als Web-App öffnen aktivieren) > Hinzufügen.
5. Das Symbol „Planner“ auf dem iPhone-Home-Bildschirm antippen.
6. Nach einer vollständigen ersten Ladung funktioniert die App auch offline.

HOME-BILDSCHIRM
- Unten auf „Home“ tippen: direkt zurück zur nächsten Aufgabe.
- Liegen neue, nicht bestätigte To-do-Vorschläge vor, öffnet sich beim App-Start weiterhin der Prüfbereich.
- Unten: Home | Neue To-dos | Aufgaben | Projekte | Mehr.
- „Mehr“ enthält Übersicht, Kanban, Zeitplan, ChatGPT und Einstellungen.

DATENSCHUTZ & DATENSICHERUNG
- Der Quellcode enthält bereits die ursprünglichen zwölf Projekte / 51 Aufgaben: Wer die gehosteten Dateien herunterladen darf, kann diese Ausgangsinformation sehen! Deshalb ausschließlich privat oder zugriffsgeschützt hosten.
- Neue Eingaben werden lokal auf dem jeweiligen Gerät gespeichert; es gibt keine automatische Synchronisation zwischen iPhone und PC oder zu ChatGPT.
- Aus der älteren HTML-Datei zuerst in deren Einstellungen JSON exportieren, dann in der PWA über Einstellungen > JSON importieren. Ein vorhandener lokaler Datenstand ist nicht automatisch übertragbar.
- Regelmäßig JSON-Backups in der Dateien-App sichern, besonders vor Updates, iOS-Speicherbereinigung oder Neuinstallation.
- Bei Browser-/Web-App-Deinstallation können lokal gespeicherte Daten verloren gehen.
- Auf „file://“-Dateien (lokal aus der Dateien-App) funktioniert die Service-Worker-Installation nicht. HTTPS ist für eine echte PWA erforderlich.

TEST AUF DESKTOP
Im Ordner lokal einen Webserver starten, z. B.: python3 -m http.server 8765
Dann im Browser http://localhost:8765/index.html öffnen. http://localhost gilt für PWA-Tests als sicherer Kontext.

WICHTIG
Bei einer bereits genutzten Installation können Daten durch neue, anders konfigurierte Domain-URLs nicht übertragen werden. Vor einem Domainwechsel JSON sichern.
