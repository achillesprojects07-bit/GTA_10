GTA Greek Travel App — V11.0.34 Start Today / Home Simplification

Built as a targeted patch on top of V11.0.33.

V11.0.34 changes:
- Added a clear Start Today hub on the Home screen.
- Start Today gives one obvious daily path before the full mode list:
  - Today's 5
  - Plan today with Today's Greek Guide
  - Review Due Now
  - Survival Search for outside use
- Changed the Home hero primary action to Start Today.
- Tucked the large practice-mode grid behind a More ways to practice toggle.
- The More ways toggle is remembered locally under gta_more_practice_open.
- Added a compact status pill showing Today's 5 progress, Due Now count, and trip countdown when available.
- Did not remove any mode or content; all existing sections remain available under More ways to practice.

Preserved:
- V11.0.33 Am I Ready? dashboard.
- V11.0.32 honest Field-ready signal.
- V11.0.31 trip-date focus and orphan SRS cleanup.
- V11.0.29 SRS stabilization and Today's 5 success grading.
- V11.0.28 durable storage / IndexedDB auto-backup patch.
- Greek audio health check, Survival Search, Scenarios, Today's 5, Today's Greek Guide, Shadowing recording, Phrase Builder, and all existing content.

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- <section> count balanced: 19 open / 19 close.
- app.js is not included.
- Service-worker cache bumped to gta-v11-0-34-start-today-home.
