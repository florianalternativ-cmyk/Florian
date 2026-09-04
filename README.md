# Florian — Portfolio

Single-file static site: `index.html`. No build step, no dependencies.

## Deploy (GitHub Pages)
1. Create a repo named `florianalternativ-cmyk.github.io` (or any repo + enable Pages on `main`).
2. Commit `index.html` to the root.
3. Settings → Pages → Source: `main` / root. Done.

## Before publishing
- Replace the two placeholder hrefs in the Contact section (`YOUR-HANDLE`) with your LinkedIn and Instagram URLs.
- Optional: change the `Source on GitHub` link in the PhysicsLab card if the repo name differs.

## Editing copy
All text lives twice: in the HTML (English, as fallback) and in the `I18N` object at the bottom of the file (`en` and `de`). Edit both, or only the `I18N` object — it overrides the HTML on load.

## Design notes
- Fonts: Fraunces (headings) + Inter (body) via Google Fonts, with Georgia / system-ui fallbacks.
- Skills section pins on desktop and scrolls horizontally with the page; on narrow screens or with `prefers-reduced-motion` it falls back to a native swipeable row.
- Language preference is persisted in `localStorage`; first visit defaults to the browser language.
