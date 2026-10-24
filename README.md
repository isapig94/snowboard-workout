# Let's Send It

Off-snow snowboard training, as a web app you can add to an iPhone home screen.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest` | App name, colours and icons |
| `sw.js` | Lets the app open with no signal (offline cache) |
| `icons/` | Home-screen icons |

Upload all of them, keeping `icons/` as a folder.

## Put it on GitHub Pages (web browser only, no Git needed)

1. Sign in at https://github.com (create a free account if you don't have one).
2. Top right **+** → **New repository**.
   - Repository name: `lets-send-it`
   - Visibility: **Public** (free accounts can only publish Pages from public repos).
   - Leave the other options alone → **Create repository**.
3. On the new repo page, click **uploading an existing file**.
4. Open this folder in File Explorer, select `index.html`, `manifest.webmanifest`, `sw.js`, `README.md` **and the `icons` folder**, and drag them all onto the upload area. Check `icons/...` appears in the list.
5. Scroll down → **Commit changes**.
6. Go to **Settings** (tab along the top of the repo) → **Pages** (left sidebar).
   - Source: **Deploy from a branch**
   - Branch: **main**, folder **/ (root)** → **Save**.
7. Wait 1–2 minutes and refresh the Pages screen. It shows **Your site is live at `https://<your-username>.github.io/lets-send-it/`**. Open that link on your computer to check it loads.

## Add it to the iPhone home screen

1. On the iPhone, open **Safari** (it must be Safari) and go to `https://<your-username>.github.io/lets-send-it/`.
2. Let the opening jump finish once, so the app saves itself for offline use.
3. Tap the **Share** button (square with an up arrow), scroll down, tap **Add to Home Screen**.
4. Name it (it suggests "Send It") → **Add**.
5. Open it from the home screen: it runs full screen with no Safari bars.

## Updating it later

1. Change `index.html`.
2. In `sw.js`, bump the version on the first line of code, e.g. `send-it-v1` → `send-it-v2`.
3. On GitHub: open the repo → **Add file → Upload files** → drop the changed files → **Commit changes**.
4. Wait a minute, then open the app on the phone twice (the first open fetches the update, the second shows it).

## Your data

Ticked sessions and logged weights are saved on the phone, inside the home-screen app. They don't sync to other devices or to the Claude artifact version, and deleting the home-screen app deletes them.
