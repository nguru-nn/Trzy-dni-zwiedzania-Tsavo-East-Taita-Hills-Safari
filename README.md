# Diani Beach → Tsavo East & Taita Hills: 3-Day Safari Map
 
This is an interactive 3D map of a 3-day road safari from **Diani Beach** on Kenya's south coast. Day 1 is a game drive across **Tsavo East National Park** to Voi Safari Lodge. Day 2 continues to the **Taita Hills Wildlife Sanctuary** for a night at the iconic **Salt Lick Safari Lodge**, where the rooms stand on stilts above a waterhole that animals visit day and night.
 
🗺️ **See the full itinerary and the live map:**
[Trzy dni zwiedzania – Tsavo Wschód i Taita Hills](https://safarikenia.com.pl/trzy-dni-zwiedzania-tsavo-wschod-taita-hills) on **Safari Kenia**
 
---
 
## The route
 
| Day | Destination | Accommodation |
|-----|-------------|---------------|
| Start | Departure from Diani Beach | — |
| Day 1 | Tsavo East National Park | Voi Safari Lodge |
| Day 2 | Taita Hills Wildlife Sanctuary | Salt Lick Safari Lodge |
| Day 3 | Return to Diani Beach | — |
 
**Day 1:** Diani Beach → Likoni Ferry → Mariakani → Taru → Buchuma (Bachuma) Gate → game drive through Tsavo East → Voi Safari Lodge
**Day 2:** Voi → Mwatate → Taita Hills Wildlife Sanctuary
**Day 3:** Taita Hills → Voi → Mariakani → Likoni Ferry → Diani Beach
 
The interface labels are in Polish, matching the tour page it's embedded on.
 
## Features
 
- **In-park game drive.** Waypoints inside Tsavo East keep the route on the park tracks from Buchuma Gate to Voi instead of the main highway.
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain at 1.5× exaggeration and a tilted camera. The Taita Hills rise sharply above the surrounding Tsavo plains.
- **Road-accurate route.** Each leg is fetched from the Mapbox Directions API (driving profile) and stitched into one line. If a request fails, the map falls back to a straight segment for that leg.
- **Animated route line.** A golden "marching ants" dashed line runs over a soft glow layer.
- **Interactive itinerary panel.** A glassmorphism sidebar lists each day. Clicking a card flies the camera to that lodge and opens its popup.
- **Custom markers.** Gold SVG pins mark the overnight stops. Hidden waypoints shape the route without cluttering the map.
- **Mobile-friendly.** On small screens the sidebar becomes a bottom sheet, and cooperative gestures keep page scrolling smooth.
- **WordPress-ready.** Styles are scoped to a single container, so the code can be pasted into a Custom HTML block.
## Tech stack
 
- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, no build step
- Plus Jakarta Sans (Google Fonts)
## Usage
 
1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own, and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.
To change the route, edit the `itineraryData` array. Entries with `isWaypoint: true` shape the route only. All other entries get a marker and a sidebar card.
 
## About
 
Built for [Safari Kenia](https://safarikenia.com.pl/), which offers Polish-language safari tours and travel guides for Kenya.
 
➡️ [View this Tsavo East & Taita Hills itinerary](https://safarikenia.com.pl/trzy-dni-zwiedzania-tsavo-wschod-taita-hills)
