# Anleitung für die KI: Szenen tauschen mit Genjutsu

Gib diesen Text an Claude Code oder einen anderen Coding-Agenten, der auf deinem Rechner arbeiten darf. Schreib dazu: „Bau mit mir ein Video nach dieser Anleitung. Meine Szene: …“

---

Du baust mit mir ein Video, in dem Higgsfield Genjutsu meinen eigenen Dreh in eine andere Szene verwandelt. Übernimm das Prinzip, nicht das Beispiel: Figuren, Objekte, Ort und Texte entstehen für meine Idee neu. Arbeite in Phasen, zeig mir jedes Ergebnis und warte auf mein Go. Bevor etwas Geld oder Credits kostet, nennst du mir Modell, Anzahl und Kosten.

## Frag mich zuerst

1. Was soll aus welchem Gegenstand werden und wo spielt die Szene?
2. Gibt es das Video schon? Länge, Format, in HDR aufgenommen?
3. Welche Objekte müssen aussehen wie ein echtes Vorbild (Auto, Produkt, Ort) und habe ich Fotos davon?
4. Für welche Plattform, mit Untertiteln?
5. Wie viele Credits darf es kosten?

## Prinzip

Die Bewegung ist echt, die KI tauscht nur, was ich festlege. Genjutsu im Modus Objects swap behält Gesicht, Stimme, Lippen und jede Bewegung. Es tauscht Personen, Gegenstände und auch den ganzen Ort. Modelle, die die Szene aus Referenzbildern neu erzeugen, taugen dafür nicht. Der Reiz entsteht, wenn man beides sieht: KI oben, echt unten, in derselben Sekunde.

## Ablauf

| Schritt | Was | Achte auf |
|---|---|---|
| 1 Dreh | Kamera fest, quer, die ganze Handlung im Bild. Platzhalter in Größe und Gewicht ähnlich wie das, was daraus werden soll. | Jede Aktion deutlich spielen, Würfe in eine klare Richtung. |
| 2 Umrechnen | iPhone-HDR zuerst nach SDR (HLG, Dolby Vision), mit dem Apple-Weg `avconvert`. Standbilder genauso ziehen. | Sonst werden Bilder flau, Hauttöne kippen und jede Referenz baut darauf auf. |
| 3 Referenzen | Outfit ohne Gesicht, jede neue Person, jedes Objekt, der leere Ort. Alle im Seitenverhältnis des Videos. | Feste Objekte als echtes Foto, Kennzeichen und Logos weg. Eine Referenz je Objekt. |
| 4 Prompt | Englisch, ein Block je Element, Gerüst siehe unten. | Jede Richtung, jeder Zeitpunkt, jedes sichtbare Kleidungsstück bis zu den Schuhen. |
| 5 Lauf | Objects swap über die ganze Länge in einem Lauf, 720p. Erst Kosten nennen, dann Go. | Bildmarken prüfen: „@image1“ plus Enter wählt zuerst „Video 1“. |
| 6 Prüfen | Bild für Bild gegen das Original, als Kontaktbogen und an jeder Aktion. | Richtung, Schuhe, Türen, Ausschnitt, erfundene Details. |

## Prompt-Gerüst

Nur die Struktur übernehmen, Inhalte in eckigen Klammern für meine Szene neu schreiben.

```
KEEP EXACTLY for the whole video: the man, his real face, hair and beard, his voice and lip movement, every movement, gesture and step, the camera position, framing and timing.
OUTFIT @Image1, whole video: [clothes], [shoes], [jewellery].
PERSON @Image2 replaces the [placeholder] for the whole video: [look]. [What she does]. At [x] s he throws her out of frame towards the [LEFT] edge.
OBJECT @Image3 replaces the [placeholder] for the whole video: [look, what happens to it].
PLACE @Image4 replaces the room for the whole video: [place, light, weather]. The [furniture] becomes [object @Image5] at the same position.
No [placeholder] appears at any moment. No text, no subtitles.
```

## Ton

Meine Stimme aus dem Original freistellen, dazu eine Atmo des neuen Ortes. Effekte nur auf Bildereignisse wie Wurf oder Geld, kurz und leise. Musik unter der Stimme, sie duckt beim Sprechen und setzt beim Wurf kurz aus. Am Ende −14 LUFS, Stereo prüfen. Je Runde nur die Änderung, die ich verlange; eigene Ideen als Variante daneben.

## Schnitt fürs Reel

9:16 auf Schwarz. Oben der Titel, darunter der KI-Clip randlos, dann ein schmales Band mit Untertiteln, darunter das Original, unten der Aufruf. Der ganze Block sitzt mittig.

## Genjutsu-Wege und Preise, Stand 31.10.2026

In der Higgsfield-Oberfläche 29,5 s in 720p 210 Credits. Higgsfield-Abo per Kommandozeile: 15 s in 720p 105 Credits. Genjutsu Lite: 2 Credits je Sekunde. API: 0,318 $ je Sekunde in 480p, 0,681 $ in 720p (Listenpreis); das Eingangsvideo wird auf volle Sekunden aufgerundet, ein Auftrag wird erst angenommen und scheitert danach, wenn das Guthaben fehlt.
