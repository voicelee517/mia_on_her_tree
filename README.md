# Bahasa Indonesian Guide — iPhone Installation Guide

## What You Have Now

Your learning app is now a **Progressive Web App (PWA)**. This means:
- ✅ Works on iPhone (home screen app)
- ✅ Works offline (downloads lessons on first visit)
- ✅ Syncs progress across devices
- ✅ No App Store needed
- ✅ Takes 10 seconds to install

---

## How to Deploy (Free Options)

### Option 1: GitHub Pages (Easiest & Free ⭐)

1. **Create a GitHub account** (if you don't have one): github.com
2. **Create a new repository** named `bahasa-indonesian` (make it public)
3. **Upload these files to the repository:**
   - `index.html`
   - `manifest.json`
   - `service-worker.js`
4. **Go to Settings → Pages**
5. **Select "Deploy from a branch" → main branch → root**
6. **Wait 1 minute**, then your app is live at: `https://yourusername.github.io/bahasa-indonesian`

### Option 2: Netlify (Also Free & Easy)

1. Go to **netlify.com**
2. Click "Add new site" → "Deploy manually"
3. Drag and drop your three files
4. Your app is instantly live at a Netlify URL

### Option 3: Vercel (Free)

1. Go to **vercel.com**
2. Click "New Project"
3. Upload your files or connect GitHub
4. Done! Your app is live

---

## How to Install on Your iPhone

### From Safari (2 minutes)

1. **Open Safari** on your iPhone
2. **Go to your app URL** (e.g., `https://yourusername.github.io/bahasa-indonesian`)
3. **Tap the Share button** (square with arrow at bottom)
4. **Scroll down and tap "Add to Home Screen"**
5. **Name it** "Bahasa" (or whatever you like)
6. **Tap "Add"**

✅ Done! The app now appears on your home screen like any native app.

### From Android

1. **Open Chrome** (or your browser)
2. **Go to your app URL**
3. **Tap the menu** (three dots) → "Install app"
4. **Or:** Long-press the browser tab → "Create shortcut"

---

## What Works Offline

Once you've opened the app once:
- All lessons load instantly (no internet needed)
- Your progress saves locally
- You can learn anywhere—plane, subway, WiFi-less cafes

---

## First-Time Setup Checklist

- [ ] Deployed to GitHub Pages, Netlify, or Vercel
- [ ] Verified the app loads in browser
- [ ] Added to iPhone home screen via Safari
- [ ] Tapped on the app icon to confirm it opens
- [ ] Checked offline mode (turn off WiFi, app still works)
- [ ] Completed Lesson 1

---

## If You Want an App Store App Later

If you want to publish to the actual App Store, you'd use:
- **Capacitor** (wraps your web app for iOS/Android)
- **React Native** or **Flutter** (rebuild in native code)
- **Swift** (pure native iOS)

But for now, this PWA works great and updates instantly—no app store waiting period.

---

## Troubleshooting

**"Add to Home Screen" option doesn't appear?**
- Make sure you're on Safari (not Chrome)
- Check that the URL is https:// (not http://)
- Try clearing browser cache and reloading

**Progress doesn't save?**
- Service worker caches after first load (refresh the page)
- Check Safari settings: Settings → Safari → Advanced → JavaScript (must be ON)

**Offline mode not working?**
- Open the app once while online
- Service worker caches after first visit
- Then offline mode works

---

## Updating Your App

To update lessons or fix bugs:

1. **Edit your files locally**
2. **Upload new versions to GitHub/Netlify**
3. **Users see updates within 24 hours** (service worker refreshes)
4. **Or:** Tell users to hard-refresh (`Cmd+Shift+R` or `Ctrl+Shift+R`)

---

## File Structure

```
bahasa-indonesian-guide/
├── index.html              (main app)
├── manifest.json           (app metadata)
├── service-worker.js       (offline support)
└── README.md              (this file)
```

All three files must be in the same folder.

---

## Need Help?

- **Progressive Web Apps**: https://developers.google.com/web/progressive-web-apps
- **Service Workers**: https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API
- **Manifest.json**: https://developer.mozilla.org/en-US/docs/Web/Manifest

---

**Happy learning! Selamat belajar! 🌏**
