# MicroQuest · Economics & Mathematics

A shared learning site for six AP Microeconomics units and Precalculus sections 1.1–1.5. Play at [MicroQuest](https://siegfried3991.github.io/ap-microeconomics-notes/).

## Mathematics · Precalculus

Open [Mathematics](https://siegfried3991.github.io/ap-microeconomics-notes/#subject/mathematics), or choose Mathematics in the subject menu. This path follows **only textbook sections 1.1–1.5**, printed pp.88–152, of *Precalculus: Graphical, Numerical, Algebraic*, ninth global edition (Demana et al., Pearson, 2015).

The five sections contain **17 lessons and 102 original practice questions**, with worked examples, guided completion, saved working, teach-back prompts, immediate feedback, immutable first-attempt outcomes, and spaced/mixed review. The toolkit has all twelve basic function graphs with domain/range and value tables, a parameter slider, inverse reflection, 24 recall cards, five saved written challenges with self-check rubrics, connected concept navigation, a quick reference and a study planner. Written solutions are not automatically graded. Simple fractions are supported for numerical answers.

The method adapts [IES recommendations](https://ies.ed.gov/ncee/wwc/PracticeGuide/1), [Taylor & Rohrer’s interleaving study](https://digitalcommons.usf.edu/psy_facpub/1760/) and [Emeny et al.’s mathematics-spacing study](https://files.eric.ed.gov/fulltext/ED611846.pdf): alternate examples with problems, retrieve and explain ideas, mix previously attempted problem types, and return after a delay. These are evidence-informed design choices; the specific course and chosen timing have not been experimentally validated.

Maths and economics retain distinct lessons, sessions and question records in the same account. Subject-wide review stays inside the selected subject; XP and streaks remain site-wide. Version-4 checkpoints include written maths work, planner marks, hints used and first checked outcomes; the existing server version guard protects them from older clients. Refresh older tabs on other devices before continuing. The owner's textbook PDF is not published; all course notes, practice questions and plots are original.

Maths content and methodology live locally in `game-source/mathematics/`. Build with the existing build script and validate using `node tests/mathematics.test.cjs` in addition to the existing suites.

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

## Explain another way

Each Homework explanation and checked practice question has an **Explain another way** button. The chooser offers simpler wording, steps, an example, or exam reasoning and keeps the original available for comparison. This covers 394 explanation contexts across the homework packet and six course units.

The private OpenAI API connection is prepared but generation is **not active until its credential and live checks are complete**. A signed-in account is required. The planned allowance reserves two US cents per request, stopping at US$5 per UTC month for the whole site, with two requests per minute and twenty per 24 hours per account. Reusing an alternative in the same page session does not spend again; asking for a fresh version makes a new request. Alternatives are not saved in progress checkpoints.

Only the selected question and its canonical study answer/explanation are sent to the AI service. Email, account identity, written working, passwords, and API keys are excluded. Generated text is labeled as AI and cannot change the answer key, score or first attempt. The API is separately billed; this implementation does not draw from a ChatGPT subscription. See OpenAI's [hosted-app plan eligibility](https://developers.openai.com/siwc/token-sharing-open-source) and [API authentication guidance](https://developers.openai.com/api/reference/overview).

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
