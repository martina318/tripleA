# Triple A Plus Ecuador

Static site for Triple A Plus Ecuador, exported from the Claude Design project
(`Triple A Plus Ecuador v5.dc.html`) and unpacked into plain files.

Live: https://martina318.github.io/tripleA/

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | The page template (markup + component script) |
| `support.js` | `dc-runtime` — renders the template with React |
| `assets/image-slot.js` | `<image-slot>` custom element used by the template |
| `assets/vendor/` | React 18.3.1 UMD builds, served locally (no CDN) |
| `assets/fonts/` | Hanken Grotesk (woff2) |
| `assets/*.png`, `assets/quito.jpg` | Images |

Everything is static: no build step. Open `index.html` through any HTTP server
to run it locally, e.g. `python3 -m http.server 8080`.

## Deploying

`.github/workflows/pages.yml` publishes the repo root to GitHub Pages on every
push to `main`.
