# Lucky I. Ampalayohan — Digital Resume Refresh V6

This revision changes the portfolio from monochrome to a **professional black + chromatic purple aesthetic with restrained pink accents**. The direction is inspired by the mood and palette of the supplied Clove references, but does **not** use any Valorant/Clove artwork.

## V4 visual direction

- Deep near-black background remains the foundation.
- Chromatic violet is now the primary interface accent.
- Pink appears only as a secondary highlight in gradients, scans, dividers, and selected status details.
- Added subtle blurred iridescent/ribbon-like ambient lighting using CSS only.
- Existing topographic, grid, scan-line, and technical HUD effects are retained and purple-tinted.
- Navigation, buttons, timeline rails, nodes, meters, chips, card edges, and hover states now use a coordinated violet spectrum.
- The profile photo stays in its **original full color**.
- The Siemens S7-1500 certificate stays in its **original full color**.
- No portfolio content image is converted to grayscale. Only decorative effect layers may use grayscale/filtering.
- Existing V3 information hierarchy, education timeline, OJT content, PLC certificate emphasis, and Coursera placeholder remain intact.

## Files to overwrite in the GitHub repository

Copy these into the root of `luckyacads/resume`:

- `index.html`
- `styles.css`
- `script.js`
- `images/`

Keep the folder structure unchanged.

## Local preview

Open the folder in VS Code and use **Live Server**, or run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Theme palette

Primary UI range: deep black-violet → violet → chromatic purple, with restrained dusty-pink highlights. The palette is intentionally less saturated than a gaming interface so it remains appropriate for recruiters, engineering teams, automation companies, and software/IT roles.


## V5 refinements
- Updated graduate-facing copy (no longer says "graduating").
- Added supplied chromatic purple wallpaper as a subtle background layer at low opacity.
- Kept wallpaper subdued so text and resume content remain the focal point.


## V6 wallpaper persistence fix

In V5, the chromatic wallpaper used a **negative `z-index`**. Depending on
browser compositing, this could put the image behind the opaque page background,
so the texture appeared only intermittently while scrolling.

V6 places the wallpaper in its own **fixed, visible background layer** at
`z-index: 0`, keeps tech overlays at `z-index: 1`, and puts all resume content
above them at `z-index: 2`. This makes the supplied image stay visible behind
the entire page as you scroll.

- Wallpaper alpha: **32% desktop**, **26% mobile** (both below 40%).
- Original image colors preserved; no grayscale filter.
- Text panels retain dark, near-opaque backgrounds for contrast.
- Portrait and certificates still display in full color.
- Graduate wording from V5 is unchanged.

### Adjust the wallpaper strength

At the bottom of `styles.css`, find the **V6 FIX** section and adjust
`.chromatic-wallpaper { opacity: .32; }`. Try `.25` for a quieter texture or
`.38` for more visibility. On mobile, the corresponding opacity is `.26`.

### Local verification

Open `index.html` in VS Code Live Server. Check the background at the top,
after scrolling to the timeline, and at the bottom. If Live Server shows
cached styling, hard refresh the browser with `Ctrl + Shift + R`.


## V7 refinements
- Kept the hero name on one line at desktop widths when space permits.
- Smoothed alignment and spacing in the hero content.
- Refined the Profile // 01 cards so they align better and blend more naturally into the purple background.
- Preserved readability by keeping text contrast high while reducing the heavy black-block look.
