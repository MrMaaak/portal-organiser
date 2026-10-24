# TMT Portal Organiser

A folder view over everything in the tmt.maps.arcgis.com portal, whoever owns it.

Live at https://mrmaaak.github.io/portal-organiser/ (published by GitHub Pages on every push to `main`).

- Sign in with your ArcGIS account. You only see items you already have access to.
- Folders are stored in one ArcGIS item, "TMT Portal Organiser – folder map", which is shared with the organisation so everyone sees the same folders. Its owner and admins can change them; everyone else can browse.
- Filing an item only updates the folder map. Nothing in ArcGIS Online moves, changes owner or changes sharing.

## Sign-in setup

The page uses the "TMT Portal Organiser" OAuth credentials in ArcGIS Online (App ID in `index.html`). Every address the page is opened from must be listed under its Redirect URLs:

- `https://mrmaaak.github.io/portal-organiser/`
- `http://localhost:8765/` (local testing)

## Running locally

```bash
python -m http.server 8765 --bind 127.0.0.1
```
