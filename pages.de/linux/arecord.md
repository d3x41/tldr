# arecord

> Sound Recorder für den ALSA-Soundkarten-Treiber.
> Weitere Informationen: <https://manned.org/arecord>.

- Nehme einen Schnipsel in CD-Qualität auf (beende die Aufnahme mit `<Ctrl c>`):

`arecord -vv --format=cd {{pfad/zu/datei.wav}}`

- Nehme einen Schnipsel in CD-Qualität auf mit einer festen Länge von 10 Sekunden:

`arecord -vv --format=cd --duration={{10}} {{pfad/zu/datei.wav}}`

- Nehme einen Schnipsel auf und speichere es als MP3 (beende die Aufnahme mit `<Ctrl c>`):

`arecord -vv --format=cd --file-type raw | lame -r - {{pfad/zu/datei.mp3}}`

- Liste alle Soundkarten und digitalen Ausgabe Geräte:

`arecord --list-devices`

- Benutze das interaktive Interface (z.B. `<Space>` oder `<Enter>` für Play oder Pause):

`arecord --interactive`
