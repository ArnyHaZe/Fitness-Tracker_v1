# Fitness Tracker v1

A modern, installable Progressive Web App (PWA) for tracking a complete 26-week strength and body recomposition program.

Fitness Tracker v1 is built as a lightweight browser-based app using HTML, CSS, and JavaScript. It stores training data locally on the device, supports offline use after the first load, and can be installed on a phone home screen like a native app.

## Live App

After GitHub Pages is enabled, the app should be available at:

https://ArnyHaZe.github.io/Fitness-Tracker_v1/

## Features

- 26-week strength and recomposition program
- Weekly cut / bulk phase toggle
- Workout logging for weight, reps, and RPE
- Suggested loads based on previous sessions
- Exercise swaps
- Rest timer
- Weekly body-weight check-ins
- Progress charts powered by Chart.js
- Local-first saving with browser localStorage
- Installable mobile app experience
- Offline support through a service worker
- No account required
- No server or database required

## Installation

### iPhone

1. Open the live app in Safari.
2. Tap the Share button.
3. Tap **Add to Home Screen**.
4. Enable **Open as Web App**.
5. Tap **Add**.

### Android

1. Open the live app in Chrome.
2. Tap the menu button.
3. Tap **Install app** or **Add to Home screen**.
4. Confirm installation.

### Desktop

Open the live app in a modern browser. Some browsers also offer an install button in the address bar.

## Privacy

Fitness Tracker v1 is local-first.

- No user account is required.
- No workout data is uploaded.
- No analytics or tracking scripts are included.
- All logged data is stored in the browser on the device being used.

Clearing browser data may delete saved progress.

## Offline Support

The app includes a service worker (`sw.js`) that caches the core app files after the first visit. This allows the app to keep opening even when the device is offline.

When publishing a new app version, update the cache version inside `sw.js` so installed devices fetch the latest files.

Example:

```js
const CACHE_VERSION = "fitness-v2";
```

## Project Structure

```text
.
├── index.html
├── manifest.json
├── sw.js
├── apple-touch-icon.png
├── icon-512.png
├── README.md
├── CHANGELOG.md
├── PRIVACY.md
├── SECURITY.md
├── LICENSE
└── .gitignore
```

## Deployment with GitHub Pages

1. Go to repository **Settings**.
2. Open **Pages**.
3. Set source to **Deploy from a branch**.
4. Select branch **main**.
5. Select folder **/(root)**.
6. Click **Save**.

After a short delay, GitHub Pages will show the public URL.

## Built With

- HTML5
- CSS3
- Vanilla JavaScript
- Chart.js
- Web App Manifest
- Service Worker API
- Browser localStorage

## Roadmap

Potential future improvements:

- CSV export and import
- Manual backup file download
- Multiple profile support
- Exercise images or videos
- Better update notification when a new service-worker version is available
- Optional cloud sync
- Apple Health / Google Fit integration

## Version

Current version: **v1.0**

## License

MIT License. See [`LICENSE`](LICENSE).
