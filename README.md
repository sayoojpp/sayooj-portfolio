# Sayooj — UX Portfolio

A dark, cinematic portfolio site (dark theme + lime accent). Static HTML — no build step.

## Live deployment (GitHub Pages)

1. Create a new GitHub repository (e.g. `sayooj-portfolio`).
2. Upload **everything inside this folder** to the repo root (so `index.html` sits at the top level).
3. In the repo: **Settings → Pages → Build and deployment**.
4. Source: **Deploy from a branch**. Branch: `main` (or `master`), folder: `/ (root)`. Save.
5. Wait ~1 minute. Your site goes live at `https://<your-username>.github.io/<repo-name>/`.

> A `.nojekyll` file is included so GitHub Pages serves every asset as-is.

## Structure

```
index.html                 Home / portfolio
pierce-manufacturing.html  Pierce case study
image-slot.js              Image drop component
tweaks-panel.jsx           Theme tweak panel (editing-only; harmless live)
assets/
  images/portrait.png      Hero + about portrait
  images/pierce-banner.png Pierce project banner
  cv/Sayooj-CV-2026.pdf    Résumé (linked from the Résumé buttons)
  fonts/                   Google Sans variable fonts (self-hosted)
```

## Editing

- **Copy / content:** open the `.html` files and edit the text directly.
- **Résumé:** replace `assets/cv/Sayooj-CV-2026.pdf` (keep the filename, or update the two links).
- **Social links:** search for `href="#"` in `index.html` and drop in your real URLs.
- **Contact email:** search for `hello@sayooj.design` and replace.

## Notes

- React + Babel load from a CDN (used only by the optional tweaks panel) — the site needs internet on first load. To go fully offline-capable, remove those three `<script>` tags and the `tweaks-panel.jsx` tag at the bottom of `index.html`.
- The 3rd and 4th projects are still placeholders — add your own covers and case-study links when ready.
