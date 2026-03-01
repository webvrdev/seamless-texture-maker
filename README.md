# Seamless Texture Maker (Beta)

A fast, **client-side** web tool to turn an image into a **tileable (seamless) texture** by mirroring and softly blending edge strips.

**Live:** https://seamless.webvrdev.com/

---

## What it does

- **Horizontal pass:** copy a strip from the **left edge**, mirror it, blend onto the **right edge**
- **Vertical pass:** copy a strip from the **top edge**, mirror it, blend onto the **bottom edge**
- The result stays close to the original texture (no “creative retile” / no AI).

---

## Features

- ✅ 100% **local** in the browser (no server, no uploads)
- ✅ Clean, controllable controls: **strip size**, **feather**, **opacity**
- ✅ Live tiled stage preview  
  - Drag = pan  
  - Mouse wheel = zoom  
  - Shift + wheel = tile size  
  - Double click = reset view
- ✅ Export **PNG / WebP / JPG**
- ✅ Minimal Skybox-style UI (movable panel, collapsible to gear)

---

## Quick start

### Option A — Run locally
1. Download this repo
2. Open `index.html` in your browser (Chrome / Edge recommended)

### Option B — GitHub Pages
1. Push the repo to GitHub
2. In **Settings → Pages**
   - Source: `Deploy from a branch`
   - Branch: `main` / `/ (root)`
3. (Optional) Custom domain: `seamless.webvrdev.com`  
   This repo includes a `CNAME` file.

---

## Documentation

- **Manual & FAQ:** open `manual.html`
- Banner image: `assets/banner.png`

---

## Repo structure

```
.
├─ index.html                 # the app
├─ manual.html                # manual & FAQ (same style)
├─ assets/
│  ├─ banner.png
│  └─ favicon.svg
├─ CNAME                      # custom domain (GitHub Pages)
├─ .nojekyll
├─ LICENSE
├─ CHANGELOG.md
├─ CONTRIBUTING.md
└─ SECURITY.md
```

---

## Known limitations (Beta)

- Best results on organic / noisy materials (concrete, dirt, fabric).
- Structured patterns (tiles/bricks) can still reveal repetition if the original photo is not aligned.
  Try smaller strip sizes + lower opacity.

---

## Roadmap ideas

- “Balanced mode” (apply blended strips on both sides for less bias)
- Optional seam-band repair for structured textures
- Optional rectangular textures (non-square output)

---

## License

MIT — see [LICENSE](LICENSE).

---

## Author

**Lel Beljaev**  
webvrdev.com
