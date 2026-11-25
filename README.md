# Mein Schießbuch v1.3.11

## Änderungen
- Foto-OCR der Serien wurde korrigiert: Es werden nur die beiden gedruckten Schusszeilen innerhalb jedes Serienblocks berücksichtigt.
- Serienüberschrift und Trefferkreis-/Teiler-Metadaten werden nicht mehr als Einzelschüsse fehlinterpretiert.
- Schusswerte werden zeilenweise nach ihrer horizontalen Position sortiert: zuerst fünf Werte links nach rechts, danach die zweite Zeile links nach rechts.
- Die sechs Dezimal-Serienwerte stammen vorrangig aus der oberen Zeile „Serien:“; die Überschriften der Einzelblöcke werden nicht mehr als beliebige Zahlenmuster gesucht.
- Zehntel- und Ganzringsummen der zehn Einzelschüsse werden mit den Serienreferenzen verglichen.
- Fotoimport bleibt ohne Pfeilerkennung; PDF-Import behält die Pfeilextraktion.
- Duplikatprüfung bleibt erhalten.
- IndexedDB `shootbook-v1` bleibt unverändert.

## Validierung mit dem bereitgestellten Meyton-Foto
Die Serienbereiche wurden lokal mit Tesseract 5.5.0 ausgewertet. Erkannte Schüsse je Serie ergaben:
- Serie 1: 99,8 (96)
- Serie 2: 103,5 (99)
- Serie 3: 100,0 (97)
- Serie 4: 102,4 (97)
- Serie 5: 101,6 (98)
- Serie 6: 99,1 (95)
- Gesamt: 606,4 (582)

Diese lokale Prüfung verwendet Tesseract 5.5.0 unter Python und ist kein Test der Tesseract.js-Ausführung im iPhone-Browser. Die Browser-OCR und das iPhone-Layout müssen weiterhin auf dem Gerät überprüft werden.

## Technische Prüfungen
- JavaScript-Syntax mit Node.js geprüft.
- ZIP-Integrität geprüft.
- Versionsnummer, Service-Worker-Cache und Datenbankname geprüft.
