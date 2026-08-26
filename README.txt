SD AutoScoring — unified mobile app (Straight Drive)
====================================================

WHAT'S HERE
  index.html          The whole app. Self-contained: all icons and the logo are
                      inlined, so the UI needs NO other files to display.
  assets/             Only used for the PWA "add to home screen" install
                      (manifest + icon PNGs) and the browser favicon.

HOST ON GITHUB PAGES
  1. Put index.html and the assets/ folder at the repo root (siblings):
        your-repo/
        |- index.html
        |- assets/  (manifest.json, favicon.png, apple-touch-icon.png,
                     icon-192.png, icon-512.png, logo.png)
  2. Repo Settings > Pages > Deploy from a branch > main > / (root) > Save.
  3. Open https://<username>.github.io/<repo>/ on laptop AND phone.
     Must be the https:// URL — Web Serial / WebUSB need a secure origin.

NOTES
  * Desktop (Chrome/Edge): uses native Web Serial.
  * Android Chrome: uses the WebUSB polyfill automatically (loaded from a CDN).
  * On a phone, turn it LANDSCAPE for the lane map.
  * To provision a node from a phone: wake the node (tap it once) BEFORE
    tapping Connect, so it appears in the USB chooser.
  * Master MAC + RF channel are saved and auto-filled into every node.
