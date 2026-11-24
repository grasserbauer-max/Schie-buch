# Mein Schießbuch – iPhone-PWA v1.0.2

- Wettkampf und Training getrennt
- Ergebnis- und Serien-Diagramme
- PDF-Import mit Vorschau und Kategorienkontrolle
- manuelle Eingabe, Details, Rekorde, Trefferkreis und Trefferlage
- Backup als JSON
- Aktualisieren-Schaltfläche und Versionsanzeige im Footer

## Keine vorinstallierten Ergebnisse
Die App startet mit einem leeren Archiv. Es werden keine der vom Nutzer gesendeten PDFs oder Ergebnisse automatisch hochgeladen oder vorausgefüllt. Bitte importiere deine eigenen Ergebnis-PDFs selbst.

## PDF-Import
Die App ist auf textbasierte Meyton-PDFs ausgelegt. Bei der Trefferlage wird nur der Wert aus dem Kopfbereich vor „Serie 1“ gelesen, nicht der restliche Seiteninhalt. PDFs mit abweichendem Format bitte vor dem Speichern in der Importvorschau kontrollieren.

## Hosting
GitHub Pages: Repository-Dateien ins Hauptverzeichnis hochladen, Settings → Pages → Deploy from a branch → main → /(root). Anschließend HTTPS-Adresse in Safari öffnen und „Zum Home-Bildschirm“ wählen.

## Speicherung
Lokal im Browser (IndexedDB). Für eine iCloud-Kopie „Backup“ wählen und JSON in iCloud Drive speichern. Keine automatische iCloud-Synchronisierung.
