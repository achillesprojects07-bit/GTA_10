GTA V10.16 Listen Mode Clean

Upload these files to GitHub:
- index.html
- manifest.json
- service-worker.js
- icon.svg

Base retained from V10.15.1:
- Speak, Vocabulary, Verb Sets, Practical Noun Patterns, Travel Mode, Play, Match, Phrase Builder, Backup, and Review.
- Audio buttons use browser speechSynthesis with lang=el-GR and do not fall back to English voices.
- Backup / Restore and storage safety reminders are retained.

New in V10.16:
- Adds separate Listen Mode with 320 listening activities.
- Listen Mode includes:
  - Hear Greek → Choose English: 120 activities
  - Hear Greek → Choose Greek Text: 120 activities
  - Hear Greek Scenario → Choose Greek Response: 80 activities
- Listen Mode uses the same installed Greek voice as the card audio.
- Includes Play Audio and Slow buttons.

Counts:
- Speak Now phrases: 438
- Vocabulary cards: 594
- Verb-set flashcards: 50
- Practical Noun Pattern cards: 54
- Play Mode activities: 1,220
- Listen Mode activities: 320
- Match Mode pairs: 1,136

Audit notes:
- JavaScript syntax passed.
- Existing card renderers retained.
- Play Mode and Match Mode click handlers retained.
- Backup filename updated to gta-backup-v10-16.json.

Test link after upload:
https://achillesprojects07-bit.github.io/GTA_10/?v=1016
