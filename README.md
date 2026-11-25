# Schießbuch – Version 1.3.0

Neue Funktion: Dokumentenscanner im PDF-Import-Bereich.

- Zusätzlicher Button „Dokument scannen“ neben „PDF importieren“.
- iPhone-Kamera wird über den nativen Datei-/Kamera-Dialog aufgerufen.
- Unterstützt eine oder zwei aufgenommene Seiten.
- Seitenvorschau und Entfernen einer aufgenommenen Seite.
- Kamerabilder werden auf maximal 2400 Pixel Kantenlänge normalisiert und als PDF im A4-Format zusammengefügt.
- OCR über Tesseract.js (Deutsch und Englisch) liest den Scantext aus.
- Erkannte Werte werden über den vorhandenen Ergebnisparser verarbeitet und vor dem Speichern angezeigt.
- Das erzeugte PDF kann separat heruntergeladen werden; nach dem Speichern wird zusätzlich gefragt, ob das PDF gespeichert werden soll.
- Scans werden nicht automatisch als Datei in IndexedDB abgelegt. Ergebnisdaten werden wie bisher in `shootbook-v1` gespeichert.
- QR-Code-Import bleibt zurückgestellt.

Einschränkungen:
- OCR funktioniert nur bei ausreichend scharfen, gut beleuchteten und möglichst gerade aufgenommenen Dokumenten.
- Die Texterkennung ersetzt keine manuelle Kontrolle; bei unvollständigen Daten wird der Scan nicht stillschweigend als korrekt behandelt.
- Pfeilgrafiken werden beim Kamera-OCR nicht übernommen, da OCR keine originalen PDF-Vektorpfeile extrahiert.
- Der Scanner nutzt Kamera-/Dateiauswahl des iPhones. Browser und iOS können je nach Berechtigung die Auswahloberfläche unterschiedlich darstellen.
- Externe Bibliotheken (Tesseract.js und jsPDF) benötigen beim ersten Laden eine Internetverbindung.
