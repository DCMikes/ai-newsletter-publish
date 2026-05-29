# ai-newsletter-publish

Session color: #0EA5E9 (sky)

Public destination for the AI newsletter. This repo holds the **finished, published** newsletter — rendered pages, archives, and anything intended for readers.

The companion **build** repo ([DCMikes/ai-newsletter-build](https://github.com/DCMikes/ai-newsletter-build), private) is where all the source material, drafts, prompts, scripts, and tooling live. Finished output from `build` lands here for public consumption.

## Layout

- `index.html` — perpetual "current edition" link; forwards the Pages root to the newest edition (update on each publish — see build PROCESS.md §6.1)
- `README.md` — public archive index (full editions table)
- `AI-Signal-Edition-{NNN}-{YYYY-MM-DD}.md` / `.html` — editions at the top level, each in both formats (same content; HTML is the dark-themed long-form rendering)
- `favicon.svg`, `favicon-16.png`, `favicon-32.png`, `favicon.ico`, `apple-touch-icon.png` — site icon (the AI Signal broadcast-arc mark; regenerated from the build repo's `tools/make_favicon.py`)

## GitHub Pages

This repo is served via GitHub Pages from the `main` branch root. Pushing to `main` deploys.
