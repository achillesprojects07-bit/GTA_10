GTA V10.25.1 — Wiring Fix for Shadowing Tips + Open Dialogues

Targeted repair build based on GTA_V10.25.0_family_time_open_dialogues.

Purpose:
- V10.25.0 declared GTA_V1025_CONTENT_ADDITIONS but the app did not explicitly consume it in the working screens.
- This patch wires the already-existing data into the UI.
- No new Greek content was added.

Preserved:
- Existing app structure and working logic.
- Speak & Check, Hear My Voice, Greek audio function, SRS, Smart Practice, Match Mode, Play, Listen, Shadowing, Conversation Simulator, Phrase Builder, Review, Backup, icons, and PWA/offline structure.

Changed in V10.25.1:
- Shadowing now reads GTA_V1025_CONTENT_ADDITIONS.tips and renders the Shadowing tip as a visible instruction card.
- Dialogue Builder now reads GTA_V1025_CONTENT_ADDITIONS.dialogues and merges those 3 open conversation scenarios into the existing Smart Practice Dialogue Builder list.
- Added de-duplication by category/title/opening line so the same 3 open conversation scenarios do not appear twice if already present in SMART_DIALOGUES.
- Updated visible version label, manifest, service-worker cache name, and backup filename.

Audit summary:
- index.html JavaScript syntax check passed.
- Required files present: index.html, manifest.json, service-worker.js, README.txt, icon.svg, icon-192.png, icon-512.png, apple-touch-icon.png.
- Confirmed wiring helpers present: consumeV1025Dialogues(), normalizeV1025Dialogue(), and v1025ShadowTipCards().
- Version label: V10.25.1.

Upload all files, then hard refresh. For the installed iPhone Home Screen app, fully close/reopen it. If the old cache persists, delete and re-add the Home Screen icon.
