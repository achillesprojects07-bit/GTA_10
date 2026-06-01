GTA V10.14.3 Batch 3 Storage Safety

Upload these files to GitHub:
- index.html
- manifest.json
- service-worker.js
- icon.svg

Base retained from V10.14.2:
- Speak, Vocabulary, Verb Sets, Practical Noun Patterns, Travel Mode, Play, Match, Phrase Builder, Backup, and Review.
- Play Mode totals 1,220 activities.
- Match Mode remains full coverage at 1,136 pairs.
- Backup / Restore remains available from Home.

Batch 1 fixes retained:
- Streak only continues when the last active day was exactly yesterday.
- Dashboard subtitle contrast improved on colored cards.
- Phrase Builder button label corrected.
- Backup download filename updated.

Batch 2 fixes retained:
- Home is highlighted for Home-only screens: Verb Sets, Noun Patterns, Travel Mode, Phrase Builder, Backup.
- Orientation label added to Home-only screens.
- showView render calls preserved.

Batch 3 storage safety fixes:
- Added device-only progress warning.
- Added backup reminder when no backup has been saved or when the last saved backup is older than 7 days.
- Copy Backup and Download Backup File update the last-backup timestamp.
- Restore imports lastBackupAt when available.
- Backup file name is gta-backup-v10-14-3.json.

Fallbacks included:
- index.v10.14.fallback.html
- index.v10.14.1.fallback.html
