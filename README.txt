GTA Greek Travel App — V11.0.25 Auto-play + README Count + ZIP Cleanup

Built as a targeted cleanup patch on top of V11.0.24.

V11.0.25 changes:
- Verified and preserved the Greek-first Shadowing auto-play call after shadow card rendering.
- Confirmed Shadowing still auto-plays the Greek model audio when a new Greek-first card loads.
- Corrected the Dialogue Builder README documentation counts:
  - Added 140 new Dialogue Builder drills:
    - 98 scripted line-choice drills
    - 42 open conversation simulations
- Removed dead duplicate app.js from the ZIP package. The active app remains index.html.
- Updated visible app version, manifest, service-worker cache, and backup filename to V11.0.25.

Preserved:
- My Progress card from V11.0.24.
- Survival Search Mode from V11.0.23.
- Scenarios mode from V11.0.22.
- Today's 5 from V11.0.21.
- Greek-first Shadowing from V11.0.20.
- Today’s Greek Guide, Phrase Builder, SRS/Weak Items, Listen Mode, Match Mode, Smart Practice, audio, backup/restore, and offline PWA behavior.

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- Required files present.
- app.js duplicate removed from ZIP cleanup.
- Scripted/open count corrected to match actual content (98 scripted, 42 open).
