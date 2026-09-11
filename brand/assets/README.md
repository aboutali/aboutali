# Brand assets

Generated from the locked v3 anchors (cobalt · Archivo · *"Curiosity meets rigor"*).
All PNGs are flat and font-independent (Archivo / Newsreader / JetBrains Mono baked
into pixels). Regenerate with:

```bash
NODE_PATH=$(npm root -g) node brand/assets/generate.cjs
```

| File | Size | Use |
|------|------|-----|
| `favicon-16.png` / `favicon-32.png` / `favicon-48.png` | 16–48px | Browser favicons |
| `apple-touch-icon.png` | 180px | iOS home-screen icon |
| `icon-512.png` | 512px | PWA / maskable app icon, large favicon |
| `avatar-512.png` | 512px | `AB` monogram — social avatars, profile pics |
| `wordmark-light.png` | — | Primary logo, ink + cobalt on paper |
| `wordmark-reversed.png` | — | Logo for dark / cobalt backgrounds |
| `og-image.png` | 1200×630 | Open Graph / Twitter share card — homepage |
| `og-about.png` | 1200×630 | Share card — About |
| `og-writing.png` | 1200×630 | Share card — Writing index |
| `og-cv.png` | 1200×630 | Share card — CV |
| `og-post-hello-world.png` | 1200×630 | Share card — Writing post: "Hello, world — what this site is" |
| `og-work-life-improver.png` | 1200×630 | Share card — Work case study: life-improver |
| `og-work-bxl_eda_worker.png` | 1200×630 | Share card — Work case study: bxl_eda_worker |
| `og-work-fit-schedule.png` | 1200×630 | Share card — Work case study: fit-schedule |
| `og-work-cloudy-plag.png` | 1200×630 | Share card — Work case study: cloudy-plag |
| `og-work-edition-guru.png` | 1200×630 | Share card — Work case study: edition-guru |
| `og-work-iKoyomi.png` | 1200×630 | Share card — Work case study: iKoyomi |

## Favicon `<head>` snippet

```html
<link rel="icon" type="image/png" sizes="32x32" href="/brand/assets/favicon-32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/brand/assets/favicon-16.png">
<link rel="apple-touch-icon" sizes="180x180" href="/brand/assets/apple-touch-icon.png">
<meta property="og:image" content="/brand/assets/og-image.png">
<meta property="og:title" content="Angelo Boutalikakis">
<meta property="og:description" content="Curiosity meets rigor.">
```

> These are 2× raster exports — crisp everywhere a PNG is expected. For print or
> infinitely-scalable logos, the wordmark/monogram can be outlined to **SVG** from
> Archivo as a follow-up (ask and I'll add `wordmark.svg` + `icon.svg`).
