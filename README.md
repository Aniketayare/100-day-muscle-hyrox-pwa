# 100-Day Shinobi Journey PWA V4

Attendance-first 100-day muscle + HYROX tracker.

## What changed
- Naruto/Shippuden-inspired motivational milestone system.
- Real character portraits loaded from the Jikan/MyAnimeList character image data at runtime and cached locally after first load.
- Current level shows a character portrait; next level shows the upcoming character portrait.
- 3-row connected chakra/Rasengan-style milestone pipe: only blue chakra balls appear on the journey path.
- Cleaner mobile-first dashboard focused on attendance, streak and completed days.
- No "Start Workout" action on the home dashboard.
- Daily action is simply "Mark Today as Attended".
- Schedule categories corrected:
  - Upper Body Strength → Calisthenics
  - Calisthenics Skills → Calisthenics
  - Leg Strength → Gym
  - Plyometric + Knee Rehab → Calisthenics
  - HYROX Conditioning → Gym
  - Cardio / Run → Gym
  - Rest → Rest
- Existing `localStorage` key `m100` is preserved, so existing attendance data can continue to work.

## Images
Character images are fetched from Jikan's public API (MyAnimeList-derived data) and cached in the browser. Internet access is needed the first time character portraits are loaded; the app keeps cached images where the browser/service worker allows.

## GitHub Pages
Upload/replace:
- `index.html`
- `manifest.json`
- `sw.js`
- `icon.svg`

Then GitHub Pages will publish the updated PWA from the main branch.
