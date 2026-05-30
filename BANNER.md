# LinkedIn / GitHub Banner Generator

A single self-contained HTML file — [banner.html](banner.html) — that renders a dark, modern
profile banner (name, location, a glowing multi-agent network graph, tagline, and tech-stack
chips). Open it in a browser and export it to a high-quality PNG/JPG at any resolution. No
build step, no JS dependencies.

![banner preview](banner.png)

---

## What's in the file

Everything is inline in `banner.html`:

- **Fonts** — `Playfair Display` (the serif name + italic tagline) and `JetBrains Mono`
  (labels and chips), pulled from Google Fonts.
- **Layout** — a single `.banner` element (`1400 × 340`, rounded border) with absolutely
  positioned blocks: location (top-left), eyebrow + name + tagline (right), tech chips
  (bottom-right).
- **Network graph** — an inline `<svg>` with gradient edges, faint satellite nodes, and three
  glowing hub nodes (blue / cyan / purple) using radial-gradient fills, a soft blur filter,
  and concentric halo rings.
- **Theme** — all colors and the export size live in the `:root { --... }` block at the top
  of the `<style>` tag. Change them there.

### Editing

| Want to change…   | Edit this                                                     |
| ----------------- | ------------------------------------------------------------- |
| Name / tagline    | `.name` and `.tagline` text in the `<body>`                   |
| Location / handle | `.meta .loc` and `.meta .handle`                              |
| Tech chips        | the `.badge` spans inside `.badges`                           |
| Colors            | the `--bg-*`, `--accent-*`, `--text` vars in `:root`          |
| Chip glow         | the `box-shadow` on `.badge`                                  |
| Export size       | `--W` / `--H` in `:root`                                      |
| Graph shape       | the `<line>` / `<circle>` coords inside `<svg class="graph">` |
| Graph colors      | the `<radialGradient>` / `<linearGradient>` stops in `<defs>` |

> The tagline `&` is rendered in a sans-serif (`.tagline .amp`) on purpose — Playfair's
> italic ampersand is an ornate squiggle, so this keeps it clean.

---

## How to export it as a high-quality PNG / JPG

### Option A — Headless Chrome (one command, repeatable)

```bash
# PNG, 2× for retina sharpness -> outputs a 2800 × 680 image
google-chrome-stable --headless --screenshot=banner.png \
  --window-size=1400,340 --default-background-color=00000000 \
  --force-device-scale-factor=2 \
  "file://$PWD/banner.html"
```

Notes:

- A `vaInitialize failed: unknown libva error` line is a **harmless** GPU/VA-API warning —
  the screenshot is still written (you'll see `… bytes written to file banner.png`). Append
  `--disable-gpu` to silence it if you like; it's not required.
- `--default-background-color=00000000` keeps the corners transparent (the card has rounded
  corners); use `ffffffff` for an opaque white page background.
- Bump `--force-device-scale-factor` to `3` for an even sharper `4200 × 1020` image.

**Want a JPG?** Headless Chrome only writes PNG, so convert the PNG afterward (JPG has no
transparency, so flatten the rounded corners onto a background — here near-black `#06070b`):

```bash
# ImageMagick (v7: `magick`, v6: `convert`)
magick banner.png -background "#06070b" -flatten -quality 95 banner.jpg

# or with ffmpeg
ffmpeg -i banner.png -q:v 2 banner.jpg
```

### Option B — Browser screenshot (no CLI)

1. Open `banner.html` in Chrome/Edge.
2. Open DevTools (`F12`) → toggle device toolbar (`Ctrl/Cmd + Shift + M`).
3. Set a custom size of `1400 × 340` (or whatever you set `--W`/`--H` to).
4. Command menu (`Ctrl/Cmd + Shift + P`) → **"Capture node screenshot"** → pick the
   `.banner` element.

### Option C — Puppeteer (best quality, PNG _and_ JPG)

```bash
npm i -D puppeteer
```

```js
// export.js  ->  node export.js
const puppeteer = require("puppeteer");

(async () => {
  const browser = await puppeteer.launch();
  const page = await browser.newPage();
  // deviceScaleFactor: 2 (or 3) = crisp, high-DPI output
  await page.setViewport({ width: 1500, height: 440, deviceScaleFactor: 3 });
  await page.goto("file://" + __dirname + "/banner.html", {
    waitUntil: "networkidle0", // waits for Google Fonts to load
  });
  const el = await page.$("#banner");

  await el.screenshot({ path: "banner.png" }); // PNG (lossless)
  await el.screenshot({ path: "banner.jpg", quality: 100 }); // JPG (high quality)

  await browser.close();
})();
```

> **Tip:** always wait for fonts (`waitUntil: "networkidle0"`). If you screenshot too early
> the serif name falls back to a system font and won't match.

---

## Recommended sizes

| Use                   | Dimensions (`--W × --H`) | Notes                          |
| --------------------- | ------------------------ | ------------------------------ |
| LinkedIn cover        | 1584 × 396               | safe zone — keep text centered |
| GitHub profile README | 1400 × 340 (default)     | renders crisply at 2×          |
| Twitter / X header    | 1500 × 500               | adjust `--H` for more height   |
