GTA Greek Travel App — V11.0.3 Pronunciation Recording + Learning Path

Built as a targeted patch on top of V11.0.2.

V11.0.3 changes:
- Added Shadowing self-recording comparison using the browser MediaRecorder API.
- Shadowing now has a separate Play model audio button and a Record my voice button.
- Recording captures a fixed 4-second attempt, then immediately provides playback beside the Greek model.
- Added pronunciation self-ratings: Stress wrong, Speed wrong, Sounds close.
- Pronunciation ratings are stored locally in gta_pron_log with item ID, rating, and timestamp.
- Added a running Shadowing tally for Sounds close ratings in the current session.
- Added microphone fallback message for unsupported/denied microphone access: use phone Voice Memos beside the model audio.
- Added a dismissible Where to start learning path on the Home screen.
- Learning path has 6 stages: Survival phrases, Basic vocabulary, Conversation repair, First drills, Speak out loud, Real conversations.
- Learning path visited stages are stored in gta_path_visited and dismissal is stored in gta_path_dismissed.
- Updated visible app label to V11.0.3.
- Updated manifest display name to GTA Greek V11.0.3.
- Updated service-worker cache name to gta-v11-0-3.
- Updated backup filename to GTA_V11_0_3_backup.json.

Preserved from prior builds:
- V11.0.2 expanded Dialogue Builder with 173 drills.
- V11.0.1 One-Minute Drill category/round picker and 143 fast rounds.
- V11.0 grammar tooltips.
- V10.28 unified Weak Items/SRS/listening integration.
- V10.27 weekly activity chart and streak counter.
- V10.26 shadowing tips and V10.25 open dialogues.
- Existing audio, Speak & Check, Match, Listen, Smart Practice, Phrase Builder notes, backup/restore, and offline PWA behavior.

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- Required files present.
