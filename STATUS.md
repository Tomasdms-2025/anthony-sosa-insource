---
updated: 2026-10-19
status: active
---

# STATUS — anthony-sosa-insource

## Where we are
- Site recovered from the live Vercel URL on 2026-10-19 (original repo lost). All 17 files pulled; local copy verified identical to live.
- Local git repo only. No GitHub remote yet. Not deployed anywhere new yet.

## What's next
- [ ] Decide: create private GitHub remote (`Tomasdms-2025/anthony-sosa-insource`)?
- [ ] Decide: deploy target (Cloudflare Pages) and the real domain.
- [ ] On launch: fill `YOUR-DOMAIN` in `site/sitemap.xml`, add `Sitemap:` to `site/robots.txt`, make `og:image` absolute.

## How to run
`python3 -m http.server 8411 --directory site` → http://localhost:8411
