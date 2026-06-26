GTA Greek Travel App — V11.0.29 Durable Storage Patch

Built as a targeted safety patch on top of V11.0.27 SRS Routing + Due Now.

V11.0.29 changes:
- Added best-effort navigator.storage.persist() request on startup.
- Patched save() to trigger a throttled automatic IndexedDB backup.
- Added automatic latest + daily IndexedDB snapshots, keeping the newest 7 daily snapshots.
- Added safe recovery from IndexedDB only when localStorage appears empty/evicted.
- Recovery restores the same backup fields used by the existing manual Backup/Restore system.
- Manual Backup/Restore, SRS scheduling, app content, and learning modes were not changed.
- Removed no files and added no external dependencies.
- Updated visible app version, manifest, service-worker cache, README, and backup filename to V11.0.29.

----------------------------------------------------------------------
Previous notes:

GTA Greek Travel App — V11.0.29 (Greek Audio Health Check) + Structural Hotfix 1

This package is V11.0.29 with one critical layout bug fixed.

HOTFIX 1 change (the only code change vs the original V11.0.29):
- Closed the <section id="scenarios"> element, which was left open in the
  original V11.0.29 build.
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
  V11.0.29.)

----------------------------------------------------------------------
Original V11.0.29 notes (unchanged):

Built as a targeted audio-safety patch on top of V11.0.25.

V11.0.29 changes:
- Added a Greek TTS voice health check that runs once each session.
- The app now checks for an installed Greek voice using speechSynthesis.getVoices() and the voiceschanged event, with a 1-second fallback.
- Added a visible Greek audio status next to the app version:
  - Green dot: Greek audio ready
  - Amber dot: Greek audio check settings
- Added a dismissible Home warning banner if no Greek voice is confirmed.
- Updated speak() so it actively prefers a Greek voice before speaking.
- If no Greek voice is available, audio is allowed to play but a single voice-warning entry is logged to gta_pron_log for the session.
- Updated visible app version, manifest, service-worker cache, and backup filename to V11.0.29.

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


V11.0.29 SRS routing and Due Now hotfix
- Routed Memory Hook Quiz, One-Minute Drill, Listen Mode, Play Mode, sentence-builder Play Mode, and Match Mode answer results through applySrsResult().
- Replaced Listen Mode seed-only SRS behavior so answers grade the SRS record instead of only ensuring one exists.
- Added Review → Due Now listing ordered by days overdue.
- Made the Home Due Today counter open the Due Now review surface.
- Removed the unreachable earlier startSpeechCheck definition; the later SRS-aware implementation remains.
- Confirmed ease is not true SM-2 scheduling in this build: it is incremented/stored, but intervals are driven by the fixed [1,3,7,21,60] ladder.
- Updated service-worker cache name so installed copies re-cache.


V11.0.29 SRS stabilization notes:
- Due Now and Home Due Today now count only valid reviewable SRS ids.
- Play Mode and Match Mode no longer write synthetic game_*/match_* ids into SRS; they keep their local review stacks.
- Today’s 5 now grades correct answers through applySrsResult(id,true,3).
- Today’s 5 failures now use applySrsResult(id,false,1).
- Today’s 5 phrase ids now resolve to canonical p_# ids, with legacy today5_phrase_# selections still readable.
