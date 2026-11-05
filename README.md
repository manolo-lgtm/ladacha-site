# La Dacha de los Pijíos — ladacha.ec

Static site for La Dacha (Guayaquil, Ecuador). Single page, Next.js static export
originally built in ChatGPT Sites and migrated here on 2026-11-05.

## Layout
- `index.html` — the whole site (sections are `#inicio`, `#experiencias`, `#bienestar`, `#eventos-privados`, `#visita`, `#papagayo-y-pijios`, `#membresia`, `#emblema`, `#contacto`). ES/EN toggle is client-side.
- `_next/static/` — built CSS/JS bundles (don't hand-edit; content lives in `index.html`).
- `images/`, `docs/` — media and the Sembrando Paz PDF.

## Deploy
Cloudflare Pages, connected to this repo. Every push to `main` deploys to ladacha.ec.
No build step: output directory is `/` (repo root).

## Editing rule
Edit only the file that changes (usually `index.html` text or an image under `images/`), commit, push.
