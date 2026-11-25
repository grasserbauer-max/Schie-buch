# Mein Schießbuch v1.3.6

## Änderungen
- Foto-OCR wird in getrennte Bereiche aufgeteilt: Kopf-/Ergebnisbereich, Zählerbereich und sechs Serienbereiche.
- Das Gesamtergebnis wird unabhängig vom OCR-Text der Serien gelesen.
- Die sechs Serienüberschriften werden anhand der Serienzeile im Kopfbereich normalisiert.
- Pro Serie werden zehn Einzelschüsse separat ausgelesen.
- Die Ganzring-Summe einer Serie wird aus den zehn erkannten Einzelschüssen abgeleitet und in der Vorschau angezeigt.
- Zähler werden separat aus dem Kopfbereich gelesen und anhand Gesamtzahl der Schüsse und Ganzring-Gesamtergebnis plausibilisiert.
- Pfeilausschnitte werden positionsbezogen je Serie extrahiert.
- Trefferbilder werden nicht gespeichert oder angezeigt.
- Foto wird weiterhin automatisch in ein A4-PDF umgewandelt.
- Die PDF-Importfunktion und Duplikatprüfung bleiben erhalten.
- IndexedDB `shootbook-v1` bleibt unverändert.

## Hinweise
- OCR und PDF-Erstellung benötigen Internetverbindung (Tesseract.js und jsPDF via CDN).
- Erkennung hängt von Bildschärfe, Beleuchtung, Perspektive und vollständiger Sichtbarkeit des Blatts ab.
- Fehlende Einzelschüsse oder unsichere Werte werden in der Importvorschau markiert.
- Die OCR-Bereichsaufteilung ist auf das Meyton-LG-60-ZR-Layout abgestimmt.
- Kein praktischer iPhone-Test durchgeführt.
