# Patient Zero — Placeholder Asset List

The game has 10 investigations. Every interview shows a portrait placeholder (the character's
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

**Totals:** 145 audio clips and 135 portraits across 10 cases. Every case
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

## Case 0047-N — Nakamura family · Orrin Syndrome

*autosomal recessive* · 14 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Evan Fujioka (27) | The proband · newly diagnosed | `audio/nakamura/evan.mp3` | ~40 s | `img/nakamura/evan.jpg` |
| Mei Silva (34) | Evan's cousin · diagnosed at 12 | `audio/nakamura/mei.mp3` | ~40 s | `img/nakamura/mei.jpg` |
| Grace Fujioka (63) | Younger daughter · Evan's mother | `audio/nakamura/grace.mp3` | ~35 s | `img/nakamura/grace.jpg` |
| Dennis Fujioka (65) | Grace's husband (married in) | `audio/nakamura/dennis.mp3` | ~40 s | `img/nakamura/dennis.jpg` |
| Kenji Nakamura (69) | Eldest son · Mei's father | `audio/nakamura/kenji.mp3` | ~30 s | `img/nakamura/kenji.jpg` |
| Linda Nakamura (67) | Kenji's wife (married in) · née Medeiros | `audio/nakamura/linda.mp3` | ~35 s | `img/nakamura/linda.jpg` |
| Aiko Nakamura (66) | Elder daughter · retired claims adjuster | `audio/nakamura/aiko.mp3` (refusal, ~30 s)<br>`audio/nakamura/aiko_deep.mp3` (after the pattern) | ~50 s | `img/nakamura/aiko.jpg` |
| Roy Nakamura (60) | Youngest son · runs the family crack seed store | `audio/nakamura/roy.mp3` | ~30 s | `img/nakamura/roy.jpg` |
| Leilani Nakamura (58) | Roy's wife (married in) · hula teacher | `audio/nakamura/leilani.mp3` | ~35 s | `img/nakamura/leilani.jpg` |
| Tess Nakamura (30) | Kyle's wife (married in) · audiologist | `audio/nakamura/tess.mp3` | ~35 s | `img/nakamura/tess.jpg` |
| Brandon Silva (36) | Mei's husband (married in) | `audio/nakamura/brandon.mp3` | ~40 s | `img/nakamura/brandon.jpg` |
| Kyle Nakamura (31) | Mei's brother · park ranger | `audio/nakamura/kyle.mp3` | ~30 s | `img/nakamura/kyle.jpg` |
| Lani Fujioka (25) | Evan's sister · grad student in Honolulu | `audio/nakamura/lani.mp3` | ~30 s | `img/nakamura/lani.jpg` |
| Koa Nakamura (24) | Roy & Leilani's son | `audio/nakamura/koa.mp3` | ~30 s | `img/nakamura/koa.jpg` |

No portrait needed: Hideo (deceased), Fumiko (deceased), Hana (minor), Noa (minor).

## Case 0052-W — Kowalski family · Brandt Syndrome

*autosomal recessive* · 12 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Mark Kowalski (44) | The proband · newly diagnosed | `audio/kowalski/mark.mp3` | ~35 s | `img/kowalski/mark.jpg` |
| Paul Dombrowski (38) | Theresa's son · Lily's father | `audio/kowalski/paul.mp3` | ~35 s | `img/kowalski/paul.jpg` |
| Kristen Dombrowski (36) | Paul's wife (married in) | `audio/kowalski/kristen.mp3` | ~25 s | `img/kowalski/kristen.jpg` |
| Annie Kowalski (47) | Mark's sister · ICU nurse | `audio/kowalski/annie.mp3` | ~40 s | `img/kowalski/annie.jpg` |
| Ed Kowalski (72) | Walter's son · Mark's father · retired steelworker | `audio/kowalski/ed.mp3` | ~35 s | `img/kowalski/ed.jpg` |
| Dorothy Kowalski (70) | Ed's wife (married in) · née Wiśniewski | `audio/kowalski/dorothy.mp3` | ~35 s | `img/kowalski/dorothy.jpg` |
| Steve Kowalski (40) | Mark's brother · steelworker | `audio/kowalski/steve.mp3` | ~30 s | `img/kowalski/steve.jpg` |
| Carol Kowalski (43) | Mark's wife (married in) | `audio/kowalski/carol.mp3` | ~35 s | `img/kowalski/carol.jpg` |
| Julie Kaminski (42) | Theresa's daughter · paralegal | `audio/kowalski/julie.mp3` | ~40 s | `img/kowalski/julie.jpg` |
| Theresa Dombrowski (69) | Walter's daughter · Lily's grandmother | `audio/kowalski/theresa.mp3` (refusal, ~35 s)<br>`audio/kowalski/theresa_deep.mp3` (after the pattern) | ~45 s | `img/kowalski/theresa.jpg` |
| Frank Dombrowski (71) | Theresa's husband (married in) | `audio/kowalski/frank.mp3` | ~30 s | `img/kowalski/frank.jpg` |
| Dave Kaminski (44) | Julie's husband (married in) | `audio/kowalski/dave.mp3` | ~25 s | `img/kowalski/dave.jpg` |

No portrait needed: Walter (deceased), Helen (deceased), Tyler (minor), Ben (minor), Lily (minor).

## Case 0058-C — Castillo family · Vance-Ortiz Syndrome

*autosomal recessive* · 15 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Daniela Salinas (26) | The proband · newly diagnosed | `audio/castillo/daniela.mp3` | ~40 s | `img/castillo/daniela.jpg` |
| Andrés Salinas (31) | Daniela's brother · diagnosed at 4 | `audio/castillo/andres.mp3` | ~35 s | `img/castillo/andres.jpg` |
| Gabriel Castillo (28) | Daniela's cousin · diagnosed at 15 | `audio/castillo/gabriel.mp3` | ~35 s | `img/castillo/gabriel.jpg` |
| Lupe Salinas (67) | Elder daughter · mother of Andrés & Daniela | `audio/castillo/lupe.mp3` | ~30 s | `img/castillo/lupe.jpg` |
| Héctor Salinas (69) | Lupe's husband (married in) · construction foreman | `audio/castillo/hector.mp3` | ~35 s | `img/castillo/hector.jpg` |
| Tony Castillo (61) | Younger son · Gabriel's father · owns a tire shop | `audio/castillo/tony.mp3` | ~30 s | `img/castillo/tony.jpg` |
| Norma Castillo (59) | Tony's wife (married in) · née Treviño, from Laredo | `audio/castillo/norma.mp3` | ~35 s | `img/castillo/norma.jpg` |
| Víctor Salinas (35) | Daniela's eldest brother · biology teacher | `audio/castillo/victor.mp3` | ~40 s | `img/castillo/victor.jpg` |
| Josh Morales (34) | Isabel's husband (married in) · football coach | `audio/castillo/josh.mp3` | ~35 s | `img/castillo/josh.jpg` |
| Sofía Brennan (22) | Marisol's daughter · culinary student | `audio/castillo/sofia.mp3` | ~40 s | `img/castillo/sofia.jpg` |
| Rubén Castillo (70) | Eldest son · retired Air Force mechanic | `audio/castillo/ruben.mp3` (refusal, ~40 s)<br>`audio/castillo/ruben_deep.mp3` (after the pattern) | ~50 s | `img/castillo/ruben.jpg` |
| Marisol Brennan (64) | Middle daughter · real-estate agent | `audio/castillo/marisol.mp3` | ~30 s | `img/castillo/marisol.jpg` |
| Greg Brennan (66) | Marisol's husband (married in) | `audio/castillo/greg.mp3` | ~35 s | `img/castillo/greg.jpg` |
| Bea Castillo (57) | Youngest daughter · elementary school principal | `audio/castillo/bea.mp3` | ~35 s | `img/castillo/bea.jpg` |
| Isabel Morales (33) | Gabriel's sister · pharmacist | `audio/castillo/isabel.mp3` | ~35 s | `img/castillo/isabel.jpg` |

No portrait needed: Arturo (deceased), Esperanza (deceased), Mateo (minor).

## Case 0063-M — Mendoza family · Tessaly Muscular Dystrophy

*X-linked recessive* · 14 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Gabriel "Gabe" Santos (19) | The proband · newly diagnosed | `audio/mendoza/gabe.mp3` | ~40 s | `img/mendoza/gabe.jpg` |
| Nico Bautista (40) | Tess's son · affected since age 11 | `audio/mendoza/nico.mp3` | ~35 s | `img/mendoza/nico.jpg` |
| Joy Bautista (37) | Nico's sister · ER nurse | `audio/mendoza/joy.mp3` | ~35 s | `img/mendoza/joy.jpg` |
| Jomar Mendoza (30) | Bong's son · high-school chemistry teacher | `audio/mendoza/jomar.mp3` | ~40 s | `img/mendoza/jomar.jpg` |
| Rogelio "Bong" Mendoza (62) | Elder son · affected since boyhood | `audio/mendoza/bong.mp3` | ~40 s | `img/mendoza/bong.jpg` |
| Linda Mendoza (61) | Bong's wife (married in) | `audio/mendoza/linda.mp3` | ~35 s | `img/mendoza/linda.jpg` |
| Carla Okada (33) | Bong's daughter · expecting her second child | `audio/mendoza/carla.mp3` | ~35 s | `img/mendoza/carla.jpg` |
| Teresita "Tess" Bautista (66) | Eldest daughter · Nico's mother | `audio/mendoza/tess.mp3` | ~35 s | `img/mendoza/tess.jpg` |
| Ronald Bautista (68) | Tess's husband (married in) · from Pampanga | `audio/mendoza/ronald.mp3` | ~30 s | `img/mendoza/ronald.jpg` |
| Marilou Santos (58) | Younger daughter · Gabe's mother | `audio/mendoza/marilou.mp3` | ~40 s | `img/mendoza/marilou.jpg` |
| Dennis Santos (60) | Marilou's husband (married in) | `audio/mendoza/dennis.mp3` | ~30 s | `img/mendoza/dennis.jpg` |
| Ana Santos (24) | Gabe's sister | `audio/mendoza/ana.mp3` | ~25 s | `img/mendoza/ana.jpg` |
| Ryan Okada (35) | Carla's husband (married in) | `audio/mendoza/ryan.mp3` | ~30 s | `img/mendoza/ryan.jpg` |
| Rodel Mendoza (55) | Youngest son · keeps Lola's house | `audio/mendoza/rodel.mp3` (refusal, ~35 s)<br>`audio/mendoza/rodel_deep.mp3` (after the pattern) | ~55 s | `img/mendoza/rodel.jpg` |

No portrait needed: Ernesto (deceased), Cora (deceased), Mia (minor).

## Case 0071-B — O'Brien family · Ashgrove Factor Deficiency

*X-linked recessive* · 14 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Conor Doyle (24) | The proband · newly diagnosed | `audio/obrien/conor.mp3` | ~40 s | `img/obrien/conor.jpg` |
| Brendan Walsh (48) | Sheila's son · diagnosed 1986 | `audio/obrien/brendan.mp3` | ~40 s | `img/obrien/brendan.jpg` |
| Erin Doyle (29) | Conor's sister · pregnant | `audio/obrien/erin.mp3` | ~35 s | `img/obrien/erin.jpg` |
| Sheila Walsh (72) | Eldest daughter · Brendan's mother | `audio/obrien/sheila.mp3` | ~35 s | `img/obrien/sheila.jpg` |
| Tom Walsh (74) | Sheila's husband (married in) · retired MBTA electrician | `audio/obrien/tom.mp3` | ~30 s | `img/obrien/tom.jpg` |
| Kevin O'Brien (66) | Only son · runs the family pub | `audio/obrien/kevin.mp3` | ~35 s | `img/obrien/kevin.jpg` |
| Anne O'Brien (64) | Kevin's wife (married in) | `audio/obrien/anne.mp3` | ~35 s | `img/obrien/anne.jpg` |
| Mike Doyle (65) | Deirdre's husband (married in) · ex-hockey player | `audio/obrien/mike.mp3` | ~35 s | `img/obrien/mike.jpg` |
| Deirdre Doyle (63) | Youngest daughter · Conor's mother | `audio/obrien/deirdre.mp3` | ~35 s | `img/obrien/deirdre.jpg` |
| Kerry Walsh (47) | Brendan's wife (married in) | `audio/obrien/kerry.mp3` | ~30 s | `img/obrien/kerry.jpg` |
| Maura Walsh (45) | Brendan's sister · public defender | `audio/obrien/maura.mp3` | ~35 s | `img/obrien/maura.jpg` |
| Siobhan Walsh (20) | Brendan's daughter · biology major | `audio/obrien/siobhan.mp3` | ~35 s | `img/obrien/siobhan.jpg` |
| Liam Walsh (18) | Brendan's son · plays hurling | `audio/obrien/liam.mp3` | ~30 s | `img/obrien/liam.jpg` |
| Noreen O'Brien (69) | Second daughter · retired ICU nurse | `audio/obrien/noreen.mp3` (refusal, ~40 s)<br>`audio/obrien/noreen_deep.mp3` (after the pattern) | ~55 s | `img/obrien/noreen.jpg` |

No portrait needed: Paddy (deceased), Maureen (deceased), Katie (minor).

## Case 0079-P — Patel family · Rennick Retinopathy

*X-linked recessive* · 12 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Arjun Shah (23) | The proband · newly diagnosed | `audio/patel/arjun.mp3` | ~35 s | `img/patel/arjun.jpg` |
| Nikhil Desai (44) | Hema's son · night-blind since age 9 | `audio/patel/nikhil.mp3` | ~35 s | `img/patel/nikhil.jpg` |
| Riya Shah (27) | Arjun's sister · engaged | `audio/patel/riya.mp3` | ~40 s | `img/patel/riya.jpg` |
| Pooja Patel (30) | Bharat's daughter · optometrist | `audio/patel/pooja.mp3` | ~45 s | `img/patel/pooja.jpg` |
| Kavita Desai (41) | Nikhil's sister · software engineer | `audio/patel/kavita.mp3` | ~25 s | `img/patel/kavita.jpg` |
| Priya Desai (42) | Nikhil's wife (married in) · pediatrician | `audio/patel/priya.mp3` | ~35 s | `img/patel/priya.jpg` |
| Meena Patel (64) | Bharat's wife (married in) · yoga teacher | `audio/patel/meena.mp3` | ~30 s | `img/patel/meena.jpg` |
| Suresh Desai (73) | Hema's husband (married in) · diabetic | `audio/patel/suresh.mp3` | ~30 s | `img/patel/suresh.jpg` |
| Bharat Patel (67) | Only son · runs a motel in Edison | `audio/patel/bharat.mp3` | ~30 s | `img/patel/bharat.jpg` |
| Ajay Shah (64) | Rekha's husband (married in) · accountant | `audio/patel/ajay.mp3` | ~30 s | `img/patel/ajay.jpg` |
| Rekha Shah (62) | Younger daughter · Arjun's mother | `audio/patel/rekha.mp3` | ~35 s | `img/patel/rekha.jpg` |
| Hema Desai (70) | Eldest daughter · Nikhil's mother | `audio/patel/hema.mp3` (refusal, ~35 s)<br>`audio/patel/hema_deep.mp3` (after the pattern) | ~50 s | `img/patel/hema.jpg` |

No portrait needed: Ramanbhai (deceased), Savita (deceased), Anika (minor), Rohan (minor).

## Case 0084-L — Moreau family · Laurent Chorea

*autosomal dominant (late onset)* · 13 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Marc Moreau (45) | The proband · newly diagnosed | `audio/moreau/marc.mp3` | ~35 s | `img/moreau/marc.jpg` |
| Nathalie Moreau (44) | Marc's wife (married in) | `audio/moreau/nathalie.mp3` | ~45 s | `img/moreau/nathalie.jpg` |
| Gérard Moreau (70) | Armand's son · Marc's father · symptoms since 44 | `audio/moreau/gerard.mp3` | ~30 s | `img/moreau/gerard.jpg` |
| Lise Moreau (68) | Gérard's wife (married in) | `audio/moreau/lise.mp3` | ~35 s | `img/moreau/lise.jpg` |
| Julie Moreau (42) | Marc's sister · ER nurse | `audio/moreau/julie.mp3` | ~35 s | `img/moreau/julie.jpg` |
| Ginette Pelletier (67) | Armand's daughter · keeps her mother's papers | `audio/moreau/ginette.mp3` (refusal, ~35 s)<br>`audio/moreau/ginette_deep.mp3` (after the pattern) | ~50 s | `img/moreau/ginette.jpg` |
| Roger Pelletier (69) | Ginette's husband (married in) | `audio/moreau/roger.mp3` | ~40 s | `img/moreau/roger.jpg` |
| Paul Gagnon (66) | Denise's husband (married in) · retired mill foreman | `audio/moreau/paul.mp3` | ~40 s | `img/moreau/paul.jpg` |
| Denise Gagnon (64) | Armand's youngest · symptoms since 46 | `audio/moreau/denise.mp3` | ~35 s | `img/moreau/denise.jpg` |
| Sophie Gagnon (36) | Denise's daughter · physical therapist | `audio/moreau/sophie.mp3` | ~35 s | `img/moreau/sophie.jpg` |
| Luc Gagnon (33) | Denise's son · line cook | `audio/moreau/luc.mp3` | ~35 s | `img/moreau/luc.jpg` |
| Mathieu Pelletier (40) | Ginette's son | `audio/moreau/mathieu.mp3` | ~30 s | `img/moreau/mathieu.jpg` |
| Annie Pelletier (37) | Ginette's daughter · genealogy hobbyist | `audio/moreau/annie.mp3` | ~30 s | `img/moreau/annie.jpg` |

No portrait needed: Armand (deceased), Thérèse (deceased), Émile (minor), Chloé (minor).

## Case 0090-K — Kim family · Sterling Cardiomyopathy

*autosomal dominant (late onset)* · 13 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Daniel Kim (34) | The proband · survived cardiac arrest | `audio/kim/daniel.mp3` | ~35 s | `img/kim/daniel.jpg` |
| Rachel Kim (33) | Daniel's wife (married in) · paralegal | `audio/kim/rachel.mp3` | ~50 s | `img/kim/rachel.jpg` |
| Jenny Kim (61) | Steve's wife (married in) · church choir director | `audio/kim/jenny.mp3` | ~35 s | `img/kim/jenny.jpg` |
| Steve (Sung-ho) Kim (63) | Eldest son · Daniel's father · defibrillator since 41 | `audio/kim/steve.mp3` | ~40 s | `img/kim/steve.jpg` |
| Grace (Eun-ji) Kim (60) | Daughter · life-insurance underwriter · keeps her mother's things | `audio/kim/grace.mp3` (refusal, ~35 s)<br>`audio/kim/grace_deep.mp3` (after the pattern) | ~50 s | `img/kim/grace.jpg` |
| Helen (Hye-jin) Alvarez (57) | Younger daughter · fainting since 44 | `audio/kim/helen.mp3` | ~40 s | `img/kim/helen.jpg` |
| Mark Alvarez (59) | Helen's husband (married in) · mail carrier | `audio/kim/mark.mp3` | ~30 s | `img/kim/mark.jpg` |
| Peter (Jae-won) Kim (54) | Youngest son · runs the family's print shop | `audio/kim/peter.mp3` | ~30 s | `img/kim/peter.jpg` |
| Mina Kim (52) | Peter's wife (married in) | `audio/kim/mina.mp3` | ~30 s | `img/kim/mina.jpg` |
| Joseph Alvarez (29) | Helen's son · firefighter | `audio/kim/joseph.mp3` | ~40 s | `img/kim/joseph.jpg` |
| Lily Alvarez (26) | Helen's daughter · digitizes old media | `audio/kim/lily.mp3` | ~40 s | `img/kim/lily.jpg` |
| Sarah Kim (31) | Daniel's sister · graphic designer | `audio/kim/sarah.mp3` | ~35 s | `img/kim/sarah.jpg` |
| Andrew Kim (22) | Peter's son · college senior | `audio/kim/andrew.mp3` | ~30 s | `img/kim/andrew.jpg` |

No portrait needed: Dong-su (deceased), Young-ja (deceased), Noah (minor), Hana (minor).

## Case 0096-R — Rossi family · Calder Neuropathy

*autosomal dominant (late onset)* · 13 interviews

| Character | Role | Audio | Length | Portrait |
|---|---|---|---|---|
| Gina DiMaio (41) | The proband · newly diagnosed | `audio/rossi/gina.mp3` | ~30 s | `img/rossi/gina.jpg` |
| Rosaria DiMaio (76) | Eldest daughter · Gina's mother · symptoms since 38 | `audio/rossi/rosaria.mp3` (refusal, ~40 s)<br>`audio/rossi/rosaria_deep.mp3` (after the pattern) | ~45 s | `img/rossi/rosaria.jpg` |
| Frank DiMaio (78) | Rosaria's husband (married in) · type 2 diabetes | `audio/rossi/frank.mp3` | ~30 s | `img/rossi/frank.jpg` |
| Paul DiMaio (45) | Gina's brother · insurance adjuster | `audio/rossi/paul.mp3` | ~35 s | `img/rossi/paul.jpg` |
| Anthony 'Tony' Rossi (72) | Son · retired barber · symptoms since 39 | `audio/rossi/tony.mp3` | ~45 s | `img/rossi/tony.jpg` |
| Linda Rossi (70) | Tony's wife (married in) | `audio/rossi/linda.mp3` | ~35 s | `img/rossi/linda.jpg` |
| Joe Rossi (68) | Youngest son · 22 years at a jewelry plating plant | `audio/rossi/joe.mp3` | ~40 s | `img/rossi/joe.jpg` |
| Donna Rossi (66) | Joe's wife (married in) · school librarian | `audio/rossi/donna.mp3` | ~35 s | `img/rossi/donna.jpg` |
| Michael Rossi (47) | Tony's son · electrician · symptoms since 39 | `audio/rossi/michael.mp3` | ~35 s | `img/rossi/michael.jpg` |
| Teresa Rossi (46) | Michael's wife (married in) | `audio/rossi/teresa.mp3` | ~35 s | `img/rossi/teresa.jpg` |
| Angela Rossi (38) | Tony's daughter · high-school biology teacher | `audio/rossi/angela.mp3` | ~35 s | `img/rossi/angela.jpg` |
| Nicky Rossi (35) | Joe's son · chef | `audio/rossi/nicky.mp3` | ~35 s | `img/rossi/nicky.jpg` |
| Luca Rossi (19) | Michael & Teresa's son · college sophomore | `audio/rossi/luca.mp3` | ~40 s | `img/rossi/luca.jpg` |

No portrait needed: Salvatore (deceased), Concetta (deceased), Sofia (minor).
