# Teams und Kader

- `team_speichern` ohne `teamId` legt ein Team an, mit `teamId` wird es geändert (nur angegebene Felder).
- Kader: `kader` mit `modus` (`ersetzen`, `ergaenzen`, `entfernen`) und `spieler` (Vorname, Nachname, Trikotnummer). Trainer: `trainer` mit `personen` (Vorname, Nachname, Mobilnummer, E-Mail, WhatsApp).
- Spieler und Trainer sind nach dem Speichern nur als Anzahl sichtbar (`teams_auflisten`). Zum Korrigieren gleiche Namen mit `ergaenzen` erneut senden oder mit `entfernen` löschen.
- Logos und Sponsorenbilder als https-Adresse eines Bildes.
- Das Teamlimit hängt vom Tarif ab (`konto_kontext`).
- `team_loeschen` ist nicht möglich, solange das Team im Spielplan oder an einem Spieltag eingeplant ist.
