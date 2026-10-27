# Still Point: press handstand trainer
Guided workouts and progress tracking for the 16-week press handstand plan. It is a single-file web app that installs to your phone's Home Screen and works offline.

## Install on your phone
1. Open **https://studiowild.github.io/press-handstand-trainer/** in Safari on iPhone, or Chrome on Android.
2. **iPhone:** tap Share → **Add to Home Screen**. **Android:** tap ⋮ → **Install app**.
3. Launch Still Point from the Home Screen. It opens full screen and works without a connection.

Your log is stored on the phone. To keep a backup or move to a new phone, use **Preferences → Your data → Export**. On a new phone, choose **Restore from a backup** on the welcome screen, or **Import** in Preferences.

## Files
- `index.html`: the whole app (markup, styles, script)
- `manifest.webmanifest` and `icons/`: Home Screen install
- `sw.js`: offline cache. Bump `VERSION` on each deploy so installed apps refresh.

## Deploy
GitHub Pages serves the repo root from `main` (Settings → Pages → Deploy from a branch → `main` / root). Any static host works too, for example Netlify Drop: drag the folder onto https://app.netlify.com/drop.

Run it locally with `python3 -m http.server` and open http://localhost:8000. Add `?dev` to the URL for dev controls.
