# Schießbuch – Version 1.2.6

- Durchschnittskachel zeigt nur Durchschnitt und Anzahl der Einheiten.
- Diagrammpunkte sind antippbar; der ausgewählte Punkt zeigt Datum/Serie und Messwert.
- PDF-Import prüft auf wahrscheinliche Duplikate (Kategorie, Disziplin, Zeitfenster 2 Minuten, Ergebnis und Serien). Bei Treffer erscheint eine Warnung; Import kann trotzdem bestätigt werden.
- CSV-Export aller gespeicherten Ergebnisse.
- Ergebnisliste und Dashboard können nach Datum (von/bis) und Disziplin gefiltert werden; Wettkampf und Training bleiben getrennt.
- Ergebnisbearbeitung in der Detailansicht: Kategorie, Disziplin, Datum, Ergebnis, ganze Ringe, Innenzehner, Serien, Serien-Ringzahlen, Zähler und kleinsten Teiler.
- Backup-Erinnerung erscheint, wenn noch nie ein Backup erstellt wurde oder das letzte Backup mindestens 14 Tage zurückliegt. Sie ist eine In-App-Erinnerung, keine iOS-Push-Mitteilung.
- QR-Code-Import ist nicht enthalten und bleibt zurückgestellt.
- Bestehende IndexedDB `shootbook-v1` bleibt erhalten. Keine automatische iCloud-Synchronisierung.
- CSV-Export umfasst alle gespeicherten Ergebnisse, unabhängig von den aktiven Listenfiltern.
