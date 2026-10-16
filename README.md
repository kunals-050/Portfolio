# Kunal Singh Bidawat — Data Analytics Portfolio (v15)

Plain HTML/CSS/JS. No build step, no backend. Single-page portfolio with cinematic intro, Signal Room data theatre, projects, playground, and certificates.

## Run
- Open `index.html` directly, or serve the folder: `python3 -m http.server 8000` then visit http://localhost:8000
- Deploy: upload the whole folder (keep `vendor/` and `kunal-profile.jpeg`) to GitHub Pages, Netlify, Cloudflare Pages or any static host. Keep relative paths intact.

## What changed in v15
- **Writing / Blog feature fully removed** — section, nav link, hero CTA, Blogger feed loader, related CSS and JS. No residual blog references.
- Intro skip/enter buttons now have working JS handlers (previously only CSS failsafe existed).

## Design notes
- Dark cinematic aesthetic, animations, profile photo, project cards, certificates and playground behaviour preserved.
- Respects `prefers-reduced-motion` for the intro motif.

## Third-party
sql.js (MIT) — see `vendor/sql.js-LICENSE.txt`.
