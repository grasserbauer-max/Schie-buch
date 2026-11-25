# Mein Schießbuch v1.3.5

## Änderungen
- Fotoimport bleibt der primäre neue Weg: Foto aus Mediathek wählen oder mit der iPhone-Kamera aufnehmen.
- Das Foto wird automatisch in ein A4-PDF umgewandelt; PDF kann aus der Vorschau gespeichert werden.
- OCR liest die Seite weiterhin für Kopf- und Ergebnisdaten.
- Bei LG 60 ZR werden die sechs Serienbereiche zusätzlich separat erkannt, um die zehn Einzelschüsse pro Serie zuverlässiger zu erfassen.
- Zähler werden separat aus dem oberen Ergebnisbereich gelesen und anhand der Schussanzahl und Summe der Ganzringe plausibilisiert.
- Schusspfeile werden als kleine Bildausschnitte neben den erkannten Schusswerten extrahiert und positionsbezogen je Serie gespeichert.
- Trefferbilder/Zielscheiben werden nicht gespeichert oder angezeigt.
- Die vorhandene PDF-Importmöglichkeit und Duplikatprüfung bleiben erhalten.
- IndexedDB-Datenbank `shootbook-v1` bleibt unverändert.

## Hinweise
- OCR und PDF-Erstellung benötigen beim Import eine Internetverbindung (Tesseract.js und jsPDF via CDN).
- Die OCR-Qualität hängt von Schärfe, Auflösung, Beleuchtung und Perspektive des Fotos ab.
- Unvollständige oder unsichere Erkennungen müssen in der Vorschau kontrolliert werden.
- Die Serienbereich-Erkennung ist auf das Layout der Meyton-LG-60-ZR-Ergebnisblätter ausgerichtet. LG 40 ZR verwendet weiterhin den bisherigen OCR-Pfad.
- Ein realer iPhone-Test wurde nicht durchgeführt.
