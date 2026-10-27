# MicroQuest · AP Microeconomics

A course hub for all six AP Microeconomics units. Play at [MicroQuest](https://siegfried3991.github.io/ap-microeconomics-notes/).

## Coverage

| Unit | Path | Lessons | Original challenges |
| --- | --- | ---: | ---: |
| 1. Basic Economic Concepts | Foundation | 6 | 24 |
| 2. Supply and Demand | Foundation | 9 | 36 |
| 3. Production, Cost, and the Perfect Competition Model | Foundation | 7 | 28 |
| 4. Imperfect Competition | Extended | 10 | 64 |
| 5. Factor Markets | Foundation | 8 | 32 |
| 6. Market Failure and the Role of Government | Foundation | 5 | 20 |
| **Total** | | **45** | **204** |

Foundation paths give concise concepts, worked rules, and four original drills per lesson. They are introductions and practice, not complete textbooks or certification of exam mastery. The [official course framework](https://apcentral.collegeboard.org/media/pdf/ap-microeconomics-course-and-exam-description.pdf) defines AP scope. The original [complete Unit 4 notes](https://siegfried3991.github.io/ap-microeconomics-notes/notes.html) remain available.

## Learn, review, and attempt AP

- Select any unit from the course hub or study-unit menu. Each unit keeps an independent unfinished session.
- Review one unit or mix attempted questions across the course. Mistakes return until solved; spaced review uses 1, 3, 7, 14, and 30 days.
- XP, daily goals, and streaks span the course. First correct answers and first lesson completions award XP once. Review XP is limited per question per day.
- The four curated authentic AP workspaces currently cover Unit 4: 2026 Q1, 2025 Set 1 Q3, 2024 Set 2 Q1, and 2023 Set 2 Q3. Other units link to the official released-paper library and clearly identify that curated workspaces have not yet been added.
- Original drills are not College Board exam questions. Official papers and scoring guides remain hosted by the College Board. Self-scoring is not an official or automated AP grade.

## Homework

Open [Homework](https://siegfried3991.github.io/ap-microeconomics-notes/#homework). The first assignment, **AP Unit 4 Revision**, contains all 10 FRQs (65 subparts) and 25 MCQs from the 18 images supplied on 27 October 2026. Its source date field is blank, so the library initially groups it by date added. A learner may set its homework date.

The assignment reader keeps scrollable questions on the left and a searchable question index on the right; on phones the index moves above the questions. FRQ model answers open individual explanation bubbles, with model graphs for drawing questions. Each checked MCQ shows a sentence explaining every option. Checked choices lock until an explicit retry, and the first checked choice is retained.

Homework notes, choices, first attempts, review marks, dates, and last visited question save with the learner's existing guest/account checkpoint and backups. This is a study record, not a submission to a teacher. The supplied questions are transcribed and attributed; student names and handwritten answers are excluded. Model explanations are MicroQuest guidance rather than official grades.

Content lives in `game-source/homework/`: packet data, question-diagram crops, display module, CSS, and a source inventory. Future assignments get stable packet/question ids and separate dates. Catalog version 3 adds homework fields; the existing server guard rejects older clients attempting to replace an upgraded checkpoint.

## Accounts and progress

Email/password registration opens an account immediately, without email confirmation, at the owner's request. Minimum password length is 12 characters. Password-recovery email is unavailable until an email service is connected.

Guest progress stays in browser local storage. Signed-in progress, per-unit sessions, and AP drafts sync to a private per-user Supabase record, with local offline caching and revision-conflict handling. Authentication sessions are kept by the Supabase SDK in local storage. Learning backups contain no passwords or tokens, but do contain written answers: keep them private. No analytics are included.

Existing Unit 4 lesson, question, and AP identifiers are retained. Old version-1 checkpoints are interpreted as Unit 4 records; new optional fields add per-unit sessions; a server guard prevents obsolete clients from overwriting an upgraded course checkpoint. Refresh the site on each device to keep syncing with the course version.

## Content architecture (local source)

- `game-source/units/unit1.js` etc. are content packages; `data.js` retains the original Unit 4 package.
- `content.js` defines package helpers and stable question identifiers. `catalog.js` registers the course and units.
- `model.js` owns scoring, unit statistics, review filtering, and session migration. `cloud.js` owns account isolation, safe checkpoint restoration, and revisioned saves. `app.js` renders the course generically.
- Add a unit package, register it in `catalog.js`, and include its script in the build. The game does not assume a fixed unit count. Unit ids, lesson ids, and question ids must remain stable once published.
- `index.html` is the standalone public game. `notes.html` is the original Unit 4 guide. Save both in one folder for offline study; official PDFs and cloud saves require internet. Downloaded files and the hosted website have separate browser storage.

Build with `python3 game-source/build.py`. Validate with `node tests/curriculum.test.cjs`, `node tests/cloud.test.cjs`, and `python3 backend/check-release.py`.

Local QA fixtures (`auth-preview.html`, `course-qa.html`, `tests/`) and private publication metadata must never be published. Public releases include only the generated game, notes, README, notices, and optional `.nojekyll`.

KaTeX 0.16.11 (MIT), D3 7.9.0 (ISC, in notes), DM Sans and Literata (SIL Open Font License), Supabase JS, and the HTML Explainer review overlay (MIT, in notes) are included; see `THIRD-PARTY-NOTICES.txt`. This independent project is not endorsed by the College Board.
