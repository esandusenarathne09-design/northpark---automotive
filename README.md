# Northpark Automotive — Website

A fast, mobile-friendly, single-page website for **Northpark Automotive** (Somerton VIC).
Built with plain HTML, CSS and JavaScript — no build step, no paid services, deploys free on Vercel.

## What's included

- Hero with booking/call CTAs and 5.0★ Google rating badge
- About, Services (log book servicing + general repairs), Why Choose Us
- Photo gallery with lightbox
- Real Google reviews section
- Booking enquiry form (phone-first: collects details, then prompts a call to confirm)
- Contact section with address, hours and embedded Google Map
- SEO: meta tags, Open Graph, LocalBusiness (AutoRepair) schema, sitemap, robots.txt
- Fully responsive, scroll animations, "Open now" live badge, mobile call button

## Deploy free on GitHub + Vercel (5 minutes)

1. **Create a GitHub repo** at [github.com/new](https://github.com/new) — name it e.g. `northpark-automotive`, set to **Public**.
2. **Upload these files** to the repo (drag & drop the whole `northpark-automotive` folder contents into the repo root, then commit).
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
| Opening hours | `index.html` (Contact + hero + footer), `js/main.js` (`HOURS` object), and the JSON-LD schema in `index.html` |
| Photos | Replace files in `images/` keeping the same names (`hero.jpg`, `about.jpg`, `gallery-1.jpg` … `gallery-4.jpg`). For best results use landscape photos under ~300 KB each. |
| Services | Edit the Services section in `index.html` |
| Phone / address | Search the project for `0433 042 518` / `+61433042518` / `23 North Park Dr` and replace |

## Optional upgrade: email booking form (free)

The booking form currently works phone-first (no backend needed). If you'd like submissions emailed to you instead, use **Formspree** (free tier):

1. Create a free form at [formspree.io](https://formspree.io) and copy your endpoint (e.g. `https://formspree.io/f/xxxxxxx`).
2. In `index.html`, set the form to `<form id="bookingForm" action="https://formspree.io/f/xxxxxxx" method="POST">`.
3. In `js/main.js`, inside the submit handler, replace the success-panel code with a `fetch()` POST to the same endpoint, then show the success panel.

## Tech notes

- No frameworks or build tools — just open `index.html` in a browser to preview.
- Fonts load from Google Fonts; everything else (images, CSS, JS) is local for speed.
- Colours: red `#E10600`, black `#0B0B0C`, white — defined as CSS variables in `css/styles.css`.
