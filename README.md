# Japan Journey 2026

A bilingual (English / Indonesian), mobile-friendly travel companion for the Japan trip, 12–24 October 2026.

## App features
- Daily itinerary for October 12–24
- Detailed routes, transit lines, stop counts and approximate journey times transcribed from the supplied itinerary PDF
- Accommodation addresses, sightseeing stops, food ideas and travel notes
- English / Indonesian toggle
- Google Maps search links
- Responsive design and small animated train illustration
- Service-worker caching for offline access after the site has loaded once

## Source and accuracy
The original itinerary PDF is the source of truth. Transport times, fares, opening hours, platforms and routes are transcribed notes, not live data, and can change. Verify important connections and reservations with official operators before travel. Ideas explicitly marked unconfirmed are not confirmed bookings or final plans. In particular, the October 18 Osaka plan is unfinished and Kawaguchiko sightseeing on October 19 is undecided.

## Run locally
Open `index.html` in a modern browser. For service-worker/PWA behavior, serve the folder over HTTPS or localhost.

## Hosting
The site is designed for GitHub Pages. In Settings → Pages, choose **Deploy from a branch**, branch `main`, folder `/(root)`. Each commit to `main` triggers a new deployment.

## Files
- `index.html`: app UI, styling, itinerary data and interactions
- `manifest.webmanifest`: installable web app metadata
- `sw.js`: service-worker caching


## Travel-first navigation update
- Refined hand-drawn-style hero into a crisp, scalable inline SVG vector illustration.
- Every itinerary item has one-tap Google Maps directions, a Google Drive search shortcut for that date/item, and an operator timetable link.
- Common Japanese station names are shown in kanji alongside English names to help match station signs.
- Timetable links point to official operator pages where available: JR East, JR Central Tokaido Shinkansen, Tokyo Monorail, Kintetsu, and Fujikyu City Bus.
- The app does not embed guaranteed departure times or live disruption data. Use the linked timetable/route planner for the actual date, and confirm platform and service on the day. Drive buttons search the signed-in user's Drive; they do not grant access to files.
