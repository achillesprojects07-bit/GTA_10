Greek Fluency Companion — V11.1 Fluency Pathway Engine

Built on top of GTA V11.0.35 I'm Here Now Mode.

What changed in V11.1:
- Renamed the app identity from Greek Travel App to Greek Fluency Companion.
- Preserved all existing V11.0.35 content and tools: Speak Now, Vocabulary, Verbs, Noun Patterns, Question Builder, Today’s 5, Smart Practice, Speak-First, Shadowing, Conversations, Scenarios, Play Mode, Listen Mode, Match Mode, Travel Mode, I’m Here Now, Phrase Builder, Review, Backup/Restore, SRS, Greek audio, and durable local progress.
- Added a clean 7-tab bottom navigation: Today, Path, Learn, Practice, Library, Partner, Review.
- Rebuilt the main Home into Today: a clear daily study session with daily minutes, target pathway, current unit, session steps, due/weak/mastered/saved stats, and partner challenge.
- Added a Fluency Pathway Engine: Foundation → A1 Everyday → A2 Connected Greek → B1 Functional Fluency.
- Added daily study time selector: 15, 30, 45, 60, 90 minutes.
- Added target pathway selector: Foundation, A1, A2, B1.
- Added Path tab with levels, units, skill chips, progress estimates, and current-unit selection.
- Added Learn tab with only the next useful lesson actions: current unit, vocabulary, grammar, listening, and speaking.
- Added Practice tab with only purposeful drills; no duplicate or decorative cards.
- Added Library tab with search-first design to avoid overwhelming walls of cards.
- Added Partner tab for real-life practice with partner challenge, freeze recovery, questions, and dialogue practice.
- Kept Travel Mode and I’m Here Now as preserved quick-use modes inside the larger fluency app.
- Added localStorage migration for state.fluency while preserving the existing greek_v104_state key.
- Updated manifest and service-worker cache to V11.1.

Design rule applied:
No card appears unless it helps the learner study, decide what to do next, review weakness, track mastery, find content, or use Greek in real life.

Audit notes:
- JavaScript syntax check passed with node --check.
- ZIP integrity check passed after packaging.
- Existing content remains in index.html; no app.js is included.
