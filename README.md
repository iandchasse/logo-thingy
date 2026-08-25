# de-link — page mark studio

A single-page, dependency-free studio for designing and exporting the **de-link** wordmark. Resize it, swap the typeface, tune the icon, and export finished files.

**Live site:** once GitHub Pages is enabled (see below), it will be served at
`https://iandchasse.github.io/logo-thingy/`.

## Features

- **20 typefaces** (loaded from Google Fonts) with a live preview.
- Four lockups: icon left, icon above, in-word, and mark only.
- Sliders for mark size, gap, line weight, and roundness; toggles for broken line, theme, and construction guides.
- **Dark UI by default.**
- **Export the full lockup** as high-res light PNG, dark PNG, or vector SVG.
- **Export the mark on its own** (separate light PNG, dark PNG, and SVG).
- Export/import a `config.json` to save and restore an exact design.
- Your last settings are remembered automatically in your browser.

## Run locally

It's a static file — just open `index.html`, or serve the folder:

```bash
python3 -m http.server
# then visit http://localhost:8000
```

## Hosting on GitHub Pages

**Option A — deploy from a branch (simplest):**
Repo **Settings → Pages → Build and deployment → Source: “Deploy from a branch”**,
pick the branch and `/ (root)`, then **Save**. The site publishes at the URL above.

**Option B — GitHub Actions:**
Set **Settings → Pages → Source: “GitHub Actions”**. The included
`.github/workflows/deploy-pages.yml` then publishes the site on every push to the
default branch.
