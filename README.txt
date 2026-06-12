GTA Greek Travel App — V11.0 Phase 4

Built from V10.28.0 Phase 3 as the final V11 polish patch.

Phase 4 changes:
- Added lightweight grammar tooltip layer on vocabulary cards.
- Vocab cards with useful grammar patterns now show a small ? button beside the Greek word.
- Tapping ? opens a brief modal grammar note.
- Notes cover article gender, adjective endings, verb endings, family gender pairs, plurals, and fixed short chunks.
- Grammar layer is non-blocking: cards still render normally even without a matching grammar note.
- Updated visible app label to V11.0.
- Updated manifest display name to GTA Greek V11.0.
- Updated service-worker cache name to gta-v11.
- Updated backup filename prefix to GTA_V11.

Preserved from previous builds:
- Phase 1 content additions, Shadowing tips, and Open Dialogue Builder badge.
- Phase 2 activity log, weekly rhythm chart, and streak counter.
- Phase 3 unified Weak Items pool and Listen Mode to SRS handoff.
- Speak & Check, Hear My Voice, memory hooks, Match Mode, Smart Practice, Listen Mode, SRS, Phrase Builder notes, backup/restore, audio, and offline PWA support.

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- Required files included: index.html, manifest.json, service-worker.js, README.txt, icons.

Upload instructions:
1. Upload all files to the same web host folder.
2. Hard refresh the app after upload.
3. If installed on iPhone Home Screen, open once online so the new service worker cache can refresh.
4. Export a backup after confirming the app opens.
