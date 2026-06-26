GTA Greek Travel App — V11.0.31 Trip Date Focus + Orphan SRS Cleanup

Built as a targeted combined patch on top of V11.0.29.

V11.0.30 cleanup included:
- Added a one-time orphan SRS prune for old synthetic records left by temporary Play/Match SRS routing.
- Prune whitelists against srsReviewLookup(), so valid reviewable records are preserved.
- Does not prune state.marks, personal items, content, or learning history.

V11.0.31 trip-focused upgrade included:
- Added a Home Trip Readiness card with a trip-date picker and countdown.
- Saves the trip date locally under gta_trip_date.
- Today’s 5 now uses trip-aware priority categories.
- In the final week before the trip, Today’s 5 prioritizes survival-critical categories: Must Know, Conversation Repair, Café/Restaurant, Getting Around, Health/Emergency, Phone/Wi-Fi, and Family/Belonging.
- SRS scheduling now avoids pushing review due dates after the saved trip date.
- In the final week, survival-critical successful reviews are scheduled sooner so they remain fresh.
- Due Now ordering prioritizes survival-critical items when the trip is within 14 days.

Preserved:
- V11.0.29 SRS stabilization and Today’s 5 success grading.
- V11.0.28 durable storage / IndexedDB auto-backup patch.
- Greek audio health check, Survival Search, Scenarios, Today’s 5, Today’s Greek Guide, Shadowing recording, Phrase Builder, and all existing content.
- Manual Backup/Restore remains unchanged.

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- <section> count balanced: 19 open / 19 close.
- app.js is not included.
- Service-worker cache bumped to gta-v11-0-31-trip-date-focus.
