# Spielplan

- Erst Teams anlegen (`team_speichern`), dann planen. `spielplan_lesen` zeigt Runden, Platzhalter („Team 1“ …), zugewiesene Teams und Spiele; `bearbeitbar` ist false, sobald im Turnier ein Spiel begonnen hat.
- `runde_anlegen` mit `vorschau=true` rechnet nur. Parameter: Modus `Gruppe` (mit `anzahlGruppen`, optional `rueckrunde`) oder `KO`, `anzahlTeams`, `spielzeit` und `pause` in Minuten, `beginn` (Datum, Uhrzeit), `spielfelder` (Anzahl oder Namen), `verteilung` (abwechselnd, spieltage, gruppen), Pausen und optional `teams` (Team-IDs in Reihenfolge der Platzhalter).
- Grobe Faustregel für die Dauer: Spiele × (Spielzeit + Pause) ÷ Spielfelder.
- `runde_aendern` mit Operationen: `zeiten`, `pausen`, `spielfelder`, `teams_zuweisen`, `verschieben`, `heimrecht_tauschen`, `spiel_entfernen`, `neu_planen`, `umbenennen`.
- K.-o.-Runden mit Verknüpfungen zu Gruppenplätzen („1. Gruppe A“) richtet der Nutzer in der App ein; über diese Verbindung entstehen Platzhalter, denen Teams zugewiesen werden.
- Ligamodus: `spieltag_speichern` mit Datum, Startzeit und Spielen (Teams, Heimteam).
- Ergebnisse, Spieluhr und Anzeigetafel sind über diese Verbindung nie änderbar.
