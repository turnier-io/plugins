# Einladungen

1. `einladung_uebersicht`: Listen, Empfänger, eingeladen, offen, letzter Versand.
2. `empfaengerlisten_auflisten`, bei Bedarf `empfaengerliste_speichern` (neue Liste) und `empfaenger_hinzufuegen` (E-Mail plus Name oder Verein). Empfänger sind danach nicht lesbar; `empfaenger_entfernen` arbeitet mit E-Mail-Adressen.
3. `einladung_vorbereiten` mit den Listen: liefert Anzahl, Teile, Tagesrest und einen Mustertext für den Beispielempfänger „Alex“. Diese Angaben dem Nutzer zeigen.
4. Erst nach ausdrücklicher Bestätigung: `einladung_senden` mit `serieId` und `bestaetigteAnzahl`. Bei `fortsetzen=true` später erneut aufrufen; Teile gehen nie doppelt raus.
5. `versand_status` zeigt die Zustellung in Zahlen.

Versand braucht den Tarif Pro, eine bestätigte Antwortadresse im Vereinsmodul und die eigene Freigabe „Mails versenden“ beim Verbinden des Assistenten. Das Tageslimit liegt bei 200 Mails.
