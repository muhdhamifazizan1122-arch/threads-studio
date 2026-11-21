THREADS STUDIO MOBILE V5

Files: index.html, server.js, manifest.json, sw.js

V5 features:
- 3 distinct copywriting variations with angle labels
- Post utama + Reply 1 benefit + Reply 2 CTA
- SEO keyword phrases and hashtags per variation
- Copy individual section or copy complete variation
- Mobile/PWA, history saved locally in browser
- Product metadata detector (may be blocked by marketplaces)

Deploy on Railway:
1. Replace index.html and server.js in GitHub repository with these V5 versions. Keep manifest.json and sw.js (or replace them too).
2. Railway redeploys from GitHub when integration is working. If not, manually redeploy latest deployment.
3. Keep OPENAI_API_KEY in Railway Variables only; do not add it to GitHub or frontend.
4. PORT is read from process.env.PORT, with fallback 8080.

No API key is included in this package.


MODULE BARU V5: Organic & Engagement Studio. Pilih niche, audience dan fokus (idea 7 hari, conversation, engagement, poll, storytelling, edukasi, komuniti atau calendar), kemudian generate 7 item. Endpoint tambahan /api/organic.
