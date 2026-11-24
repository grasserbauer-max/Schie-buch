# Mein Schießbuch – iPhone-PWA

Die Web-App bietet getrennte Ansichten für Wettkämpfe und Training, Ergebnis- und Serien-Diagramme, Innenzehner, Trefferkreis, Trefferlage, Rekorde, PDF-Import, manuelle Eingabe und JSON-Backup.

## Daten und iCloud
Ergebnisse werden lokal im Safari-Browser (IndexedDB) gespeichert. Es gibt keine automatische iCloud-Synchronisierung. Über „Backup“ kann eine JSON-Datei erzeugt und in der iPhone-Dateien-App unter iCloud Drive gespeichert werden; diese Datei kann später wieder importiert werden.

## Auf iPhone installieren – ohne Mac
Die App benötigt eine HTTPS-Adresse, damit „Zum Home-Bildschirm“ und der Service Worker funktionieren. Du kannst den Ordnerinhalt z. B. über GitHub Pages veröffentlichen:
1. Auf github.com ein Repository erstellen.
2. Diese Dateien hochladen.
3. Repository Settings → Pages → Deploy from branch → main → /(root).
4. Die HTTPS-Adresse in Safari öffnen → Teilen → Zum Home-Bildschirm.

PDF.js wird beim PDF-Import von einem CDN geladen; dafür ist eine Internetverbindung erforderlich. Der Import ist auf textbasierte Meyton-PDFs ausgelegt. Die Beispiel-Probe-PDF mit `inv`-Ergebnis hat kein normales Ring-Gesamtergebnis und kann daher nicht automatisch als Ring-Ergebnis importiert werden; bitte dafür manuell erfassen oder ein anderes Trainingsergebnis-PDF verwenden.

Die beiden verifizierten Wettkampfergebnisse 599,9 und 606,4 sind als Startdaten eingebaut. Die Probe-PDF wurde nicht als gültiges Ergebnis übernommen.
