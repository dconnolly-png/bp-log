# BP Log — private blood pressure tracker

A blood pressure log that runs on your phone and works offline. Your readings are stored only on your phone and are never sent anywhere. (The page blocks all network requests: `connect-src 'none'`.)

## Files
- `index.html` — the whole app
- `sw.js` — lets it work offline
- `manifest.webmanifest` + 3 icons — let it install like a normal app

## Put it online (free, about 5 minutes)
Android only installs web apps from an `https://` address. The host only stores these app files. Your readings never go to it.

**GitHub Pages**
1. Sign in at github.com and create a new repository, for example `bp-log`.
2. Click **Add file → Upload files**, drag in all 6 files and click **Commit**.
3. Go to **Settings → Pages**. Set **Source** to "Deploy from a branch", pick the **main** branch and **/(root)**, then click **Save**.
4. After a minute your app is at `https://<your-username>.github.io/bp-log/`.

## Install on Android
1. Open that link in **Chrome** on your phone.
2. Tap the **⋮** menu, then **Add to Home screen**, then **Install**.
3. Open it from the home-screen icon. From then on it works with no signal.

## Updating later
Upload the changed files to the same repository. The phone picks up the new version the second time you open the app while online. Your readings aren't affected.

## Keep your data safe
- Use **Settings → Back up everything** now and then, and keep the file somewhere safe (Google Drive, email it to yourself, and so on).
- Uninstalling the app or clearing Chrome's data for the site deletes your readings.
- To move to a new phone: install the app there, then **Restore from backup**.
