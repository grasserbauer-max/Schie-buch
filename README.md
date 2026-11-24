# Mein Schießbuch – iPhone-PWA v1.2.0

- Einstellungsmenü: Name, Akzentfarbe, Aktivierung von LG 40 ZR-Wettkämpfen.
- Titel zeigt „[Name]s Schießbuch“; bisherige LG-60-/Training-Unterzeile entfernt.
- LG-40-ZR-PDFs werden standardmäßig blockiert, bis die Disziplin in den Einstellungen aktiviert ist.
- Serienanzahl wird aus der PDF ermittelt; der Parser verarbeitet alle erkannten Serien und erwartet je Serie zehn Schüsse.
- Bereits gespeicherte Ergebnisse bleiben in IndexedDB erhalten.

Wichtiger Hinweis zu den Schusspfeilen:
Die Meyton-PDF enthält die kleinen Pfeile als grafische Vektorelemente. Die aktuelle PDF-Textauswertung kann diese nicht zuverlässig auslesen. Die Detailansicht zeigt Pfeile nur, wenn ein Ergebnis entsprechende shotDirections-Daten enthält. Eine automatische Extraktion dieser Grafikpfeile ist noch nicht implementiert; es werden keine Richtungen erfunden.
