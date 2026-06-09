# Timemark Replica

A browser-based camera timestamp watermark tool that replicates the look of the **Timemark** app. Built with HTML5 Canvas, vanilla JavaScript, and CSS — everything runs locally in your browser with no server uploads.

## Features

- **Timemark-style watermark** — tall condensed clock, vertical divider line, stacked date lines, and drop shadows that scale with image resolution
- **27 locales** — date and weekday formatting via `Intl` (Indonesian, Japanese, Chinese, Korean, Swedish, Arabic, and more)
- **Timezone-aware defaults** — locale is auto-detected from your IANA timezone on load
- **Smart metadata import** on image upload:
  - Date/time from EXIF
  - Filename timestamp fallback (e.g. `IMG_20240609_143022.jpg`)
  - GPS reverse geocoding for location (OpenStreetMap Nominatim)
  - Toast feedback showing what was extracted
- **Manual overrides** — edit date, time, date lines, and location; weekday is inferred from the selected date
- **Layout presets** — two built-in date layouts plus a fully custom text mode
- **Design controls** — font family (Barlow Condensed / Oswald), 12h/24h clock, text/divider colors, scale, margins, divider size/offset, shadow opacity/blur/offset
- **EXIF on export** — downloaded JPEGs include injected date/time metadata via [piexifjs](https://github.com/hMatoba/piexifjs)
- **Drag & drop** — drop an image anywhere on the preview to load it
- **Private** — images never leave your device

## Getting Started

### Install

```bash
git clone https://github.com/okasi/timemark-replica.git
cd timemark-replica
npm install
```

### Development

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Production build

```bash
npm run build
```

Output is written to `dist/`. The Vite config uses relative asset paths (`base: './'`) so the build works on GitHub Pages.

## Deployment

Pushes to `main` automatically deploy to GitHub Pages via the workflow in `.github/workflows/deploy.yml` (Node 24, `npm ci` + `npm run build`).

## Tech Stack

| Layer | Stack |
|---|---|
| Core | HTML5, Canvas API, ES modules |
| Styling | Vanilla CSS (Grid, custom properties, glassmorphism) |
| Metadata | [piexifjs](https://www.npmjs.com/package/piexifjs) |
| Tooling | Vite 5 |

## License

MIT
