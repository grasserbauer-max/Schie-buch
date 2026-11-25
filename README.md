# Mein Schießbuch v1.3.9

## Änderungen
- Fotoimport verarbeitet die sechs Serienbereiche getrennt.
- Die zehn Schusswerte je Serie werden anhand ihrer OCR-Bildkoordinaten erkannt und geometrisch in zwei Zeilen gruppiert.
- Innerhalb jeder Zeile gilt die feste Reihenfolge von links nach rechts: Schüsse 1–5, danach Schüsse 6–10.
- Die Serienüberschrift wird separat aus dem jeweiligen Serienbereich gelesen.
- Die obere Kopfzeile mit den sechs Serienwerten wird nicht als zweite Quelle für zusätzliche Serien verwendet.
- Die Summe der zehn Schüsse wird mit dem separat erkannten Serienwert in Zehntelringen und ganzen Ringen verglichen.
- Abweichungen und unvollständige Reihen werden in der Vorschau markiert.
- Fotoimport bleibt ohne Pfeilerkennung. PDF-Import extrahiert weiterhin Pfeile aus dem Original-PDF.
- Trefferbilder werden nicht gespeichert oder angezeigt.
- Duplikatprüfung bleibt erhalten.
- IndexedDB-Datenbank `shootbook-v1` bleibt unverändert.

## Hinweise
- OCR und PDF-Erstellung benötigen beim Fotoimport eine Internetverbindung.
- Die Erkennung basiert auf dem Meyton-LG-60-ZR-Seitenlayout und den Bildkoordinaten. Perspektive, Drehung, Zuschnitt, Licht und Unschärfe können die Positionszuordnung beeinflussen.
- Ein iPhone-Feldtest wurde nicht durchgeführt. Die tatsächliche Erkennung muss auf dem Gerät mit einem scharfen, vollständig sichtbaren Foto geprüft werden.
