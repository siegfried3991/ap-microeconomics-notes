# MicroQuest · AP Microeconomics

**Account status:** open email/password registration with immediate sign-in; email confirmation is disabled at the owner’s request. Progress syncs to a private, revisioned cloud record. Password recovery by email remains unavailable until an email service is configured.

A game-style study companion for Unit 4: Imperfect Competition.

**Play:** https://siegfried3991.github.io/ap-microeconomics-notes/  
**Complete original notes:** https://siegfried3991.github.io/ap-microeconomics-notes/notes.html

## Learn, review, then attempt AP

- Ten short lessons and 64 original challenges: market structures, monopoly, profit and loss, welfare, natural monopoly, price discrimination, monopolistic competition, oligopoly, game theory, and a mixed checkpoint.
- Multiple choice, multiple selection, numerical calculations, graph reading, and ordering tasks. Immediate explanations; missed questions return until solved.
- XP, daily goals, study streaks, and saved sessions. First correct answers and first lesson completions earn XP once. Review XP is limited to once per question per day.
- Mistake repair, mixed practice, and spaced review after 1, 3, 7, 14, then 30 days. Concept bars count unique correct answers, not predicted AP scores.
- Four authentic released AP free-response tasks: 2026 Q1, 2025 Set 1 Q3, 2024 Set 2 Q1, and 2023 Set 2 Q3. Open the official paper, write in an autosaving answer workspace, sketch on the graph pad, use a practice timer, and self-score using the official scoring guide.

Original drills are clearly distinguished from official exam questions. Official papers remain hosted by the College Board; they are linked or embedded, not rehosted. Brief scoring reminders are paraphrases and do not replace the official criteria. This independent project is not endorsed by the College Board.

## Privacy and offline use

Guest progress stays in local storage. Signed-in progress and AP drafts sync to a private per-user Supabase database row, with an offline account cache. Authentication sessions are stored by the Supabase SDK in local storage; learning backups never contain passwords or authentication tokens. No analytics are included. Use the progress backup/restore tools to move between browsers. Clearing site data removes locally stored progress unless you keep a backup. A backup includes your written answers: keep it private.

Save `index.html` and `notes.html` in the same folder for offline learning. Fonts, math rendering, and game code are embedded; official PDFs require internet. A downloaded file and the hosted website have separate browser storage. The original notes retain their graphs, flashcards, original exercises, printable reference, and review planner.

## Files

`index.html` is the standalone game. `notes.html` is the full original guide. `game-source/` contains editable source files locally. The game is buildless once generated. Run `python3 game-source/build.py` to regenerate the page from its editable source and vendored assets. Run `node tests/cloud.test.cjs` for cloud state tests. `tests/build-preview.py` builds a clearly labeled mock account preview for local QA only; never publish `auth-preview.html`.

KaTeX 0.16.11 (MIT), D3 7.9.0 (ISC, in notes), DM Sans and Literata (SIL Open Font License), and the HTML Explainer review overlay (MIT, in notes) are included. See `THIRD-PARTY-NOTICES.txt`.

Created 25 October 2026; account upgrade prepared 26 October 2026.
