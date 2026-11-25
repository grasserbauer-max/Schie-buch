# Mein Schießbuch v1.3.8

## Änderungen
- Fotoimport: Jede Serie wird anhand ihrer zehn Einzelschüsse geprüft.
- Die zehn Dezimal-Schusswerte einer Serie werden addiert und mit dem unabhängig erkannten Serienwert verglichen, sofern dieser in der Serienüberschrift lesbar ist.
- Zusätzlich wird die Ganzring-Summe der zehn Schüsse mit dem erkannten Ganzring-Serienwert verglichen.
- Wenn die Serienüberschrift nicht zuverlässig erkannt wird, wird die Summe der Einzelschüsse als Serienwert verwendet und ausdrücklich als nicht unabhängig geprüft markiert.
- Die Summe aller 60 Einzelschüsse wird mit dem Gesamtergebnis in Zehntelringen und ganzen Ringen verglichen.
- Die Importvorschau zeigt die Prüfergebnisse für jede Serie und das Gesamtergebnis.
- Fotoimport erkennt oder speichert keine Pfeile.
- PDF-Import extrahiert weiterhin die Schusspfeile aus dem Original-PDF.
- Duplikatprüfung bleibt erhalten.
- Trefferbilder werden nicht gespeichert oder angezeigt.
- IndexedDB `shootbook-v1` bleibt unverändert.

## Hinweise
- OCR und PDF-Erstellung benötigen beim Import eine Internetverbindung.
- Die Plausibilitätsprüfung erkennt Abweichungen, garantiert aber nicht, dass jeder OCR-Wert richtig gelesen wurde.
- Nicht unabhängig erkannte Serienwerte werden in der Vorschau entsprechend gekennzeichnet.
- Kein praktischer iPhone-Test wurde durchgeführt.
