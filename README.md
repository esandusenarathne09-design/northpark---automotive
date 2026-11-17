# Northpark Automotive — Website

A fast, mobile-friendly, single-page website for **Northpark Automotive** (Somerton VIC).
Built with plain HTML, CSS and JavaScript — no build step, no paid services, deploys free on Vercel.

> **Important:** All files live in ONE folder (no subfolders). When uploading to GitHub,
> upload the files exactly as they are — `index.html`, `styles.css`, `main.js`, the
> `.webp` photos, `favicon.svg`, `robots.txt`, `sitemap.xml`. Do not create folders.

## What's included

- Hero with booking/call CTAs and 5.0★ Google rating badge
- About, Services (log book servicing + general repairs), Why Choose Us
- Photo gallery with lightbox
- Real Google reviews section
- Contact section with address, hours and embedded Google Map
- SEO: meta tags, Open Graph, LocalBusiness (AutoRepair) schema, sitemap, robots.txt
- Fully responsive, scroll animations, "Open now" live badge, mobile call button

## Deploy free on GitHub + Vercel (5 minutes)

1. **Create a GitHub repo** at [github.com/new](https://github.com/new) — name it e.g. `northpark-automotive`, set to **Public**.
2. **Upload these files** to the repo root (drag & drop all files, then commit).
3. **Deploy on Vercel**: go to [vercel.com/new](https://vercel.com/new) → sign in with GitHub → **Import** the repo.
   - Framework preset: **Other**
   - Root directory: `./`
   - Build command: *(leave empty)* · Output directory: *(leave empty)*
4. Click **Deploy**. Your site is live at `https://northpark-automotive.vercel.app` (free subdomain).
5. Update the canonical URL in `index.html`, `robots.txt` and `sitemap.xml` if Vercel gives you a different subdomain.

Every push to GitHub redeploys automatically. Total cost: **$0**.

## Updating the site

| What | Where |
|---|---|
| Opening hours | `index.html` (Contact + hero + footer), `main.js` (`HOURS` object), and the JSON-LD schema in `index.html` |
| Photos | Replace the `.webp` files keeping the same names (`workshop-interior.webp`, `workshop-exterior.webp`, `services-card.webp`, `northpark-logo.webp`) |
| Services | Edit the Services section in `index.html` |
| Phone / address | Search the project for `0433 042 518` / `+61433042518` / `23 North Park Dr` and replace |

## Tech notes

- No frameworks or build tools — just open `index.html` in a browser to preview.
- Fonts load from Google Fonts; everything else (images, CSS, JS) is local for speed.
- Colours: red `#E10600`, black `#0B0B0C`, white — defined as CSS variables in `styles.css`.
