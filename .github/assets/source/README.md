# Banner source

`banner.html` is the self-contained source of the README banner (`../banner-light.png` and `../banner-dark.png`). One file holds both themes: a `@media (prefers-color-scheme: dark)` block swaps the colours.

## Identity

- **Fonts:** **DM Serif Display** (headline, with an italic second line; it echoes the chunky serif of the original logo) and **DM Sans** (body), loaded from Google Fonts.
- **Colours:** `#8c1d2c` cardinal and `#bd8b38` gold (sampled from `Lease Kings Logo.webp`: `#672529`, `#bd8b38`), `#f8f1e4` sandstone background, `#2a1215` ink and `#24100f` dark background.
- **Motif:** a street-map card: blocks around a green campus, listing pins in cardinal and gold, dashed walking-distance rings, a small crown and one "Price · safety · reviews" card.
- The logo is loaded from `../../../Lease%20Kings%20Logo.webp`.

## Re-render

From the repository root:

```bash
export CHROME_PATH="<path to a Chrome or Chromium binary>"
node render-html.mjs .github/assets/source/banner.html .github/assets/banner-light.png --scheme light
node render-html.mjs .github/assets/source/banner.html .github/assets/banner-dark.png --scheme dark
```

`render-html.mjs` is a small Playwright script (not in this repository) that opens the page at 1600 x 600, waits for fonts, and saves a 2x screenshot with the given `prefers-color-scheme`. Any headless browser that screenshots a 1600 x 600 viewport at 2x, once in light and once in dark mode, gives the same result.

## Notes for agents

- Keep the banner honest: no invented numbers, users, partners or results. Status words in the banner must match the README's "Honest status" section.
- Check both PNGs after rendering for overflow, clipped text and weak contrast.
