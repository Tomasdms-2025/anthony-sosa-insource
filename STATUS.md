---
updated: 2026-10-19
status: active
---

# STATUS — anthony-sosa-insource

## Where we are
- Site recovered from the live Vercel URL on 2026-10-19 (original repo lost). All 17 files pulled; local copy verified identical to live.
- Private GitHub repo: https://github.com/Tomasdms-2025/anthony-sosa-insource
- Live on Cloudflare Pages: https://anthony-sosa-insource.pages.dev (manual deploy, see README). All 18 files verified identical to the original.
- Old Vercel deployment still running, untouched.

## What's next
- [ ] Decide the real domain and attach it to the Pages project.
- [ ] Decide whether to delete the old Vercel deployment.
- [ ] On launch: fill `YOUR-DOMAIN` in `site/sitemap.xml`, add `Sitemap:` to `site/robots.txt`, make `og:image` absolute.

## How to run
`python3 -m http.server 8411 --directory site` → http://localhost:8411
