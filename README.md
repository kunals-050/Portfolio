# Kunal Singh Bidawat — Data Analytics Portfolio (v15)

Plain HTML/CSS/JS. No build step, no backend. Single-page portfolio with cinematic intro, Signal Room data theatre, projects, playground, and certificates.

## Run
- Open `index.html` directly, or serve the folder: `python3 -m http.server 8000` then visit http://localhost:8000
- Deploy: upload the whole folder (keep `vendor/` and `kunal-profile.jpeg`) to GitHub Pages, Netlify, Cloudflare Pages or any static host. Keep relative paths intact.

## What changed in v15
- **Writing / Blog feature fully removed** — section, nav link, hero CTA, Blogger feed loader, related CSS and JS. No residual blog references.
- **Cinematic intro sound** — “Enter with Sound” control on the intro screen unlocks the Web Audio API from a real user gesture, then plays a soft 3–5 s atmospheric sequence (deep pad, rising sweep, glass notes, warm resolve). Quiet enter option remains.
- **Master sound toggle** in the nav works for the rest of the visit. Sound defaults OFF and is never persisted across visits.
- **Interaction sounds** (synthesized only, no external audio files): muted nav clicks, Signal Room entrance scanning motif when the section becomes visible, restrained metric ticks, gentle contact confirmation.
- **Signal Room** entrance sound fires only once when visible and audio is enabled; enabling sound later still allows the entrance sequence if not yet heard.
- Intro skip/enter buttons now have working JS handlers (previously only CSS failsafe existed).

## Design notes
- Dark cinematic aesthetic, animations, profile photo, project cards, certificates and playground behaviour preserved.
- No new external libraries or large audio assets.
- Respects `prefers-reduced-motion` for the intro motif.
- AudioContext is created/resumed only after an explicit gesture; autoplay is never attempted.

## Third-party
sql.js (MIT) — see `vendor/sql.js-LICENSE.txt`.
