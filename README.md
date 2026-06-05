# Workout Tracker PWA

A personal workout tracker for gym, calisthenics, running and cycling.

## Files

- `index.html` — the entire app
- `manifest.json` — PWA config (name, icon, display mode)
- `sw.js` — service worker (offline support)
- `icon-192.png` / `icon-512.png` — app icons (replace with your own!)

---

## Deploy to Netlify (easiest, 2 minutes)

1. Go to [netlify.com](https://netlify.com) and create a free account
2. On the dashboard, find the **"Sites"** section
3. Drag the entire `workout-pwa` folder onto the page
4. You get a URL like `https://random-name-123.netlify.app`
5. Done!

To rename it: Site settings → Domain management → change site name → `https://yourname.netlify.app`

---

## Deploy to GitHub Pages (free, keeps version history)

1. Create a free account at [github.com](https://github.com)
2. Create a new repository, call it `workout` (or anything)
3. Upload all 5 files (drag & drop in the GitHub UI)
4. Go to Settings → Pages → Source: "Deploy from branch" → branch: `main`, folder: `/ (root)`
5. Your app is live at `https://yourusername.github.io/workout`

---

## Install to iPhone home screen

1. Open your app URL in **Safari** (must be Safari, not Chrome)
2. Tap the **Share** button (box with arrow pointing up)
3. Scroll down and tap **"Add to Home Screen"**
4. Name it "Workouts" or whatever you like → tap **Add**

It will now appear on your home screen like a native app, launch full-screen, and work offline.

---

## Customising the app

Everything is in `index.html`. Key things you might want to change:

- **Add exercises to the dropdown**: search for `<optgroup label="Gym">` and add `<option>Your exercise</option>`
- **Change the app name**: edit `manifest.json` → `"name"` and `"short_name"`
- **Change colors**: look for the `:root {` block near the top of the `<style>` section
- **Add new activity types**: search for `setType` in the JS

The app stores all data in your browser's localStorage — it never leaves your device.

---

## Replace the icons

The included icons are minimal placeholders (black squares). To replace:
- Create a 192×192px and 512×512px PNG image
- Name them `icon-192.png` and `icon-512.png`
- Re-upload/re-deploy

Free icon generators: [favicon.io](https://favicon.io) or [realfavicongenerator.net](https://realfavicongenerator.net)
