# Shopfront

Marketing site for a website-repair service aimed at small businesses.

Static, single page, no build step and no dependencies. `index.html` carries its
own CSS and a small amount of vanilla JavaScript for the scroll reveals.

## Running it locally

    python -m http.server 8000 --directory .

## Deploying

Any static host will serve this correctly. `vercel.json` sets security headers
and clean URLs; nothing else is required.

## Before it goes live

- `hello@shopfront.example` is a placeholder. Replace it in `index.html`
  (the mailto: link and the JSON-LD block) with a real address.
- Replace `https://shopfront.vercel.app` in `index.html`, `robots.txt` and
  `sitemap.xml` with the real domain once it is assigned.
- Prices are in USD.

## Checking your own work

The site is audited by the same scanner it advertises:

    python ../leadmagnet/audit.py <your-domain>

It should come back clean. If it does not, fix that before sending the report
to anyone else.
