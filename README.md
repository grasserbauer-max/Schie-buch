# Mein Schießbuch – Version 1.3.1

## Änderungen
- PDF-Import erkennt weiterhin echte PDF-Texte direkt über PDF.js.
- Bei PDFs ohne auslesbare Textebene wird automatisch OCR (Tesseract.js, Deutsch/Englisch) auf den gerenderten PDF-Seiten ausgeführt.
- Importvorschau zeigt zusätzlich erkannte Schützen-/Start-/Standdaten, Serien, Einzelschüsse, Zähler und weitere Meyton-Felder.
- Dokument-Duplikatprüfung: SHA-256-Dateiprüfsumme sowie Vergleich von Kategorie, Disziplin, Datum, Ergebnis und Serien. Bei möglichem Duplikat erscheint eine Bestätigung.
- Datenbankname bleibt unverändert `shootbook-v1`.
- Service-Worker-Cache auf `schiessbuch-v1.3.1` aktualisiert.

## Hinweise und Grenzen
- OCR und PDF.js benötigen beim Import eine Internetverbindung (CDN-Bibliotheken).
- OCR-Ergebnisse können insbesondere bei kleinen Ziffern, Zählerlisten und Schusswerten fehlerhaft oder unvollständig sein. Die Vorschau muss vor dem Speichern kontrolliert werden. Nicht sicher erkannte Werte werden nicht als garantiert korrekt ausgegeben.
- Bei eingescannten PDFs bleiben die Trefferbilder im Dokument erhalten, aber Pfeil-/Richtungssymbole können nicht zuverlässig aus OCR rekonstruiert werden. Für die Pfeile weiterhin möglichst das originale, digitale Meyton-PDF importieren.
- Die Duplikatprüfung erkennt identische Dateien über SHA-256. Neu gescannte Kopien werden zusätzlich anhand der erkannten Ergebnisdaten verglichen; bei OCR-Abweichungen ist eine Erkennung nicht garantiert.
- Speicherung bleibt lokal im Browser/IndexedDB. Es gibt keine automatische iCloud-Synchronisierung.

## Installation
Alle Dateien auf GitHub Pages hochladen und die vorhandenen App-Dateien ersetzen. Die bestehende IndexedDB `shootbook-v1` wird weiterverwendet und nicht gelöscht oder umbenannt.
