# Awakening System — Mobile Edition

A free, phone-first Solo Leveling-inspired life quest tracker built with plain HTML, CSS, JavaScript, and a small PWA setup. No framework, paid API, account, or backend is needed.

## Features
- Minimal dark gaming dashboard with rank, level, XP bar, and stat points
- Five default daily quests plus custom quests (10, 20, 35, or 50 XP)
- Claimable XP and level progression
- Streak tracking and achievement milestones
- Browser local-storage saving
- Export/import save backups
- PWA manifest, icon, and offline service worker

## Fastest way to run
1. Extract this ZIP on your phone or computer.
2. Open `index.html` in a modern browser. The core tracker works without a server.
3. For installable/offline PWA support, host the folder on a free static host such as GitHub Pages, Cloudflare Pages, or Netlify. HTTPS is required for service workers.
4. On Android Chrome, open the hosted website, tap the browser menu, and choose **Install app** or **Add to Home screen** (wording can vary).

## Local development
From the extracted folder, if Node.js is installed:
```bash
npx serve .
```
Open the local URL printed by the command. A static server is enough; there is no backend.

## Files
- `index.html` — complete UI and application logic
- `manifest.json` — installable app metadata
- `sw.js` — offline cache
- `icon.svg` — app icon

## Notes
- Progress lives in the browser storage on that device/browser. Export a JSON backup before clearing browser data or changing devices.
- A daily streak advances when the app detects a new date after a day with a claimed quest. If you skip a day, the streak resets.
- This is a fan-inspired personal productivity tool, not an official Solo Leveling product. XP/stats are motivational game mechanics, not real-world measurements.
- Browser notifications are not included in this version; notifications on phones need permission and extra testing.
