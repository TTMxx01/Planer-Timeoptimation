PROJEKTPLANNER – iPhone-Web-App (öffentliche App ohne persönliche Startdaten)

GITHUB PAGES AKTIVIEREN:
1. Repository https://github.com/TTMxx01/Planer-Timeoptimation öffnen.
2. Settings → Pages → Deploy from a branch → main → /(root) → Save.
3. Im Anschluss https://ttmxx01.github.io/Planer-Timeoptimation/ in Safari öffnen.
4. Teilen → Zu Home-Bildschirm hinzufügen → Als Web-App öffnen → Hinzufügen.

PROJEKTDATEN:
Die öffentliche index.html enthält absichtlich keine persönlichen Projekte oder Aufgaben.
Dein JSON-Backup bleibt separat: Öffne in der App „Mehr“ → „Einstellungen“ → „JSON importieren“.
Ein Export in der App als HTML enthält wieder persönliche Daten und darf NICHT auf GitHub hochgeladen werden.
Alle Änderungen werden nur im lokalen Speicher des jeweiligen Geräts gehalten; keine automatische Gerätesynchronisierung.
Regelmäßig JSON-Backups erzeugen und sicher aufbewahren.

DATENSCHUTZ:
GitHub Pages ist auch bei einem privaten Repository keine private Zugriffsverwaltung.
Ältere Git-Commits bzw. hochgeladene ZIP-Dateien können frühere Projektdaten weiterhin enthalten.
Das Bereinigen der aktuellen Dateien entfernt solche Daten NICHT aus der Git-Historie.
Für eine vollständige Entfernung ist ein gesondertes Bereinigen der Historie bzw. ein neues Repository nötig.

TECHNISCH:
index.html / manifest.webmanifest / service-worker.js und icon-180.png,
icon-192.png, icon-512.png liegen nebeneinander im Repository-Hauptverzeichnis.
Nach erstem Onlineaufruf stellt der Service Worker die statischen Dateien für Offlinezugriff bereit.
