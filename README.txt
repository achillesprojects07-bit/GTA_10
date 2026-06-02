GTA V10.17.2 — Category Progress Corrected from V10.16.11 Base

This build returns to the working V10.16.11 app core and adds only the corrected category progress layer.

WHAT IS CORRECTED:
- Speak Now, Vocabulary, Verb Sets, and Noun Patterns show category progress counts.
- Counts use only the learning-status language: Mastered, Needs Review, and Unmarked.
- Clicking a category status filters that exact category.
- Play Mode categories are visible and show Mastered / Needs Review / Unmarked.
- Listen Mode categories show Mastered / Needs Review / Unmarked, not Done / Correct / Review.
- Match Mode rounds show Mastered / Needs Review / Unmarked.
- Travel Mode rows show linked Mastered / Needs Review / Unmarked progress.
- A category turns green only when all items are Mastered and Needs Review + Unmarked are zero.
- Clearing Listening Review moves missed listening items back to Unmarked and refreshes counts immediately.

PRESERVED FROM V10.16.11:
- Existing app layout and navigation.
- Existing Greek audio system.
- Existing Play, Listen, Match, Travel, Review, Phrase Builder, and Backup/Restore structure.
- Existing Mastered / Needs Review / Unmarked card marking.

UPLOAD TO GITHUB:
- index.html
- service-worker.js
- manifest.json
- icon.svg

IMPORTANT AFTER UPLOAD:
Fully close and reopen the app, or clear the browser cache, because the service worker cache has been bumped to gta-v10-17-2-category-progress-corrected.
