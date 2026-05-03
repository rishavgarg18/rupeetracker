# ₹ Tracker — Monthly Finance PWA

## Files in this folder
```
index.html      ← The app
manifest.json   ← PWA manifest (detected by PWABuilder)
sw.js           ← Service worker (offline support)
icon-192.svg    ← App icon (small)
icon-512.svg    ← App icon (large)
```

---

## How to publish to Google Play Store

### Step 1 — Host on GitHub Pages (free)

1. Go to https://github.com and sign in (create account if needed)
2. Click **"New repository"** → name it `rupee-tracker` → set to **Public** → click Create
3. Upload ALL 5 files from this folder (drag & drop on GitHub)
4. Go to **Settings → Pages** → under "Source" select **main branch / root** → Save
5. Your app is now live at:
   `https://YOUR-USERNAME.github.io/rupee-tracker/`

Wait ~2 minutes for it to go live, then open that URL in Chrome to confirm it works.

---

### Step 2 — Generate APK with PWABuilder

1. Go to https://www.pwabuilder.com
2. Paste your GitHub Pages URL and click **Start**
3. It should now show green checkmarks for Manifest ✅ and Service Worker ✅
4. Click **Package for Stores** → choose **Google Play**
5. Fill in your package name (e.g. `com.yourname.rupeetracker`)
6. Click **Generate** → download the `.aab` file

---

### Step 3 — Upload to Google Play Console

1. Go to https://play.google.com/console
2. Pay the one-time $25 developer fee (if not done)
3. Create a new app → fill in title, description, category (Finance)
4. Under **Release → Production** → upload your `.aab` file
5. Fill in store listing, add screenshots, submit for review

Google review takes 3–7 days for new apps.

---

## Tips
- Keep all 5 files in the same folder / same GitHub repo root
- Don't rename the files
- If you update the app, just replace `index.html` on GitHub — the service worker version (`sw.js`) will auto-update for users
