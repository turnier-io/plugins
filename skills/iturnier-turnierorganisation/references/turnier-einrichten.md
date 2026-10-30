# Turnier einrichten

1. `konto_kontext`: Tarif, Grenzen (aktive Turniere, Teams pro Turnier) und Vereine. Für ein Vereinsturnier die `vereinsId` des Vereins verwenden (nur als Vereinsadmin).
2. `turnier_anlegen` mit Name, Art (Hallenturnier, Großfeldturnier, Kleinfeldturnier, Kinderfussball), Altersklasse, Tagen (`zeitraum`: Datum, Start- und Endzeit) und Spielstätten. Ein Link-Name (`alias`, 4–64 Zeichen) macht die Turnierseite unter turnier.io/<alias> erreichbar.
3. Vereinsstandards (Spielzeiten, Design, Sponsoren) übernimmt turnier.io beim Anlegen automatisch.
4. `ansprechpartner_setzen` für Kontaktpersonen auf der Turnierseite; `oeffentlich` steuert, welche Angaben sichtbar sind. Die Angaben sind danach nur noch als Anzahl sichtbar.
5. `turnier_aktualisieren` ändert Stammdaten, Tage, Spielstätten, Status (Planung → Vorbereitung → Durchführung → Abgeschlossen) und den Spielbetrieb (Countdown, Sirene, Tormusik, Netto-Spielzeit, Teamfouls).
6. `aufgaben_auflisten` zeigt Vorschläge je Phase; mit `aufgabe_speichern` übernehmen (vorlageId), Fälligkeit und Erinnerung setzen.

Abgeschlossene Turniere lassen sich mit `turnier_archivieren` archivieren; archivierte Turniere sind schreibgeschützt.
