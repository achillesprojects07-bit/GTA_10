GTA Greek Travel App — V11.0.33 Am I Ready? Dashboard

Built as a targeted patch on top of V11.0.32.

V11.0.33 changes:
- Added an Am I Ready? trip-readiness dashboard on the Home screen.
- Shows survival-critical Greek readiness as a percentage using the honest Field-ready signal.
- Breaks readiness down by practical survival buckets:
  - Survival basics
  - Conversation repair
  - Café + taverna
  - Getting around
  - Health + emergency
  - Phone / Wi-Fi
  - Family + home
- Surfaces the biggest readiness gaps.
- Adds one-tap practice buttons for the weakest area, Due Now, and Today's 5.
- Uses the saved trip date when available to make the readiness card deadline-aware.
- Does not change SRS scheduling or Field-ready requirements.

Preserved:
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
- Service-worker cache bumped to gta-v11-0-33-readiness-dashboard.
