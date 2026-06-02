GTA V10.16.11 — Audio in Play & Match Modes

Adds audio buttons to Play Mode and Match Mode.
All previous fixes (mark buttons, content cleanup) are included.

WHAT'S NEW:
- Play Mode MC: a 🔊 Hear Greek button appears when a Greek prompt
  is shown on the card, so you can hear it before answering.
- Play Mode correct feedback: 🔊 Hear Greek button appears in the
  "Correct" panel so you can hear the answer after getting it right.
  Only fires when the answer is Greek text (not English answers).
- Match Mode correct feedback: 🔊 Hear Greek button appears in the
  "Correct match" panel so you can hear the Greek word after matching.

HOW IT WORKS:
These buttons use the same speech engine already in the app.
If your device has a Greek voice installed, it speaks automatically.
If no Greek voice is available, the button is hidden.

Upload all four to GitHub, keeping the same filenames:
- index.html
- service-worker.js   (CACHE_NAME bumped)
- manifest.json
- icon.svg

After uploading, fully close and reopen the app to clear the old cache.
