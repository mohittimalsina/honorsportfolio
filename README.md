# Mohit Timalsina — Honors Portfolio

Live site files. This folder is fully self-contained: `index.html` + the `images/` folder. Total size ~1 MB.

## Deploy to GitHub Pages

1. Create a repo (e.g. `portfolio`) and upload **the contents of this `docs` folder** to the repo root — so the repo has `index.html`, `images/`, and `.nojekyll` at the top level.
2. Repo → **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Branch: **main**, folder: **/ (root)**. Click **Save**.
5. Wait 1–2 minutes, then refresh. Your site URL appears at the top of the Pages settings.

### Why it wasn't deploying before
- GitHub Pages runs files through Jekyll by default, which can silently fail. The `.nojekyll` file here turns that off so your files are served exactly as-is.
- Pages needs an `index.html` at the root of whatever it's serving. This folder has one.
- The old project had a 14 MB bundled file, original full-res photos, and dev artifacts (~46 MB total) that bloated uploads. None of that is needed — only what's in this folder.

> Note: the page loads React, Babel, and Google Fonts from a CDN, so it needs an internet connection to render (normal for a live web page).
