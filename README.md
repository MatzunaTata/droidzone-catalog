# struckto.de – public files for the Struckto apps

This public repo is served by GitHub Pages at **https://struckto.de** and is **edited directly here**.

| File | What it is |
|---|---|
| `index.html` | Landing page with all apps |
| `privacy/<app>.html` | Privacy policy per app (German + English), linked from the Play Store listing |
| `img/` | App icons for the landing page |
| `app-ads.txt` | AdMob seller declaration for all apps |
| `vehicles.json` | Vehicle catalog for the fuel app (Spritrechner) |
| `CNAME`, `.nojekyll`, `robots.txt` | GitHub Pages settings |

## Adding an app
1. Icon (512 × 512 PNG) to `img/<app>.png`.
2. Privacy policy as `privacy/<app>.html` – copy an existing one and adapt it to what the app actually does.
3. A card in `index.html`.

## Vehicle catalog (`vehicles.json`)
Makes, models and engine/battery variants, each with a **permanent id**. The fuel app downloads it about once a week
and also ships a bundled copy for offline use (refreshed from here before each release).
- Ids are never changed, reused or removed; outdated entries get `"deprecated": true`.
- Bump `version` on every change – the app only replaces its copy with a newer or equal version.
