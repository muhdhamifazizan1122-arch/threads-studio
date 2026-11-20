THREADS STUDIO MOBILE V3

Files: index.html, server.js, manifest.json, sw.js

Requires Node.js 18+ and an OpenAI API key.

Setup:
1. Extract all files into a folder.
2. npm init -y
3. npm install express
4. Set API key securely:
   macOS/Linux: export OPENAI_API_KEY="YOUR_KEY"
   Windows PowerShell: $env:OPENAI_API_KEY="YOUR_KEY"
5. node server.js
6. Open http://localhost:3000

For mobile access/PWA:
Deploy this folder on a Node-capable host with HTTPS (Render/Railway/etc).
Set OPENAI_API_KEY as a server environment secret, not in HTML.
Then open deployed HTTPS URL on your phone and use browser menu Add to Home Screen.

Features:
- Mobile-first layout and bottom navigation
- Attempts product metadata detection via server
- AI-generated 3 copy variations (main/reply1/reply2)
- Copy controls and local history (localStorage)
- PWA manifest and service worker shell cache

Link scraping is best-effort; marketplace sites may block requests, redirects or metadata. A production server should have stronger SSRF protections, rate limiting, and host-level egress controls before public use. API calls incur OpenAI charges.
