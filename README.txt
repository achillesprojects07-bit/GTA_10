GTA V10.16.11 — Mark Button Fix

Fix: Mastered / Needs Review / Unmarked buttons now register and change
color again. They had stopped working after the audio feature was added,
because the new speak() function collided with the Speak screen's element
id and crashed the re-render. renderVisible() now resolves screens through
the $() helper, so audio and the mark buttons work together.

Files to upload to GitHub (replace the existing ones, keep the same names):
- index.html
- service-worker.js   (CACHE_NAME bumped to force the update)
- manifest.json
- icon.svg

After uploading, fully close and reopen the app to clear the old cache.
