# Mein Schießbuch – Version 1.3.2

## Änderungen
- OCR-Erkennung für gescannte PDFs mit höherer Renderauflösung und Layout-Erkennung.
- Bei OCR werden erkannte Schusswertpositionen verwendet, um die unmittelbar rechts daneben gedruckten Richtungspfeile aus dem gerenderten Dokumentbild auszuschneiden.
- Bei digitalen Meyton-PDFs werden die Pfeile weiterhin aus dem gerenderten PDF-Bereich neben den Schusswerten extrahiert.
- Pfeile werden nur dann automatisch Schüssen zugeordnet, wenn die Anzahl der erkannten Schusswerte und Pfeilausschnitte exakt übereinstimmt. Bei abweichender Anzahl bleiben sie unzugeordnet, statt möglicherweise falsche Richtungen anzuzeigen.
- Die Importvorschau kontrolliert weiterhin, ob bei LG 60 ZR sechs Serien mit jeweils zehn Einzelschüssen und elf Zählerwerten erkannt wurden.
- Duplikatprüfung über SHA-256 sowie Vergleich von Kategorie, Disziplin, Datum, Ergebnis und Serien bleibt erhalten.
- Datenbankname bleibt unverändert `shootbook-v1`.
- Service-Worker-Cache auf `schiessbuch-v1.3.2` aktualisiert.

## Hinweise und Grenzen
- OCR und PDF.js benötigen beim Import eine Internetverbindung (CDN-Bibliotheken).
- OCR kann insbesondere bei kleinen Ziffern, Zählerlisten und Pfeilsymbolen Fehler machen. Die Vorschau muss vor dem Speichern kontrolliert werden.
- Pfeile werden anhand der OCR-Wortposition aus dem unmittelbar rechts angrenzenden Bildbereich ausgeschnitten. Bei schlechter Scanqualität oder abweichendem Layout kann die Pfeilerkennung ausbleiben. Die App ordnet Pfeile nur bei exakt passender Anzahl zu.
- Die Duplikatprüfung erkennt identische Dateien über SHA-256. Neu gescannte Kopien werden zusätzlich anhand der erkannten Ergebnisdaten verglichen; bei OCR-Abweichungen ist eine Erkennung nicht garantiert.
- Die JavaScript-Syntax und das ZIP-Archiv wurden geprüft. Ein vollständiger OCR-/Pfeil-Funktionstest in einem iPhone-Browser mit dem vorliegenden Scan wurde nicht durchgeführt. Daher ist die zuverlässige Erkennung aller 60 Schüsse und Pfeile noch nicht als bestanden bestätigt.
- Speicherung bleibt lokal im Browser/IndexedDB. Es gibt keine automatische iCloud-Synchronisierung.

## Installation
Alle Dateien auf GitHub Pages hochladen und die vorhandenen App-Dateien ersetzen. Die bestehende IndexedDB `shootbook-v1` wird weiterverwendet und nicht gelöscht oder umbenannt.
