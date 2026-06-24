GTA Greek Travel App — V11.0.26 (Greek Audio Health Check) + Structural Hotfix 1

This package is V11.0.26 with one critical layout bug fixed.

HOTFIX 1 change (the only code change vs the original V11.0.26):
- Closed the <section id="scenarios"> element, which was left open in the
  original V11.0.26 build.
- Cause: with that tag missing, every view after Scenarios (Speak, Vocab,
  Verbs, Patterns, Questions, Smart Practice, Speak-First, Shadowing,
  Conversations, Play, Listen, Travel, Match, Phrase Builder, Backup/Restore,
  and Priority Review) was parsed as a child of #scenarios. Because a hidden
  (.view without .active = display:none) parent hides all of its children,
  those 16 views rendered as a blank content area when opened. Home, Today's 5,
  and Scenarios were unaffected.
- Fix: a single </section> tag was added. No JavaScript, CSS, or content was
  changed. Section tags now balance (19 open / 19 close) and all views are
  top-level siblings again.
- Bumped the service-worker cache name to 'gta-v11-0-26-hotfix1' so existing
  installs re-cache the corrected index.html instead of serving the old broken
  copy. (The visible app version, manifest, and backup filename remain
  V11.0.26.)

----------------------------------------------------------------------
Original V11.0.26 notes (unchanged):

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
- Today's Greek Guide, Phrase Builder, SRS/Weak Items, Listen Mode, Match Mode, Smart Practice, audio buttons, backup/restore, and offline PWA behavior.

Files in this package:
- index.html (fixed)
- manifest.json
- service-worker.js (cache name bumped)
- icon.svg, icon-192.png, icon-512.png, apple-touch-icon.png
