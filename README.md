# hello-world
learning

## Premier League xG Distribution Curve (PWA)

Open `index.html` in a browser (or serve the folder, e.g. `python3 -m http.server 8000`).

- League-wide Premier League 2026-27 xG scored/conceded distribution, GW1-38 (actuals GW1-11, projections GW12-38), with bell curve and Fourier smoothing/projection layers.
- **Club filter (GW1-38, club-specific):** pick any of the 20 clubs and everything below the selector is that club only. GW1-11 shows its actual result next to a no-peeking backtest prediction (expanding window, prior weeks only) with outcome hit/miss, error size and an investigation tag for big misses (finishing/VAR/red-card/injury/weather checks - tags are prompts to verify in the match report, not confirmed causes). GW12-38 shows predictions (xG for/against, most likely score, W/D/L %, expected points) from GW11 Opta strengths, venue and the Fourier wave, corrected by the club's backtest bias. Backtest summary (hits/11, MAE, biggest miss) is shown per club.
- **Install as an app (PWA):** open the served page in Chrome/Edge/Android or Safari, then "Add to Home Screen" / use the in-page Install button when offered. It works offline after the first load (`sw.js` caches the app shell; your last selected club is remembered).

Files: `index.html` (app), `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`.
