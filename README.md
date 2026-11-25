# Schießbuch – Version 1.2.9

Änderungen gegenüber 1.2.8:
- PDF-Import rendert die Meyton-PDF-Seite und extrahiert die kleinen Richtungspfeile als transparente Bildausschnitte direkt aus dem PDF.
- Die Pfeile werden in der Detailansicht neben dem jeweiligen Einzelschuss angezeigt.
- Es werden keine Pfeile berechnet oder aus Ringzahlen abgeleitet. Wenn im PDF an der Schussposition kein Pfeil erkannt wird, bleibt die Stelle leer.
- Die Pfeilform und -richtung stammen aus dem PDF; die Farbe wird für die Lesbarkeit auf dem dunklen App-Design invertiert.
- Im Importdialog wird angezeigt, wie viele Pfeile erkannt wurden.
- Bereits gespeicherte, doppelte Ergebnisse können durch erneuten PDF-Import um die Pfeilbilder ergänzt werden, ohne einen zweiten Eintrag anzulegen.
- Neue Pfeildaten werden im bestehenden IndexedDB-Datensatz gespeichert und sind im JSON-Backup enthalten.
- Bestehende Datenbank `shootbook-v1` bleibt unverändert.
- QR-Code-Import weiterhin zurückgestellt.

Hinweis zur Aktualisierung bestehender Einträge:
Bereits gespeicherte Ergebnisse enthalten noch keine Pfeilbilder. Nach dem App-Update das jeweilige Original-PDF erneut importieren. Erkennt die App denselben Wettkampf/dasselbe Training wieder, ergänzt sie den vorhandenen Eintrag um die Pfeile, statt einen zweiten Eintrag anzulegen.
