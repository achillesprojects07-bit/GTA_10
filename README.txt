GTA Greek Travel App — V11.0.21

Targeted patch: Today’s 5 daily lesson mode.

Changes:
- Added a new Today’s 5 practice mode on the Home screen.
- Today’s 5 selects 5 priority phrases for the day from existing DATA.phrases.
- Priority categories: Must Know, Conversation Repair, At Home & Family, Café & Drinks, Restaurant & Dinner, Getting Around.
- Each phrase uses a 4-step flow:
  1. Listen — Greek audio plays first, English hidden.
  2. Guess — choose the English meaning from 3 options.
  3. Repeat — see Greek, pronunciation, and English together with normal and 0.7× playback.
  4. Scenario — practice the phrase in a real-life cue.
- Wrong guesses are sent to weak review with applySrsResult(id, false, 3).
- Today’s selection is stored in localStorage as gta_today_phrases.
- Completed phrase IDs for the day are stored in localStorage as gta_today_done and reset by date.
- Added completion card: Today’s 5 complete, with a Go to Review button that opens Shadowing.
- Updated visible app version, manifest, service-worker cache, and backup filename to V11.0.21.

Dialogue Builder expansion count correction preserved:
- Added 140 new Dialogue Builder drills:
  - 98 scripted line-choice drills
  - 42 open conversation simulations

Preserved:
- Shadowing Greek-first reveal flow
- Today’s Greek Guide reset selections
- Global Quick Search
- Speak Now search
- Phrase Builder to Speak/Vocab
- SRS / Weak Items
- Listen Mode
- Match Mode
- Dialogue Builder expansion
- Shadowing pronunciation recording
- Grammar tooltips
- Backup / Restore

Audit notes:
- JavaScript syntax check passed.
- ZIP integrity check passed.
- Required files present.
- Scripted/open count corrected to match actual content (98 scripted, 42 open).
