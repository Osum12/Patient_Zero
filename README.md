# Patient Zero

An interactive genetics mystery. Students play a genetic counselor investigating the Okafor family:
Sam (28) was just diagnosed with Keller Syndrome, a fictional autosomal recessive disorder, and his
cousin Kelechi has had it since age 15. The goal is to trace the four-generation pedigree back to the
family's "patient zero": the ancestor through whom the variant entered the family.

The family and the disorder are fictional.

## Play

Open `index.html` in any modern browser. It's one self-contained file and works offline from `file://`.
Progress saves to the browser's localStorage. "Restart" restarts the case, and "Start over" on the title
screen clears everything.

On phones the pedigree switches to a vertical layout (generations as columns, families top to bottom),
so it fits the screen without sideways scrolling.

## Customize

The case is one `CASES.push({...})` block near the top of the `<script>` in `index.html`: names,
dialogue, evidence, rebuttals and asset paths are all plain JS objects. See [CONTENT.md](CONTENT.md)
for the list of placeholder audio clips and portraits to record or create.
