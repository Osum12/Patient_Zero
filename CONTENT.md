# Patient Zero — Placeholder Asset List

The game has 1 investigations. Every interview shows a portrait placeholder (the character's
initials) and an audio placeholder strip. To use your own files, put them in folders next to
`index.html` and add the paths to that character's entry in the case's `interviews` object:

```js
sam: {
  audio: "audio/okafor/sam.mp3",
  portrait: "img/okafor/sam.jpg",
  lines: [ ... ]
}
```

Each case's gatekeeper (the relative who refuses to talk until the inheritance pattern is solved) has
two clips: `audio` for the refusal and `audioDeep` for the full interview afterwards.

If a path is set, the game shows an `<audio controls>` player and an `<img>` instead of the placeholder;
leave it out to keep the placeholder. Paths are relative, so everything works from `file://` and on
GitHub Pages.

**Totals:** 16 audio clips and 15 portraits across 1 cases. Every case
works fine with placeholders, so you can add assets one case at a time.

## Recommended specs

| Asset | Format | Spec |
|---|---|---|
| Interview audio | MP3 (or M4A/OGG) | Mono, 44.1 kHz, 96–128 kbps, about 20–30 s each, under 500 KB |
| Portraits | JPG or WebP | Square 512 × 512 px (shown cropped to a circle, so keep the face centered), under 150 KB |

Read each character's interview lines from the game; stage directions (italic) aren't read aloud.
Lengths below are estimates from the word count at a natural speaking pace.

Suggested folders:

```
patient_zero/
├── index.html
├── audio/<case>/<character>.mp3
└── img/<case>/<character>.jpg
```

Portraits can be illustrations, student artwork or photos. These families are fictional, so don't use
photos of real people unless you have their consent.

## Case 0031-K — Okafor family · Keller Syndrome

*autosomal recessive* · 15 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Sam Okafor (28) | The proband · newly diagnosed | `audio/okafor/sam.mp3` | ~40 s | `img/okafor/sam.jpg` |
| Kelechi Okafor (38) | Sam's cousin · affected since age 15 | `audio/okafor/kelechi.mp3` | ~30 s | `img/okafor/kelechi.jpg` |
| Chidi Okafor (67) | Emeka's eldest son · Kelechi's father | `audio/okafor/chidi.mp3` | ~25 s | `img/okafor/chidi.jpg` |
| Folake Okafor (64) | Chidi's wife (married in) | `audio/okafor/folake.mp3` | ~30 s | `img/okafor/folake.jpg` |
| Obi Okafor (61) | Emeka's younger son · Sam's father | `audio/okafor/obi.mp3` | ~30 s | `img/okafor/obi.jpg` |
| Yemi Okafor (57) | Obi's wife (married in) | `audio/okafor/yemi.mp3` | ~35 s | `img/okafor/yemi.jpg` |
| Ngozi Bell (64) | Emeka's daughter | `audio/okafor/ngozi.mp3` (refusal, ~20 s)<br>`audio/okafor/ngozi_deep.mp3` (after the pattern) | ~45 s | `img/okafor/ngozi.jpg` |
| Daniel Bell (66) | Ngozi's husband (married in) | `audio/okafor/daniel.mp3` | ~25 s | `img/okafor/daniel.jpg` |
| Zara Bell (24) | Ngozi's daughter · medical student | `audio/okafor/zara.mp3` | ~35 s | `img/okafor/zara.jpg` |
| Emeka Bell Jr. (21) | Ngozi's son · named for his grandfather | `audio/okafor/emekajr.mp3` | ~25 s | `img/okafor/emekajr.jpg` |
| Adanna Reyes (35) | Kelechi's sister | `audio/okafor/adanna.mp3` | ~25 s | `img/okafor/adanna.jpg` |
| Tobi Okafor (31) | Kelechi's brother | `audio/okafor/tobi.mp3` | ~20 s | `img/okafor/tobi.jpg` |
| Chiamaka Okafor (31) | Sam's sister | `audio/okafor/chiamaka.mp3` | ~25 s | `img/okafor/chiamaka.jpg` |
| Dara Okafor (37) | Kelechi's wife (married in) | `audio/okafor/dara.mp3` | ~25 s | `img/okafor/dara.jpg` |
| Marcus Reyes (36) | Adanna's husband (married in) | `audio/okafor/marcus.mp3` | ~25 s | `img/okafor/marcus.jpg` |

No portrait needed: Emeka (deceased), Adaeze (deceased), Nia (minor), Lola (minor).
