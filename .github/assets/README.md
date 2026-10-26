# README images

Images used by the root `README.md`.

| File | What it is | How it was made |
| --- | --- | --- |
| `banner-light.png`, `banner-dark.png` | README banner for light and dark mode | Rendered from [`source/banner.html`](source/banner.html) with headless Chrome (26 October 2026), using `Lease Kings Logo.webp` |
| `where-it-stands.svg` | Five-stage summary of the project's progress | Hand-written SVG in the README palette (cardinal, sandstone, DM Sans with system fallbacks); the text summarises the repository's documents |

The hero image is the existing conceptual cover in `assets/brand/cover.png` (AI-generated, fictional buildings).

This repository has no running software, so there are no app screenshots. `Areas near USC.png` is deliberately not shown in the README because it includes a video-call participant. Images here must only show public or synthetic content; never add interview, survey or personal details to them.

## Visual identity

Rental and student-housing products are map-first, with pins, filters and walk times on every listing. The original logo's cardinal-and-gold crown sets the warmer, campus-spirited tone.

- **Fonts:** **DM Serif Display** (headline, with an italic second line; it echoes the chunky serif of the original logo) and **DM Sans** (body).
- **Colours:** `#8c1d2c` cardinal and `#bd8b38` gold (sampled from `Lease Kings Logo.webp`: `#672529`, `#bd8b38`), `#f8f1e4` sandstone background, `#2a1215` ink and `#24100f` dark background.
- **Motif:** a street-map card: blocks around a green campus, listing pins in cardinal and gold, dashed walking-distance rings, a small crown and one "Price · safety · reviews" card.

The README badges use the same colours. To change the banner, edit [`source/banner.html`](source/banner.html) and follow [`source/README.md`](source/README.md) to re-render both PNGs.
