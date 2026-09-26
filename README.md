# Finn Dash — web version (works on iPhone and iPad)

This folder is the whole web game. Put it online once and anyone can play it in a browser, or add it
to their home screen so it opens full-screen and works with no internet.

## Put it online with GitHub Pages (free)

1. On GitHub, make a new **public** repository, for example `finn-dash-web`.
2. Choose **Add file → Upload files** and drag in everything from this folder:
   `index.html`, `manifest.webmanifest`, `sw.js`, and the `icons` folder.
3. Commit the upload.
4. Go to **Settings → Pages**. Under "Build and deployment", set **Source** to *Deploy from a branch*,
   pick branch `main` and folder `/ (root)`, then **Save**.
5. Wait a minute or two. The page appears at:
   `https://<your-github-username>.github.io/finn-dash-web/`

That link is the game. It works on iPhone, iPad, Android and any computer.

## Add it to an iPhone or iPad home screen

1. Open the link in **Safari** (it has to be Safari, not Chrome).
2. Tap the **Share** button (the square with the arrow).
3. Tap **Add to Home Screen**, then **Add**.
4. The Finn Dash icon appears with the other apps. It opens full-screen, with no address bar, and
   plays with no internet after the first run.

On Android, Chrome shows an **Install app** option in its menu that does the same thing.

## Updating the game later

Upload a new `index.html` the same way. Also change the version line at the top of `sw.js`
(`const CACHE = 'finn-dash-…'`) to something new — that is what tells phones to fetch the new copy.
Players get the update the next time they open it with an internet connection.

## Things to know on iPhone

- **Sound:** the game plays a silent clip on the first tap so it can be heard even when the ring/silent
  switch is set to silent. If there is still no sound, flick the switch back on.
- **Saved progress** lives on that device. Apple can clear a web app's storage if it goes unused for a
  long stretch; if that happens, the **🔑 Secret Codes** on the main menu give a quick head start again.
- There are no ads, no accounts and nothing is sent anywhere — the game runs entirely on the device.
