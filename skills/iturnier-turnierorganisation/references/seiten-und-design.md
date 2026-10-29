# Turnier- und Vereinsseite

- `turnierseite_gestalten`: Beschreibung und Design. Layouts: stadion, tribuene, klar, panorama, sanft, anpfiff, flutlicht, morgenlicht (ab Pro). Feinanpassung im Feld `experte` je Gerät (`beide`, `mobile`, `desktop`): Farben `primary`, `secondary`, `background`, `surface`, `text`, `muted`, `heading`, `border` (Hex), Schriften `font`/`headingFont`, Größen `fontSize` (12–24), `headingSize` (20–72), `smallSize` (10–20).
- Für gut lesbare Farben: Text auf Hintergrund mit mindestens 4,5:1 Kontrast; Vereinsfarben eignen sich als `primary`/`secondary`.
- Vereinsseite (Tarif Verein): `vereinsseite_entwurf_lesen` liefert Entwurf und `version`. `vereinsseite_entwurf_speichern` führt Änderungen zusammen (Listen wie Sponsoren und Infoseiten werden ersetzt). `vereinsseite_veroeffentlichen` mit `version`, `liveVersion` und `aktiv`.
- Infoseiten bestehen aus Blöcken (`ueberschrift`, `text`, `bild`, `link`); Bilder als https-Adresse.
