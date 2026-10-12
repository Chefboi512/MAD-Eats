# MAD Eats

Static website for **MAD Eats** — a smash burger / smokie / poutine food cart on Norcross Rd in Duncan, BC.

- Live site: https://madeatsfoods.com
- Order on DoorDash or pull up to the cart.

## Stack

Pure static HTML + CSS + vanilla JS. No build step required. Fonts are pulled from Google Fonts.

## Local preview

Any static server works. Easiest:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Deployment

Hosted on **Cloudflare Pages** from this repository (`main` branch).

| Setting       | Value |
|---------------|-------|
| Framework     | None (static) |
| Build command | _(empty)_ |
| Build output  | `/` (repository root) |
| Root directory| `/` |

After the first deploy, point your custom domain `madeatsfoods.com` at the Pages project in the Cloudflare dashboard.

## Files of note

- `index.html` — the entire site (single-page)
- `logo.png`, `og-card.png`, `icon-192.png`, `apple-touch-icon.png`, `favicon-48.png`, `favicon.ico` — branding / social-share assets
- `robots.txt`, `sitemap.xml` — SEO
- `_headers` — Cloudflare Pages caching rules

## Updating

Edit the files in this repo, commit, and push to `main`. Cloudflare Pages will redeploy automatically.
