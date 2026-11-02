# Midnight IT website

Static site for midnightit.com.au — 24/7 IT support and managed services, a Code Black Group company.

- `public/index.html` — the home page (desktop + mobile, 3D effects, hero background video)
- `public/assets/` — logo, wordmark, hero video, poster and favicon

Hosted on Render as a static site (publish directory: `public`). Every push to `main` redeploys.

**Before switching the midnightit.com.au domain over:** remove the `<meta name="robots" content="noindex, nofollow">` line in `public/index.html` so search engines can index the new site.
