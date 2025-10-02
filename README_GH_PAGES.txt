# HEC Site — GitHub Pages

This folder contains a static site split into two files:

- `index.html` (or `index_auto.html`): the main page
- `map.html`: the Folium/Leaflet map

## Deploy

### Option A: Project Pages (recommended)
1. Create a repo (or use existing).
2. Put both files at repo root: `index.html` and `map.html`.
3. Settings → Pages → Source: Deploy from a branch → `main` → `/root`.
4. Visit `https://<user>.github.io/<repo>/`.

### Option B: `/docs` folder
1. Put both files inside `/docs` (`/docs/index.html`, `/docs/map.html`).
2. Settings → Pages → Source: `main` → `/docs`.
3. Visit the Pages URL.

### If your map 404s
- Ensure `map.html` is in the same folder as `index.html` (or `docs` if using docs).
- Use `index_auto.html` which includes a small script that tries to auto-detect the correct `map.html` path.
- Confirm file name is exactly `map.html` (case-sensitive).
- Confirm the branch and folder you selected in Pages actually contain `map.html`.
