# Mein Schießbuch v1.3.14

## Änderungen
- Fotoimport vollständig entfernt: kein Foto-Button, kein Foto-Importhandler und keine Foto-zu-PDF-Konvertierung mehr.
- PDF importieren ist die einzige Importmöglichkeit und bleibt links als primärer Importbutton.
- PDF-Import erkennt weiterhin PDFs mit Textebene und gescannte Bild-PDFs ohne Textebene.
- OCR für Bild-PDFs überarbeitet: adaptive Renderauflösung mit begrenzter maximaler Bildkante, um Speicherprobleme auf dem iPhone zu reduzieren.
- OCR-Bildvorverarbeitung verbessert den Kontrast von grauem Papier, ohne kleine Dezimalpunkte durch harte Binarisierung zu entfernen.
- Zweiter OCR-Durchlauf mit alternativer Seitensegmentierung, wenn die erste Erkennung zu wenig Text liefert.
- Bestehender PDF-Parser, Duplikatprüfung und Pfeilextraktion bleiben erhalten.
- IndexedDB `shootbook-v1` bleibt unverändert.
- Versionsanzeige und Service-Worker-Cache auf 1.3.14 aktualisiert.

## Hinweis zum iPhone-Scan
Das bereitgestellte iPhone-PDF ist ein Bild-PDF ohne Textschicht. Es wird daher über PDF.js gerendert und lokal mit Tesseract.js OCR verarbeitet. Die neue OCR-Verarbeitung wurde syntaktisch geprüft, aber noch nicht auf einem echten iPhone ausgeführt. Die Erkennungsqualität muss nach dem Upload mit dem bereitgestellten Scan kontrolliert werden.
