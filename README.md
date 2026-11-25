# Mein Schießbuch v1.3.7

## Änderungen
- Fotoimport: keine Pfeilerkennung, keine Pfeilausschnitte und keine Pfeilspeicherung.
- PDF-Import: bestehende Extraktion der Schusspfeile aus dem Original-PDF bleibt erhalten.
- Foto-OCR: Serienwerte können zusätzlich aus der Kopfzeile „Serien:“ gelesen werden, falls die einzelnen Serienüberschriften nicht zuverlässig erkannt werden.
- Die Ganzringwerte der Serien werden aus jeweils zehn vollständig erkannten Einzelschüssen abgeleitet.
- Zähler werden separat ausgewertet und anhand der Schussanzahl sowie des Ganzring-Gesamtergebnisses plausibilisiert.
- Foto wird weiterhin automatisch in ein A4-PDF umgewandelt.
- Duplikatprüfung bleibt für beide Importwege erhalten.
- Trefferbilder werden nicht gespeichert oder angezeigt.
- IndexedDB-Datenbank `shootbook-v1` bleibt unverändert.

## Hinweise
- OCR und PDF-Erstellung benötigen beim Import eine Internetverbindung.
- Foto-OCR hängt von Schärfe, Beleuchtung, Perspektive und vollständiger Sichtbarkeit des Dokuments ab.
- Nicht vollständig erkannte Serien und Zähler müssen in der Importvorschau kontrolliert werden.
- Der PDF-Pfeilimport nutzt weiterhin die bestehende Extraktion aus dem Original-PDF.
- Kein praktischer iPhone-Test für diese Version durchgeführt.
