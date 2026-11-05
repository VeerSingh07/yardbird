# Yardbird – Homepage Design (Phase 1)

Static HTML/CSS/JS. No build step. Fonts load from Google Fonts.

## Structure
- `index.html` – homepage (all CSS and JS inline)
- `vercel.json` – clean URLs, security headers, long cache for `/assets`
- Put images in `/assets` (e.g. `/assets/hero.jpg`) and reference them as `/assets/...`

## Deploy to Vercel (GitHub)
1. Create an empty GitHub repo, then from this folder run:
   ```
   git init && git add . && git commit -m "Yardbird homepage design"
   git branch -M main
   git remote add origin https://github.com/<you>/yardbird-site.git
   git push -u origin main
   ```
2. In Vercel: Add New > Project > import the repo.
3. Framework Preset: **Other**. Build Command: leave empty. Output Directory: leave empty (root).
4. Deploy. Every push to `main` redeploys; other branches get preview URLs.

## Deploy with the CLI
```
npm i -g vercel
vercel --prod
```
