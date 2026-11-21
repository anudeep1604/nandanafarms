# Nandana Farms – Breathe Green. Grow Wealth.

Static website for Nandana Farms (Tangutoor, near Mokila & Shankarpally, Hyderabad).
Designed by Digital Win (https://digitalwin.in).

## Deploy on Vercel (no coding)
1. Go to https://vercel.com → sign in → **Add New… → Project**.
2. Choose **Upload / drag & drop** (or push this folder to a GitHub repo and import it).
3. Framework preset: **Other**. Build command: *(leave empty)*. Output directory: *(leave empty / root)*.
4. Click **Deploy**. You get a link like `nandana-farms.vercel.app`.

### Deploy with the Vercel CLI (optional)
```
npm i -g vercel
cd nandana-farms
vercel          # preview
vercel --prod   # live
```

## Connect your domain (nandanafarms.com)
Vercel → Project → **Settings → Domains** → add `nandanafarms.com` and `www.nandanafarms.com`,
then add the DNS records Vercel shows at your domain registrar (GoDaddy / Hostinger etc.).

## Before going live
- The site-visit form shows a thank-you message but does **not send data anywhere yet**.
  Connect it to a form service (e.g. Formspree, Web3Forms, Google Sheets) or your CRM:
  in `index.html`, find `vf.addEventListener('submit'` and send the fields there.
- If your domain is not `nandanafarms.com`, update it in `index.html` (canonical & og tags),
  `robots.txt` and `sitemap.xml`.

## Files
- `index.html` – the website
- `images/` – photos, layout, map, share image (og.jpg), app icon
- `favicon.svg`, `404.html`, `robots.txt`, `sitemap.xml`
- `vercel.json` – clean URLs, image caching, security headers
