# Runway-Prompts für das Einweisungsvideo

Diese Prompts erzeugen in Runway (Gen-4 / Gen-4 Turbo, Text-zu-Video oder Bild-zu-Video)
je einen 5- bis 10-Sekunden-Clip pro Szene. Die Clips werden als MP4 in den Ordner
`einweisungsvideo/clips/` gelegt und in `index.html` bei der jeweiligen Szene unter
`video: "clips/03-tank-kilometer.mp4"` eingetragen. Der Clip läuft dann stumm als
Hintergrund, während die Cartoon-Figuren den Dialog sprechen.

Für einen einheitlichen Look immer denselben Stil-Vorspann verwenden:

> **Stil-Vorspann:** 2D flat cartoon explainer style, thick clean outlines, bright friendly
> colours (signal orange #FF7A1A car, sky blue background), smooth simple animation,
> no text, no letters, no subtitles, 16:9, camera static.

| Nr | Szene | Prompt (nach dem Stil-Vorspann) | Dateiname |
|----|-------|----------------------------------|-----------|
| 01 | Willkommen | Friendly female rental agent in orange polo waves in front of a small car rental office, an orange compact car parked beside her, sunny day. | clips/01-willkommen.mp4 |
| 02 | Übergabe | Agent and customer walk around an orange car, agent holds a clipboard and takes photos of the car with a phone, checkmarks appear. | clips/02-uebergabe.mp4 |
| 03 | Tank und Kilometer | Close-up of a cartoon dashboard: fuel gauge needle moves to full, odometer digits tick upward, then a fuel pump nozzle fills the tank. | clips/03-tank-kilometer.mp4 |
| 04 | Rauchverbot | Inside the car a hand with a cigarette appears, a big red no-smoking sign pops up and pushes it away, window opens and smoke leaves. | clips/04-rauchverbot.mp4 |
| 05 | Driften verboten | Orange car drifting sideways on an empty lot leaving tyre marks, a large red prohibition circle slams over it, screen shakes briefly. | clips/05-driften.mp4 |
| 06 | Weitere Regeln | Split scene: a driver's licence with a green checkmark, a beer bottle with a red cross, a map with a border and a red stop hand. | clips/06-regeln.mp4 |
| 07 | Verschmutzung | Car interior with sand, mud, crumbs and a spilled coffee cup on the seats, then a cleaning brush and sparkle effect. | clips/07-verschmutzung.mp4 |
| 08 | Schäden | Shopping cart bumps the car door leaving a dent and scratch, a warning triangle icon appears, a phone camera takes a photo. | clips/08-schaeden.mp4 |
| 09 | Unfall | Two cartoon cars with a small fender bender, hazard lights blinking, driver in hi-vis vest places a warning triangle, police car arrives with blue lights. | clips/09-unfall.mp4 |
| 10 | Unfallprotokoll | Two drivers fill in a European accident report form on the car bonnet, one draws a sketch, a hand takes photos of number plates. | clips/10-unfallprotokoll.mp4 |
| 11 | Sofort melden | Customer holding a phone to the ear, big green ringing phone icon, rental agent answers at the office desk, day-and-night clock spins. | clips/11-melden.mp4 |
| 12 | Rückgabe | Orange car rolls back into the rental lot, clock on the wall shows the agreed time, agent and customer shake hands over the return form. | clips/12-rueckgabe.mp4 |
| 13 | Gute Fahrt | Orange car drives off along a sunny coastal road, agent waves goodbye from the office, sun shining. | clips/13-gute-fahrt.mp4 |

## Ton

Die Stimme kommt weiterhin aus der Sprachausgabe des Browsers. Für eine Studio-Stimme kann
der Dialog aus `index.html` (Feld `SCENES`) in ElevenLabs oder Canva „KI-Stimme generieren“
eingesprochen und als `clips/NN-*.mp3` abgelegt werden; das Feld `audio:` bei der Szene
spielt die Datei statt der Browserstimme ab.
