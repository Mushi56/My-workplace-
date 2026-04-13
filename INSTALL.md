# Viratmas Payroll — Install as App (Chrome)

## Files needed (keep all in same folder)
- `viratmas-payroll-4.html` — Main app
- `manifest.json` — PWA manifest
- `sw.js` — Service worker (offline support)
- `icon-192.png` — App icon
- `icon-512.png` — App icon (large)

## How to install on Android / Chrome Desktop

### Option A — Host locally with a simple server
```bash
# In the folder with all files, run:
python3 -m http.server 8080
# Then open: http://localhost:8080/viratmas-payroll-4.html
```
Chrome will show an **"Install"** banner or you can tap the ⋮ menu → **"Add to Home Screen"**

### Option B — Host on GitHub Pages (free)
1. Create a free GitHub repo
2. Upload all 5 files
3. Enable GitHub Pages (Settings → Pages → main branch)
4. Open the URL in Chrome → install from there

### Option C — Use any web host
Upload all 5 files to the same folder on any web server (must be HTTPS for full PWA).

## Offline Support
Once installed, the app works fully offline — all data is stored locally in the browser.

## Notes
- The install banner appears automatically in Chrome when the app meets PWA criteria
- On iOS Safari: tap Share → "Add to Home Screen" manually
- Data is stored per-browser; clearing browser data will reset it
