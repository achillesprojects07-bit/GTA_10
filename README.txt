GTA Greek Travel App — V11.0.26 Greek Audio Health Check

Built as a targeted audio-safety patch on top of V11.0.25.

V11.0.26 changes:
- Added a Greek TTS voice health check that runs once each session.
- The app now checks for an installed Greek voice using speechSynthesis.getVoices() and the voiceschanged event, with a 1-second fallback.
- Added a visible Greek audio status next to the app version:
  - Green dot: Greek audio ready
  - Amber dot: Greek audio check settings
- Added a dismissible Home warning banner if no Greek voice is confirmed.
- Updated speak() so it actively prefers a Greek voice before speaking.
- If no Greek voice is available, audio is allowed to play but a single voice-warning entry is logged to gta_pron_log for the session.
- Updated visible app version, manifest, service-worker cache, and backup filename to V11.0.26.

Preserved:
- My Progress card from V11.0.24.
- Survival Search Mode from V11.0.23.
- Scenarios mode from V11.0.22.
- Today's 5 from V11.0.21.
- Greek-first Shadowing from V11.0.20.
- Today’s Greek Guide, Phrase Builder, SRS/Weak Items, Listen Mode, Match Mode, Smart Practice, audio buttons, backup/restore, and offline PWA behavior.

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- Required files present.
- app.js duplicate remains removed from the ZIP package.
- Greek audio health check added without blocking audio playback.
