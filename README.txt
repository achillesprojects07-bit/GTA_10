GTA V10.22.1 — Audio Stability Fix

Base: V10.22 Smart Practice Modes.

Fixes:
- Strengthened Greek audio playback for repeated tapping across Speak, Vocab, Listen Mode, Smart Practice, Match feedback, Travel shortcuts, and Question Builder.
- Audio text is encoded safely for all buttons.
- Listen Mode Play Audio and Slow buttons now use the same robust audio player.
- Long phrases are split into smaller speech chunks.
- Added speech resume keep-alive to reduce mobile/browser speechSynthesis pausing after a few plays.
- Buttons show Playing while active and reset after playback.

Preserved:
- Smart Practice Modes
- Memory hooks
- Expanded Match Mode
- Quick Commands and Quick Direction Words
- Taverna/Bakery/Drinks/Desserts/Menu content
- Intensive Category Quiz
- Progress, Review, Backup/Restore

Upload all four main files:
index.html
service-worker.js
manifest.json
icon.svg

After upload, fully close and reopen the app. If old audio behavior continues, clear site data/cache once because an old service worker may still be serving the previous file.
