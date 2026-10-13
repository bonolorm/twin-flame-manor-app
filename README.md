# Twin Flame App — PWA / GitHub Pages Package

This folder is ready to upload directly to a GitHub repository.

## Files that must stay together

- `index.html` — the Twin Flame guest guide
- `manifest.webmanifest` — tells iPhone/Android this is an installable web app
- `service-worker.js` — makes the guide cache for offline/reliable use
- `icons/` — iPhone and Android app icons
- `.nojekyll` — keeps GitHub Pages from altering the static files

## Publish free with GitHub Pages

1. In GitHub, create a new **public** repository. A good name is `twin-flame-app`.
2. Open the repository and choose **Add file → Upload files**.
3. Upload **everything inside this folder**. Do not upload only `index.html`.
4. Commit the files to the `main` branch.
5. Open **Settings → Pages**.
6. Under **Build and deployment**:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
7. Save.
8. After GitHub publishes it, your link will look like:
   `https://YOUR-USERNAME.github.io/twin-flame-app/`

## Install on iPhone

1. Open the published link in **Safari**.
2. Tap the **Share** button.
3. Tap **Add to Home Screen**.
4. Turn on **Open as Web App** if iOS shows that option.
5. Tap **Add**.

The Home Screen icon will show the Twin Flame gold TF crest.

## Install on Android

1. Open the link in Chrome.
2. Tap the browser menu.
3. Choose **Install app** or **Add to Home screen**.
4. Confirm.

## Offline support

After the app has been opened successfully once from the published HTTPS link,
the service worker caches the core app so it can reopen with poor/no internet.

## Important note about Owner Studio

The current Owner Studio stores edits only in the browser on the device where you make them.
Because GitHub Pages is static hosting, those edits do **not** automatically update every guest's copy.

For now, use the hosted PWA as the shared guest guide. If you later want one admin panel
that updates the live app for every guest, that requires a small shared backend/CMS.

Default local Owner Studio password:
`twinflame-admin`

This password is not suitable for protecting sensitive information on a public static site.
