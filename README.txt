GTA V10.16.11 — Mark Button Fix + Content Cleanup

This build includes two rounds of fixes:

1) MARK BUTTON FIX (code)
   Mastered / Needs Review / Unmarked buttons register and change color again.
   They had broken after audio was added, because the new speak() function
   collided with the Speak screen's element id and crashed the re-render.

2) CONTENT CLEANUP (data only — no Greek meaning changed)
   - Pronunciation spelling standardized: the "ch" sound (χ) is now always
     written "h" (was sometimes "kh"); the "ks" sound (ξ) is now always "ks"
     (was sometimes "x"). 100+ entries normalized.
   - Fixed two transcription typos: "fan" (ανεμιστήρας) and the laundromat
     entry (πλυντήριο).
   - "Takeaway" standardized to πακέτο everywhere (the word the app's own
     listening line already uses), instead of mixing it with "για το χέρι".

Upload all four to GitHub, keeping the same filenames:
- index.html
- service-worker.js   (CACHE_NAME bumped to force the update)
- manifest.json
- icon.svg

After uploading, fully close and reopen the app to clear the old cache.
