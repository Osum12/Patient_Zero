# Patient Zero

An interactive genetics mystery. Students play a genetic counselor tracing a fictional inherited
disorder through a four-generation family pedigree to find the family's "patient zero": the ancestor
through whom the variant entered the family.

There are 10 investigations, each with its own family, disorder, interviews and archive document.
"Start random investigation" picks a case you haven't closed yet.

| Case | Family | Disorder | Pattern |
|---|---|---|---|
| 0031-K | Okafor | Keller Syndrome | Autosomal recessive |
| 0047-N | Nakamura | Orrin Syndrome | Autosomal recessive |
| 0052-W | Kowalski | Brandt Syndrome | Autosomal recessive |
| 0058-C | Castillo | Vance-Ortiz Syndrome | Autosomal recessive |
| 0063-M | Mendoza | Tessaly Muscular Dystrophy | X-linked recessive |
| 0071-B | O'Brien | Ashgrove Factor Deficiency | X-linked recessive |
| 0079-P | Patel | Rennick Retinopathy | X-linked recessive |
| 0084-L | Moreau | Laurent Chorea | Autosomal dominant, late onset |
| 0090-K | Kim | Sterling Cardiomyopathy | Autosomal dominant, late onset |
| 0096-R | Rossi | Calder Neuropathy | Autosomal dominant, late onset |

All families and disorders are fictional.

## Play

Open `index.html` in any modern browser. It's one self-contained file and works offline from `file://`.
Progress saves to the browser's localStorage. "Restart" restarts the current case, and "Erase all
progress" on the title screen clears everything.

## Customize

Each case is one `CASES.push({...})` block near the top of the `<script>` in `index.html`: names,
dialogue, evidence, rebuttals and asset paths are all plain JS objects. See [CONTENT.md](CONTENT.md)
for the list of placeholder audio clips and portraits to record or create.
