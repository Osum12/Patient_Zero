# Patient Zero — Placeholder Asset List

Every interview in `index.html` shows a portrait placeholder (the character's initials) and an audio
placeholder strip. To use your own files, put them next to `index.html` and set the paths in the
`INTERVIEWS` object near the top of the file:

```js
sam: {
  audio: "audio/sam.mp3",
  portrait: "img/sam.jpg",
  lines: [ ... ]
}
```

If a path is set, the game shows an `<audio controls>` player and an `<img>` instead of the placeholder.
Leave it as `null` to keep the placeholder. Paths are relative, so it all works from `file://` as long as
the folders sit next to `index.html`.

## Recommended specs

| Asset | Format | Spec |
|---|---|---|
| Interview audio | MP3 (or M4A/OGG) | Mono, 44.1 kHz, 96–128 kbps, about 20–30 s each, under 500 KB |
| Portraits | JPG or WebP | Square 512 × 512 px (shown at 56 px, cropped to a circle, so keep the face centered), under 150 KB |

Suggested folders:

```
patient_zero/
├── index.html
├── audio/   ← 15 clips
└── img/     ← 15 portraits
```

## Interview audio clips (15)

Each clip should be the character reading their interview lines (shown in the game) in their own voice.
Stage directions (italic text) are not read aloud.

| # | Character | File | Length | Voice / delivery notes |
|---|---|---|---|---|
| 1 | Sam Okafor (28) — proband | `audio/sam.mp3` | ~25 s | Nervous, wry humor covering fear. Introduces the word "proband." |
| 2 | Kelechi Okafor (38) — affected cousin | `audio/kelechi.mp3` | ~25 s | Steady, tired, matter-of-fact. Has lived with this for 23 years. |
| 3 | Chidi Okafor (67) — Kelechi's father | `audio/chidi.mp3` | ~20 s | Slow and precise, a retired engineer. Healthy parents, affected child. |
| 4 | Folake Okafor (64) — Chidi's wife | `audio/folake.mp3` | ~25 s | Warm but defensive. Mentions the "weak blood" rumor (red herring). |
| 5 | Obi Okafor (61) — Sam's father | `audio/obi.mp3` | ~25 s | Talkative, hospitable, anxious underneath. "Two branches, same tree." |
| 6 | Yemi Okafor (57) — Obi's wife | `audio/yemi.mp3` | ~25 s | Pharmacist, crisp and factual. She and Folake are unrelated. |
| 7a | Ngozi Bell (64) — refusal | `audio/ngozi.mp3` | ~15 s | Guarded and protective. Refuses until the pattern is known. |
| 7b | Ngozi Bell — after the pattern is solved | `audio/ngozi_deep.mp3` | ~30 s | Softer and reflective. Reveals Emeka's brother and Adaeze's sister. |
| 8 | Daniel Bell (66) — Ngozi's husband | `audio/daniel.mp3` | ~20 s | Genial, teasing in-law. Points to Emeka's locked trunk. |
| 9 | Zara Bell (24) — medical student | `audio/zara.mp3` | ~30 s | Bright, quick, a little nerdy. The recessive-inheritance tutorial. |
| 10 | Emeka Bell Jr. (21) — named for grandpa | `audio/emekajr.mp3` | ~20 s | Gentle, nostalgic. Remembers the unsent letters. |
| 11 | Adanna Reyes (35) — Kelechi's sister | `audio/adanna.mp3` | ~20 s | Worried mother, thoughtful. |
| 12 | Tobi Okafor (31) — Kelechi's brother | `audio/tobi.mp3` | ~20 s | Breezy and dismissive, then a flicker of doubt at the end. |
| 13 | Chiamaka Okafor (31) — Sam's sister | `audio/chiamaka.mp3` | ~20 s | Direct, controlled, wants numbers, not comfort. |
| 14 | Dara Okafor (37) — Kelechi's wife | `audio/dara.mp3` | ~25 s | Calm, informed. Sets up the obligate-carrier idea. |
| 15 | Marcus Reyes (36) — Adanna's husband | `audio/marcus.mp3` | ~20 s | Easygoing, reassuring. Married in too late to explain anything. |

> Ngozi has two dialogue states: set `audio` (the refusal) and `audioDeep` (the post-pattern interview)
> on her `INTERVIEWS` entry. That makes 16 clips in total, for 15 characters.

Optional: a reading of Emeka's 1989 letter (`audio/letter.mp3`, ~60–75 s, older man's voice, slow and
private). The archive modal doesn't have an audio slot yet; it can be added the same way.

## Portraits (15)

All 512 × 512 px, square, face centered, neutral or simple background. Illustrations, student artwork or
photos all work. Since this is a fictional family, don't use photos of real people unless you have their consent.

| # | Character | File |
|---|---|---|
| 1 | Sam Okafor | `img/sam.jpg` |
| 2 | Kelechi Okafor | `img/kelechi.jpg` |
| 3 | Chidi Okafor | `img/chidi.jpg` |
| 4 | Folake Okafor | `img/folake.jpg` |
| 5 | Obi Okafor | `img/obi.jpg` |
| 6 | Yemi Okafor | `img/yemi.jpg` |
| 7 | Ngozi Bell | `img/ngozi.jpg` |
| 8 | Daniel Bell | `img/daniel.jpg` |
| 9 | Zara Bell | `img/zara.jpg` |
| 10 | Emeka Bell Jr. | `img/emekajr.jpg` |
| 11 | Adanna Reyes | `img/adanna.jpg` |
| 12 | Tobi Okafor | `img/tobi.jpg` |
| 13 | Chiamaka Okafor | `img/chiamaka.jpg` |
| 14 | Dara Okafor | `img/dara.jpg` |
| 15 | Marcus Reyes | `img/marcus.jpg` |

Not interviewed, so no portrait is needed: Emeka and Adaeze (deceased; reached through the archive) and
Nia (9) and Lola (6) (minors).

## Other editable content

All of these are plain JS objects at the top of the `<script>` in `index.html`:

- `CASE`: case number, disorder and gene names, test budget, unlock thresholds
- `FAMILY`: names, ages, roles, pedigree x-positions, hidden genotypes (`truth`)
- `COUPLES`: who is married to whom and their children (all pedigree lines are drawn from this)
- `EVIDENCE`: evidence titles, descriptions and sources
- `INTERVIEWS`: dialogue, the clue each interview grants, audio and portrait paths
- `LETTER`: Emeka's 1989 letter
- `PATTERN_OPTIONS`, `SUSPECTS`: rebuttal text for each wrong answer
- `GLOSSARY`: Field Notes terms
