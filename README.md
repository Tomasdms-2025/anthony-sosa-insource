# Anthony Sosa — Insource (one-page site)

Static one-page website for Anthony Sosa, MA, LPCC (Insource, Denver).

Recovered on 2026-10-19 from the live Vercel deployment
(`https://anthony-sosa-insource.vercel.app/`) after access to the original repo was lost.
The live site was plain hand-written HTML (no framework, no build step), so every file in
`site/` is a byte-for-byte copy of what Vercel was serving.

## Layout

```
site/                  <- the whole website; this folder is what gets hosted
  index.html           page markup, all CSS (inline <style>) and the animation script (inline <script>)
  privacy.html         privacy page (linked from the footer)
  404.html             custom not-found page
  robots.txt, sitemap.xml
  img/                 10 images (photos, og-image, favicon)
  js/                  vendored libraries: GSAP 3.13.0, ScrollTrigger, Lenis 1.3.26 (smooth scroll)
```

Fonts load from external CDNs (Google Fonts: Fraunces + Pinyon Script; Fontshare: Satoshi).

## Run locally

```bash
python3 -m http.server 8411 --directory site
```

Then open http://localhost:8411.

## Deploy (Cloudflare Pages)

No build step. Framework preset: **None**, build command: *(empty)*, output directory: **`site`**.
Or direct upload: `npx wrangler pages deploy site --project-name <name>`.

Before launch on a real domain, replace `YOUR-DOMAIN` in `site/sitemap.xml` and add the
`Sitemap:` line to `site/robots.txt` (both files carry a note saying so). The `og:image`
tags use a relative path (`img/og-image.jpg`); some social previews need an absolute URL,
so switch it to `https://<domain>/img/og-image.jpg` once the domain is known.
