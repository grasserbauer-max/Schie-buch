# Mein Schießbuch v1.3.4

## Änderungen
- Neuer Foto-Import über iPhone-Kamera oder Fotomediathek.
- Bild wird automatisch aufbereitet, per OCR ausgewertet und als A4-PDF erzeugt.
- Das erzeugte PDF kann aus der Importvorschau gespeichert werden; nach dem Speichern wird es ebenfalls angeboten.
- Die bestehende PDF-Importfunktion bleibt erhalten.
- Redundante Serien-Zusammenfassungszeile (Trefferkreis/Trefferlage/beste Teiler) aus der Detailansicht entfernt.
- Duplikatprüfung für Fotoimporte nutzt Datei-Hash und den Vergleich der Ergebnisdaten.
- IndexedDB-Datenbank `shootbook-v1` bleibt unverändert.

## Hinweise
- Für OCR und PDF-Erzeugung ist beim Import eine Internetverbindung erforderlich (Tesseract.js und jsPDF werden von CDNs geladen).
- Die Erkennung von Einzelschüssen und Pfeilen hängt von Bildqualität, Schärfe, Perspektive und Beleuchtung ab. Unvollständige Werte werden in der Vorschau angezeigt und müssen vor dem Speichern kontrolliert werden.
- Kein tatsächlicher iPhone-Feldtest wurde durchgeführt.
