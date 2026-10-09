# Japan Journey 2026

A lightweight, bilingual English/Indonesian travel companion for the Japan trip (12–24 October 2026).

## Files
- `index.html`: interactive itinerary and illustrated route map.
- `manifest.webmanifest`: installable web app metadata.
- `sw.js`: service worker for offline caching when hosted over HTTPS.

## Run locally
Open `index.html` in a modern browser. For PWA/offline behavior, serve the folder over HTTPS or localhost.

## Deploy
Recommended low-cost option: GitHub Pages for this static site. In repository Settings → Pages, choose **Deploy from a branch**, select `main` and `/ (root)`, then save. Vercel is also supported but adds little value for a static HTML/CSS/JS app unless you plan to expand it with server-side features.

## Notes
The illustrated map is conceptual rather than geographically precise. External map links need an internet connection, and transport details are based on the itinerary supplied, not live service data. Unconfirmed itinerary items should remain marked as unconfirmed.
