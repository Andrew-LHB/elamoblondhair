# Elvira Mor — Portland Hair

One-page static website built with Astro. English content, original supplied photography, responsive WebP images, portfolio filters and keyboard-accessible photo dialog.

## Local development

```sh
npm ci
npm run dev
```

## Production

```sh
npm run build
```

Upload `dist/` to a static host. Production domain: `https://emorportlandhair.com`.

## GitHub Pages

Repository: https://github.com/Andrew-LHB/elamoblondhair

Every push to `main` runs `.github/workflows/deploy.yml`, builds the website, and deploys `dist/` to GitHub Pages. The repository Pages settings use GitHub Actions and the custom domain `emorportlandhair.com`.

DNS is managed in Cloudflare. The apex has the four GitHub Pages A records and four IPv6 AAAA records. `www` is a CNAME to `andrew-lhb.github.io`; GitHub redirects it to the apex. These records use DNS only.

## Editing

Copy and contact details: `src/pages/index.astro`. Photos: `src/assets/`. There are no fixed prices; appointments are arranged by phone or SMS. No booking backend is connected.
