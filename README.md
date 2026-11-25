# Mein Schießbuch v1.3.13

## Änderungen
- Fotoimport erstellt zuerst ein PDF aus dem ausgewählten Foto.
- Das erzeugte PDF wird anschließend durch denselben PDF-Extraktions- und Analysepfad wie ein normaler PDF-Import verarbeitet.
- Die direkte, separate Foto-OCR und deren abweichende Serien-Sonderlogik werden im Fotoimport nicht mehr verwendet.
- PDF-Bild wird als PNG eingebettet, um zusätzliche JPEG-Kompressionsverluste zu vermeiden.
- Duplikatprüfung bleibt aktiv; bei erneutem Import wird vor dem Speichern gewarnt.
- Originale Schusspfeile werden weiterhin nur aus normalen Meyton-PDFs übernommen.
- Datenbank `shootbook-v1` bleibt unverändert.
- Versionsanzeige und Service-Worker-Cache auf 1.3.13 aktualisiert.

## Einschränkungen
- Ein Foto-PDF enthält weiterhin nur Bilddaten. Die Werte werden daher über die OCR des normalen PDF-Imports erkannt.
- Die Bildqualität kann nicht besser werden als das Ausgangsfoto. Unschärfe, Reflexionen, Perspektivfehler oder abgeschnittene Ränder lassen sich durch die PDF-Konvertierung nicht vollständig beheben.
- Die Änderung wurde syntaktisch geprüft; ein vollständiger iPhone-Test mit realen Fotos wurde nicht durchgeführt.
