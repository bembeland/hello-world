# hello-world
learning

## Premier League xG Distribution Curve (PWA)

Open `index.html` in a browser (or serve the folder, e.g. `python3 -m http.server 8000`).

- League-wide Premier League 2026-27 xG scored/conceded distribution, GW1-38 (actuals GW1-11, projections GW12-38), with bell curve and Fourier smoothing/projection layers.
- **Club filter:** pick any of the 20 clubs in the "Club filter" section to see its weekly GW12-38 predictions - predicted xG for/against, most likely score, win/draw/loss probabilities and expected points, based on GW11 Opta attack/defence strengths, venue and the Fourier league wave.
- **Install as an app (PWA):** open the served page in Chrome/Edge/Android or Safari, then "Add to Home Screen" / use the in-page Install button when offered. It works offline after the first load (`sw.js` caches the app shell; your last selected club is remembered).

Files: `index.html` (app), `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`.
