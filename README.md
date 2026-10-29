# MicroQuest · AP Economics, Mathematics & Literature

A shared learning site for complete AP Microeconomics and AP Macroeconomics topic paths, Precalculus Chapters 1–3, and English Literature. Play at [MicroQuest](https://siegfried3991.github.io/ap-microeconomics-notes/).

## Mathematics · Precalculus

Open [Mathematics](https://siegfried3991.github.io/ap-microeconomics-notes/#subject/mathematics), or choose Mathematics in the subject menu. This path follows **textbook Chapters 1–3** (sections 1.1–1.7, 2.1–2.8, 3.1–3.6), printed pp.88–342, of *Precalculus: Graphical, Numerical, Algebraic*, ninth global edition (Demana et al., Pearson, 2015).

Start at [Tests & study plan](https://siegfried3991.github.io/ap-microeconomics-notes/#tests). There are **21 section checks** of six questions and **three chapter checks** of 42, 48 and 36 questions. These use 126 seeded question templates spanning the textbook sections. Fresh attempts vary numerical parameters and option order; some conceptual questions recur. Students can edit answers and navigate freely before final submission, pause/resume across reloads, and save working. Hints and solutions appear only after submission; diagnostic scores do not award XP or modify lesson practice records.

Wrong and unanswered questions both link to the exact lesson to revisit. Outstanding topic reminders persist until a later check answers every sampled item for that topic correctly. Opening a solution or finishing a lesson alone does not clear them. Reports show section-level results, preserve the latest 20 attempts, and label results as evidence on that sampled check rather than proof of full mastery. Signed-in checks use the existing private account checkpoint; guest checks remain in the browser. Catalog version 5 protects the expanded record against replacement by older open clients.

The 21 sections contain **50 lessons and 234 original practice questions**, with worked examples, guided completion, saved working, teach-back prompts, immediate feedback, immutable first-attempt outcomes, and spaced/mixed review. The toolkit has all twelve basic function graphs with domain/range and value tables, a parameter slider, inverse reflection, 24 recall cards, five saved written challenges with self-check rubrics, connected concept navigation, a quick reference and a study planner. Written solutions are not automatically graded. Simple fractions are supported for numerical answers.

The method adapts [IES recommendations](https://ies.ed.gov/ncee/wwc/PracticeGuide/1), [Taylor & Rohrer’s interleaving study](https://digitalcommons.usf.edu/psy_facpub/1760/) and [Emeny et al.’s mathematics-spacing study](https://files.eric.ed.gov/fulltext/ED611846.pdf): alternate examples with problems, retrieve and explain ideas, mix previously attempted problem types, and return after a delay. These are evidence-informed design choices; the specific course and chosen timing have not been experimentally validated.

Maths and economics retain distinct lessons, sessions and question records in the same account. Subject-wide review stays inside the selected subject; XP and streaks remain site-wide. Version-4 checkpoints include written maths work, planner marks, hints used and first checked outcomes; the existing server version guard protects them from older clients. Refresh older tabs on other devices before continuing. The owner's textbook PDF is not published; all course notes, practice questions and plots are original.

Maths content and methodology live locally in `game-source/mathematics/`. Build with the existing build script and validate using `node tests/mathematics.test.cjs` and `node tests/assessments.test.cjs` in addition to the existing suites.

## Original Microeconomics lesson bank

The original lesson/question identifiers and their saved progress remain available. The direct topic sets below add a simpler primary route.

| Unit | Path | Lessons | Original challenges |
| --- | --- | ---: | ---: |
| 1. Basic Economic Concepts | Full topic path | 6 | 24 |
| 2. Supply and Demand | Full topic path | 9 | 36 |
| 3. Production, Cost, and the Perfect Competition Model | Full topic path | 7 | 28 |
| 4. Imperfect Competition | Full topic path | 10 | 64 |
| 5. Factor Markets | Full topic path | 8 | 32 |
| 6. Market Failure and the Role of Government | Full topic path | 5 | 20 |
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

## Economics mastery checks and graph lab

Start at [Mastery](https://siegfried3991.github.io/ap-microeconomics-notes/#mastery) to bypass introductory drills. Every one of the 45 economics subtopics has four original AP-style diagnostic probes (180 in total), covering calculation, interpretation and reasoning. A check passes with 4/4; a missed probe identifies its skill and links back to the corresponding lesson. First checked answers lock. Retakes vary some numerical cases and option order; conceptual prompts can recur. Passing is separate from completing the introductory lesson and lets the next-lesson suggestion move past that topic. Passed checks become due again after three days. These small checks provide evidence, not certification of mastery or an AP score. Optional written reasoning is saved but not automatically graded.

[Graph lab](https://siegfried3991.github.io/ap-microeconomics-notes/#graphlab/monopoly) includes 13 analytic models: PPC, supply/demand shifts, elasticity, taxes, international trade/tariffs, competitive firm, monopoly, natural monopoly, monopolistic competition, labor-market competition/monopsony, externalities, public goods and Lorenz curves. Native controls update curves, intersections, areas and numeric summaries. Each model explains how to read it and offers three interpretation probes on changed conditions with guidance hidden. A coordinate table supplies the same plotted information for accessibility. Monetary calculations allow the rounding implied by displayed coordinates. A phone can pan the graph without widening the page.

These are original questions and teaching models. Related authentic released FRQs are linked to their named questions/parts on the College Board website, with access to the official scoring-guide library; the original diagnostics are labeled separately. The alignment follows the [official course framework](https://apcentral.collegeboard.org/media/pdf/ap-microeconomics-course-and-exam-description.pdf), with related released examples from [2023 Set 1](https://apcentral.collegeboard.org/media/pdf/ap23-frq-microeconomics-set-1.pdf), [2024 Set 2](https://apcentral.collegeboard.org/media/pdf/ap24-frq-microeconomics-set-2.pdf), [2025 Set 1](https://apcentral.collegeboard.org/media/pdf/ap25-frq-microeconomics-set-1.pdf) and [2025 Set 2](https://apcentral.collegeboard.org/media/pdf/ap25-frq-microeconomics-set-2.pdf). No secure AP Classroom questions are used.

Checks, unfinished subtopic attempts, reasoning, graph settings and graph evidence use the existing guest/account checkpoint, offline cache, conflict handling and backup/restore. Checkpoint version 6 preserves maths tests, homework and AP drafts; the existing server version guard rejects older clients replacing a newer checkpoint. Refresh older tabs on all devices after this release. No new database migration or AI API connection is needed for these features. Content and analytic models live locally in `game-source/mastery/`; validation is `node tests/economics.test.cjs` alongside the existing suites. Public publication remains limited to the standalone page and public documentation.

## English Literature · Close Reading

The subject menu now includes **English Literature**. [Open the course](https://siegfried3991.github.io/ap-microeconomics-notes/#subject/literature) or [the reading and writing studio](https://siegfried3991.github.io/ap-microeconomics-notes/#literature/read).

Four units contain 12 lessons and 72 original challenges: literal comprehension/inference, diction and context, narrative perspective; imagery and comparison, sound/syntax/tone, symbolism and structure; characterisation, dialogue and power, theme and complexity; thesis, evidence/commentary, and planning/revision. Each lesson includes an original passage, worked analysis, a guided response, a teach-back prompt, and explanatory feedback. The studio adds six original passages, evidence highlighting and annotation, 20 recall cards, a quick reference, a saved study plan, and six writing tasks including comparison and a 50-minute unseen rehearsal. Drafts can be exported; self-review is not an awarded school mark.

Scope was informed by the Quarter 1 Grade 9 Honors English Literature materials reviewed on 28 October 2026: the first writing-assessment format/rubric, the September posts for *Of Mice and Men* resources and unfamiliar assessment passages, and the October benchmark procedure/rubric. The reviewed benchmark required an introduction plus at least two body paragraphs about an unseen Steinbeck passage outside *Of Mice and Men*. The original practice here is not by Steinbeck and does not predict an upcoming assessment. Comparison is additional transfer practice. The Teams Shared view did not load during the survey; this is not a complete syllabus audit. Original school attachments, student work, rosters, identities and grades are not in the public release.

Literature questions use stable `l1`–`l4` unit identifiers. Existing economics and mathematics content and identifiers are preserved. Checkpoint catalog version 7 adds bounded literature annotations, selected evidence, drafts, self-review, planner, model-assistance flags, and a practice timer. Account cleaning and backups retain every subject; old clients cannot replace an upgraded cloud checkpoint under the existing monotonic-version guard. Refresh older tabs after updating. XP/streaks span subjects; review stays in the selected subject. No new authentication settings or database permissions are needed.

Build locally with `python3 game-source/build.py`; validate with `node tests/literature.test.cjs` and the existing suites. The local reporting-service source and generated catalog are updated for version 7, including literature practice summaries without private writing. This frontend release does not deploy that separate reporting endpoint. Publication consists of the generated standalone page, public documentation, and original literature module sources; local account configuration and source class materials are excluded.


## AP Economics: direct topic practice

Open [AP Microeconomics](https://siegfried3991.github.io/ap-microeconomics-notes/#subject/microeconomics) or [AP Macroeconomics](https://siegfried3991.github.io/ap-microeconomics-notes/#subject/macroeconomics). Each topic is one button that opens a question immediately. No introductory lesson completion or separate diagnostic dashboard is required.

All six units of each AP syllabus are represented: 45 Microeconomics learning topics cover the framework's 36 topic codes, and 42 Macroeconomics topics follow its 42 codes. Each topic has original teaching notes, worked examples or reasoning guidance, 5–7 question steps, and official framework/released-paper links. The current topic sets contain 299 Microeconomics and 210 Macroeconomics steps. These are original AP-style activities, not reproduced official exam items. Related genuine released FRQs and scoring guides open on College Board's site.

There are two answer-tile tasks in each topic (174 activities). Students tap chunks into an explanation, undo/remove them, or assemble calculation working with its final result last. Independent working pieces may be placed in either order. Numerical tasks accept typed answers, fractions, scientific notation, or the number pad. An “I'm not sure” action records a miss and shows the model explanation instead of forcing a guess.

Graph work is embedded where relevant. The 25 graph views include both courses' PPC/market versions and new AD–AS, money-market, reserve-market, loanable-funds, Phillips-curve, exchange-rate, growth, business-cycle, bond-price and inflation views. Graph conditions change between attempts. The current Macroeconomics framework's limited- versus ample-reserves distinction is explicit; the simple deposit multiplier is labelled as a constrained teaching model.

First checked answers lock per attempt. Misses and notes-assisted answers prompt review; an independent pass becomes due for a retention check after three days. A small practice set is evidence about sampled questions, not an AP grade or certification of mastery. Conceptual and numerical prompts may recur on retries; answer ordering and graph conditions vary. The latest six topic attempts and each unfinished topic are saved through the existing private browser/account checkpoint, without deleting old mastery, homework, Mathematics or Literature records. Catalog version 8 protects these fields against older clients; refresh older open tabs.

Validation includes `tests/topics.test.cjs`, all previous curriculum/cloud/homework/tutor/mathematics/assessment/literature/economics suites, public configuration checks, and browser checks for one-press entry, tile construction, keypad answers, skips, reload/results restoration, and 320/390-pixel layouts. The prepared reporting API also understands the new topic evidence; it remains undeployed pending Supabase activation.
