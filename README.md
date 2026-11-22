# Midnight IT website

Static site for midnightit.com.au — 24/7 IT support and managed services, a Code Black Group company.

- `public/index.html` — the home page (desktop + mobile, 3D effects, hero background video)
- `public/assets/` — logo, wordmark, hero video, poster and favicon

Hosted on Render as a static site (publish directory: `public`). Every push to `main` redeploys.

**Before switching the midnightit.com.au domain over:** remove the `<meta name="robots" content="noindex, nofollow">` line in `public/index.html` so search engines can index the new site.

## Security
Every page carries a Content Security Policy, referrer policy and anti-framing guard (`assets/guard.js`).
The policy pins each inline script by hash, so **after editing any inline `<script>` run `python3 tools/csp.py`**.
