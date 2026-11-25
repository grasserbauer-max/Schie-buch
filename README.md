# Mein Schießbuch v1.3.10

## Änderungen
- Fotoimport erhält einen zusätzlichen, eigenständigen OCR-Durchlauf nur für die Ergebniszeile.
- Der Ergebnisbereich wird als eigener, hochskalierter Bildausschnitt verarbeitet und mit mehreren Tesseract-Seitenmodi gelesen.
- Ein erkannter Wert wird nur bei passendem Zahlenformat und plausiblen Wertebereichen als kanonische Zeile `Ergebnis: x (y)` an den bestehenden Parser übergeben.
- Die bisherige Kopfbereichs-OCR bleibt als zusätzlicher Erkennungsweg bestehen.
- Bei weiterhin fehlendem Gesamtergebnis wird der OCR-Text des Ergebnisbereichs in der Fehlermeldung zur Diagnose ausgegeben.
- Die positionsbasierte Erkennung der sechs Serienbereiche aus Version 1.3.9 bleibt erhalten.
- Fotoimport ohne Pfeilerkennung; Pfeile weiterhin ausschließlich beim Original-PDF-Import.
- Duplikatprüfung bleibt erhalten.
- Trefferbilder werden nicht gespeichert oder angezeigt.
- IndexedDB `shootbook-v1` bleibt unverändert.

## Prüfungen
- JavaScript-Syntaxprüfung mit Node.js.
- ZIP-Integritätsprüfung.
- Versionsnummer, Service-Worker-Cache und Datenbankname geprüft.

## Grenzen
- Die Ergebniszeile wird anhand eines festen Bildbereichs im Meyton-Seitenlayout ausgeschnitten. Stark abweichende Zuschnitte, Drehungen oder Perspektiven können den Bereich verfehlen.
- Es wurde kein realer iPhone-Kameratest durchgeführt. Die OCR-Erkennung muss auf dem Gerät mit dem tatsächlichen Foto überprüft werden.
