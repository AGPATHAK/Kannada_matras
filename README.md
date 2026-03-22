# Kannada Matras

Static GitHub Pages package for the embedded-data Kannada Matras app.

## Files
- `index.html` – main app file
- `manifest.json` – installable web app metadata
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `favicon.png` – app icons
- `kannada_matra_master_v6_1.csv` – optional source deck reference; the app does **not** require this to run because the default deck is already embedded in `index.html`
- `.nojekyll` – avoids GitHub Pages processing quirks

## Publish on GitHub Pages
1. Create a new GitHub repository.
2. Upload all files from this folder to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` (or `master`) and `/ (root)`
5. Save. GitHub will generate a Pages URL.
6. Open that URL on your iPhone and add it to the Home Screen from Safari.

## Local use
- You can open `index.html` directly on your Mac by double-clicking it.
- The built-in deck is included in the HTML, so no CSV selection is required.
- The CSV picker remains available only as an optional override.
