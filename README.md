# Mein Schießbuch v1.3.16

## Änderungen
- Bildbasierte PDFs ohne Textschicht werden nicht mehr nur als eine einzige Vollseite-OCR verarbeitet.
- Die gescannte Seite wird für Meyton-Protokolle in Kopf-/Ergebnisbereich und sechs separate Serienbereiche aufgeteilt.
- Jede Serie wird einzeln mit positionsbasierter Erkennung der zwei Schusszeilen ausgewertet.
- Serienübersicht und Gesamtergebnis bleiben die gedruckten Referenzwerte; erkannte Einzelschüsse überschreiben diese Werte nicht.
- Je Serie wird die Summe der zehn erkannten Schüsse gegen den gedruckten Serienwert geprüft.
- Die Gesamtsumme der Einzelschüsse wird separat gegen das Gesamtergebnis geprüft.
- Zähler werden nur übernommen, wenn eine eindeutige mathematische Zuordnung möglich ist.
- Fotoimport bleibt entfernt; PDF ist die einzige Importmöglichkeit.
- Originale PDF-Pfeilextraktion, Duplikatprüfung und IndexedDB `shootbook-v1` bleiben erhalten.
- Versionsanzeige und Service-Worker-Cache auf 1.3.16 aktualisiert.

## Einschränkungen und Teststatus
- OCR-Regionen sind auf das bekannte Meyton-Einseitenlayout ausgelegt.
- Mehrseitige PDFs werden seitenweise OCR-verarbeitet; die zusätzliche Serien-Übernahme nutzt die erste erkannte Scan-Seite.
- JavaScript-Syntax und Paketstruktur werden geprüft. Die tatsächliche OCR-Qualität muss mit dem Originalscan und auf Safari/iPhone praktisch getestet werden.


## Version 1.3.16
- iPhone-PDFs without a complete text layer now trigger OCR even if they contain stray extracted characters.
- OCR results are correctly passed to the import parser, including the six separately recognized series regions.
- Removed duplicated shot-consistency lines in the import preview.
- Existing native Meyton PDF text import remains the preferred path when the text layer is complete.
