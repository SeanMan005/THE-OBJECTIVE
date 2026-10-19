# What an Algorithm Is

Settled refusal, standing asymmetry, and measurable reach — the reference text
plus one figure per idea, and a site that walks them in order.

**Open `index.html`.** It is self-contained: the five figures are embedded, so
it works offline and can be moved anywhere on its own.

---

## What is here

```
WHAT IS AN ALGORITHM/
├── index.html                          the site (plain-language walkthrough, 5 figures)
├── What an Algorithm Is.md             the reference text the site follows
├── cover.jpg                           the cover plate at the head of the site
├── what_an_algorithm_is_diagram.png    all five panels on one sheet
├── figures/                            one PNG per panel, as used on the site
│   └── algorithm_panel_1–5.png
└── scripts/
    ├── algorithm_panels.py             draws the five panels and the sheet
    ├── build_algorithm_page.py         inlines the plates into index.html
    └── what-an-algorithm-is.src.html   the page template ({{PANEL_1}}…{{PANEL_5}})
```

## The five panels

Each panel is one bullet of the **In Simple Terms** section of
`What an Algorithm Is.md`, drawn.

| | Panel | The idea it draws |
|---|---|---|
| I | Settled refusal, not stored volume | A corpus logs arrivals; linkage logs verdicts. Only a settled comparison deposits structure. |
| II | The two motions that build it | Reaching extends scope, tightening raises resolution — scope × resolution is the deposit. |
| III | The seat changes hands | A smooth deposit against a moving arrival weight: the verdict flips from *files* to *places*. |
| IV | Why it commands | A spark spends its gap and becomes the baseline; an algorithm re-makes the gap every cycle. |
| V | How far it reaches | Remaining depth D — three owners (rate, direction, reach) and four readings of one number. |

## The four source theories

All in `NEW FILES/` in the project root, and also bundled in
`NEW FILES/COMMAND MEDIUM/theories/`:

- **The Selector Gradient** — the column, the seat, and the funded arc
- **The Absorption Threshold** — the hinge; why a smooth deposit flips sharply
- **The Commanding Deposit** — D, its four readings, the latency law
- **The Standing Asymmetry** — the conductive base; rate / direction / reach

## Rebuilding

Paths resolve against the scripts themselves, so run these from this folder:

```bash
python scripts/algorithm_panels.py        # figures/algorithm_panel_1–5.png + the sheet
python scripts/build_algorithm_page.py    # index.html
```

Edit the prose in `scripts/what-an-algorithm-is.src.html` and re-run the build
step; edit the drawing in `scripts/algorithm_panels.py` and re-run both, since
the page embeds the plates rather than linking them.

Swapping the cover is just replacing `cover.jpg` and re-running the build — it
is downscaled to 1800px and re-encoded as a progressive JPEG on the way in. The
title sits on the plate under a gradient scrim that goes near-opaque at the
base, so the art stays legible at the top and the type keeps its contrast at
the bottom.

The page template reuses the stylesheet from
`NEW FILES/COMMAND MEDIUM/scripts/the-commanded-medium.src.html`, so the two
bundles read as one family. It is copied in, not linked — changing one does not
change the other.

Requires `matplotlib`, `numpy` and `pillow`.

---

Refusal deposits linkage · linkage past a density reads as a cost function · a
cost function at an apex is a maintained Δ · a bound base conducts toward Δ with
its own energy · the verdict at the door decides which side holds the seat · D
decides how far the seat reaches.
