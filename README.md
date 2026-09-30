# WebsiteRenting0511-

## Einweisungsvideo für Mietkunden

Im Ordner `einweisungsvideo/` liegt eine animierte Kunden-Einweisung als Cartoon:
zwei Figuren (Mitarbeiterin und Kunde) besprechen in 13 Szenen den Ablauf der Miete,
die Regeln und Gebühren (Rauchverbot, Driftverbot, Zusatzkilometer, Verschmutzung,
Schäden) sowie das richtige Verhalten bei Unfall, Panne und Rückgabe. Der Text wird
von der deutschen Sprachausgabe des Browsers vorgelesen und als Untertitel angezeigt.

### Auf dem Fernseher abspielen

1. Ordner `einweisungsvideo/` auf einen USB-Stick kopieren oder auf einem Laptop öffnen.
2. `index.html` im Browser öffnen (Chrome oder Edge haben die besten deutschen Stimmen).
   Auf einem Smart-TV mit Browser, Fire-TV-Stick (Silk-Browser) oder Chromecast funktioniert
   es ebenfalls; Laptop per HDMI ist die zuverlässigste Variante.
3. Mit **F** oder dem Knopf „Vollbild“ in den Vollbildmodus wechseln, dann „Video starten“.
4. Für den Schaufensterbetrieb „Endlosschleife“ anhaken.

Bedienung: Leertaste = Pause/Weiter, Pfeiltasten = Szene vor/zurück, R = Neustart,
M = Ton aus/an, F = Vollbild. Die meisten TV-Fernbedienungen senden dieselben Tasten.

### Texte und Gebühren ändern

Alle Beträge, der Firmenname, die Notfallnummer und die Namen der Figuren stehen am Anfang
des `<script>`-Blocks in `index.html` im Objekt `CONFIG`. Die Dialoge stehen darunter in
`SCENES`; jede Szene hat einen Titel, eine Illustration und die Sprechblasen.

### Richtiges Video mit Runway

`einweisungsvideo/runway-prompts.md` enthält für jede Szene einen fertigen Prompt für
Runway (Gen-4). Die erzeugten MP4-Clips in `einweisungsvideo/clips/` ablegen und bei der
Szene `video: "clips/…mp4"` eintragen; der Clip läuft dann als Hintergrund hinter den
Figuren. Eine eingesprochene Tonspur (z. B. ElevenLabs oder Canva KI-Stimme) wird per
`audio: "clips/…mp3"` eingebunden.
