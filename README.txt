GTA Greek Travel App — V11.0.23

Built as a targeted patch on top of V11.0.22.

V11.0.23 changes:
- Upgraded Quick Search into Survival Search Mode.
- Added a Survival Mode toggle saved in localStorage as gta_survival_mode.
- Survival Mode shows large, one-hand friendly single-column cards.
- Survival cards show Greek first, pronunciation, English, a large audio button, and a Needs Review button.
- Added situation quick-filter buttons: café, restaurant, directions, shopping, home, health, repair.
- Situation buttons pre-fill the existing Quick Search input and run the existing search logic.
- Quick Search continues to save the last searched term under gta_last_quick_search and pre-fills it on the next open.
- Clear button clears the input and results only; the situation quick filters remain available.
- In Survival Mode, Must Know and Conversation Repair items sort to the top.
- Updated visible app version, manifest, service-worker cache, and backup filename to V11.0.23.

Preserved:
- Existing grouped Quick Search layout when Survival Mode is off.
- Existing gtaRunQuickSearch(), gtaClearQuickSearch(), and gtaOpenQuickSearch() entry points.
- Scenarios mode from V11.0.22.
- Today's 5 from V11.0.21.
- Greek-first Shadowing from V11.0.20.
- Today’s Greek Guide, Phrase Builder, SRS/Weak Items, Listen Mode, Match Mode, Smart Practice, audio, backup/restore, and offline PWA behavior.

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- Required files present.
