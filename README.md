# BIRTHZAK — Happy Birthday Website

A self-contained birthday celebration webpage for Firdaus Zaki Ramadhan.

## Files
- `index.html` — the full website (inline CSS, JS, SVG animations, canvas starfield + meteor loop, Web Audio music-box fallback)
- `lagu.mp3` — background song (played via the music player)
- `vercel.json` — Vercel static deployment config (audio MIME + caching headers)

## Deploy to Vercel

### Option A — Vercel CLI (fastest)
```bash
npm i -g vercel
cd birthzak-deploy
vercel          # preview deploy
vercel --prod   # production deploy
```

### Option B — Vercel Dashboard (drag & drop)
1. Zip this folder
2. Go to https://vercel.com/new
3. Drag the zip into the Vercel dashboard
4. Framework Preset: **Other** (auto-detected as static)
5. Click **Deploy**

### Option C — Git repo
1. Push this folder to a GitHub repo
2. Import the repo at https://vercel.com/new
3. Vercel auto-detects it as a static site
4. Deploy

## Notes
- All images load from external CDN (imglinkv-3.vercel.app) — no upload needed
- Google Fonts loaded from CDN
- `lagu.mp3` streamed with Accept-Ranges for seeking
- Fully responsive (mobile 3+2 polaroid grid, desktop row layout)
- No build step required — pure static HTML
