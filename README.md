# Mein Schießbuch – Version 1.3.3

## Fehlerbehebung
- OCR rendert gescannte PDF-Seiten mit höherer Auflösung (3×) und behält die Zeilenstruktur für die Serienauswertung bei.
- Gesamtergebnis-Erkennung toleriert OCR-typische Abweichungen bei Doppelpunkt, Zeilenumbrüchen und einzelnen Zeichen.
- OCR-Pfeilbereiche werden anhand der Position erkannter Schusswerte aus dem Scanbild ausgeschnitten; Zuordnung erfolgt nur bei passender Anzahl erkannter Schüsse.
- Digitale PDF-Texterkennung und bisherige Detailansicht bleiben erhalten.
- Duplikatprüfung bleibt aktiv (SHA-256 und Vergleich erkannter Ergebnisdaten).
- IndexedDB bleibt unverändert `shootbook-v1`.

## Grenzen / Teststatus
- JavaScript-Syntax und Archivstruktur werden geprüft. Ein vollständiger OCR-/Pfeiltest auf einem echten iPhone wurde nicht durchgeführt.
- OCR kann bei schiefen, unscharfen oder kontrastarmen Scans einzelne Ziffern verwechseln. Vorschau deshalb vor dem Speichern kontrollieren.
- Pfeile aus Scans werden als Bildausschnitte neben den erkannten Schusswerten gespeichert; ob jedes Symbol exakt getroffen wird, muss mit dem konkreten Gerät/Scan kontrolliert werden.
- PDF.js und Tesseract.js werden beim Import über CDN geladen; Internetverbindung erforderlich.

## Installation
Alle Dateien aus dem ZIP auf GitHub Pages hochladen und die bisherigen Dateien ersetzen. Datenbank `shootbook-v1` nicht löschen oder umbenennen.
