GTA Greek Travel App — V10.28.0 Phase 3

Built from latest working build: GTA_V10.27.0_phase2_activity_streak.zip

Phase 3 scope only:
- Added unified Weak Items pool for Speak-First and Shadowing.
- Weak Items now combine:
  1. SRS due items,
  2. normal Needs Review marks,
  3. Listen Mode Listening Review items,
  4. Listen Mode items missed 2+ times.
- Listen Mode misses now track per-item mistake counts in state.listenMistakes.
- When a Listen Mode item is missed 2+ times, it is added to the SRS queue as a listenweak_* item.
- Speak-First now shows a Listening Weak badge when an item came from Listen Mode weakness.
- Listen Mode explanation text now tells the user that repeated misses are added to SRS.
- Backup/restore now carries listenReview, listenMistakes, and SRS data while remaining backward-compatible with older backups.

Preserved from V10.27.0:
- Activity log under gta_activity_log.
- Study streak under gta_streak.
- Weekly study rhythm chart.
- Header flame streak display.
- Open badge rendering for the three open Dialogue Builder scenarios.
- Shadowing tip cards with Got it dismissal.
- Phase 1 content: Expressing Opinions & Agreement, At the Beach & Outdoors, Greek Family Words.
- Existing Greek audio function.
- Speak & Check, Hear My Voice, memory hooks, Match Mode, Smart Practice, Listen Mode, SRS, Phrase Builder, and backup/restore.

Version updates:
- Visible app label: V10.28.0
- Manifest name: GTA Greek V10.28.0
- Service worker cache: gta-v10-28-0-phase3
- Backup file name: gta-backup-v10-28-0.json

Audit checklist:
- ZIP integrity checked.
- JavaScript syntax checked from embedded script.
- Required files present.
