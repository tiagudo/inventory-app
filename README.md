# Inventory Control PWA

A fully offline-capable QR code inventory system.

## Setup (5 minutes)

### Step 1 — Download jsQR
The app needs the jsQR library (MIT licensed). Download it once:

  https://cdn.jsdelivr.net/npm/jsqr@1.4.0/dist/jsQR.min.js

Save it as `jsqr.min.js` in the same folder as `index.html`.

### Step 2 — Host it (required for camera + offline)
You need HTTPS. Easiest free options:

**Netlify (recommended):**
1. Go to https://netlify.com → sign up free
2. Drag the entire `inventory-pwa` folder onto the Netlify dashboard
3. You get a URL like `https://your-name.netlify.app`

**GitHub Pages:**
1. Create a GitHub repo, push all files
2. Settings → Pages → Deploy from main branch
3. URL: `https://yourusername.github.io/inventory`

**Glitch:**
1. Go to https://glitch.com → New project → Import from GitHub or paste files
2. Instant HTTPS URL

### Step 3 — Open on your phone
Visit your hosted URL in Safari (iOS) or Chrome (Android).

### Step 4 — Add to Home Screen
- **iOS Safari:** Share button (box with arrow) → "Add to Home Screen"
- **Android Chrome:** ⋮ menu → "Add to Home Screen" or "Install app"

The app icon appears on your home screen. From now on it works **fully offline** with camera support.

## Files
- `index.html` — the entire app
- `sw.js` — service worker (offline caching)
- `manifest.json` — PWA metadata (name, icon, theme)
- `icon.svg` — app icon
- `jsqr.min.js` — QR decoder (download separately, see Step 1)

## Features
- Camera QR scanning (rear camera on mobile)
- Check in / Check out tracking
- Add items with name, SKU, category, notes
- Low stock alerts with configurable threshold
- Full activity log with filters
- CSV export
- Persistent local storage (survives offline)
- Dark mode support
