GTA Greek Travel App — V11.0.32 Honest Field-Ready Signal

Built as a targeted patch on top of V11.0.31.

V11.0.32 changes:
- Added an honest Field-ready signal so the app no longer treats same-session success as true readiness.
- Field-ready now means the item was recalled strongly on more than one day.
- Updated SRS mastery gate: level-4/strong answers must occur across at least 2 unique dates before state.marks[id] becomes mastered/field-ready.
- Same-session app recognition now appears as Practiced rather than Field-ready.
- Speech feedback labels now distinguish app recognition from real-world readiness:
  - App understood you
  - App clearly understood you
- My Progress now shows Field-ready count instead of a flattering Mastered count.
- Home stat label changed from Mastered to Field-ready.
- Existing SRS scheduling, trip-date focus, durable storage, and backup/restore remain preserved.

Preserved:
- V11.0.31 trip-date focus and orphan SRS cleanup.
- V11.0.29 SRS stabilization and Today’s 5 success grading.
- V11.0.28 durable storage / IndexedDB auto-backup patch.
- Greek audio health check, Survival Search, Scenarios, Today’s 5, Today’s Greek Guide, Shadowing recording, Phrase Builder, and all existing content.

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- <section> count balanced: 19 open / 19 close.
- app.js is not included.
- Service-worker cache bumped to gta-v11-0-32-field-ready.
