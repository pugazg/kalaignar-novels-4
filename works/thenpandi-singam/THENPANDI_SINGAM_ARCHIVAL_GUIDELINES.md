# தென்பாண்டிச் சிங்கம் — Part-by-Part Archival Guidelines

## Controlling-source rule

The user-supplied split PDFs are the controlling source.

Preserve source-visible:

- wording and word boundaries;
- punctuation and quotation/dialogue structure;
- paragraphing and displayed text;
- historical glyph identity and source-era orthography;
- printed pagination;
- illustrations, blank areas and non-text matter;
- physical scan order;
- genuine continuations across split boundaries.

Do not silently modernize, normalize, spell-correct or semantically complete a source reading.

If a character or glyph cannot be established from the source image, record a source-limited/needs-review condition instead of guessing.

## Source packaging

The user reports **18 split PDF files**, each no larger than **50 MB**.

Until each file is attached and inspected, do **not** invent:

- exact filenames;
- byte sizes;
- SHA-256 hashes;
- local page counts;
- global scan boundaries;
- printed-page ranges;
- source-family/catalogue identifiers;
- edition/year metadata;
- split-boundary classifications.

These belong in `SOURCE_PART_REGISTRY.md` and the corresponding `SOURCE_INTAKE_PART_NNN.md`.

## Canonical numbering

- `scan_page` is the global physical scan number across the complete work.
- It starts with the first physical scan in Part001 and never resets.
- `part` identifies the split file number.
- `part_page` is the local physical page within that split file.
- `printed_page` records only a source-visible printed folio; use null/— when absent or not established.
- Never infer printed pagination from sequence alone when the folio is not visible.

## Mandatory Part lock

> **Finish the entire maintained workflow for the active Part before beginning canonical transcription of the next Part.**

A later Part may be inspected only as an adjacent boundary witness when required to classify the active Part's outgoing split boundary.

Boundary-witness text is not canonical text for the later Part and must not be imported into the active Part.

## Tamil workflow

For every Part:

1. **Source intake**
   - exact filename
   - local physical extent
   - global scan mapping
   - byte size
   - SHA-256
   - source representation/text-layer note
   - first/last scan inspection
   - incoming/outgoing boundary state where evidence exists
2. **Pass 1 — complete physical capture/transcription**
   - create one canonical page record per physical scan
   - capture all source-visible textual matter
   - record illustrations/non-text pages and blanks structurally
   - keep `status: needs-review` and `visual_fidelity: needs-review`
3. **Pass 2A — direct textual verification**
   - word-for-word source comparison
   - punctuation, paragraph/dialogue and printed-pagination verification
   - log every source-supported correction
4. **Pass 2B — independent lexical/historical-glyph reread**
   - lexical segmentation and spacing
   - source-era forms
   - historical glyph identity
   - punctuation-sensitive reread
   - do not normalize a source form for familiarity
5. **Pass 3 — visual/structural verification**
   - full-page image comparison
   - headings, chapter openings/closings
   - blank lower fields
   - illustrations and spreads
   - page furniture and reading order
6. **Whole-Part audit**
   - continuous physical coverage
   - no duplicate/omitted canonical scan records
   - printed-page mapping reconciled
   - Pass2A/2B/3 evidence complete
   - split boundaries reconciled
   - unresolved questions explicitly counted
7. **Final metadata/status synchronization**
   - promote to `verified` only after the Part audit passes
   - do not alter canonical Tamil merely as a side effect of status promotion
8. **Documentation synchronization**
   - README/HANDOVER/registry/page-map and active Part records agree
9. **Tamil archival-ready checkpoint**
   - canonical Tamil and visual fidelity closed
   - unresolved Tamil/glyph/visual/structural blockers = 0, except explicitly source-limited conditions
10. **Assembled Tamil construction + audit**
    - derive only from verified canonical `pages/`
    - preserve chapter/section structure
    - omissions = 0; duplicates = 0
    - canonical page mutations caused by assembly = 0

## English workflow

English begins only after the active Part's assembled Tamil has closed.

For every Part:

1. translation planning/setup;
2. assign non-colliding English batch IDs;
3. create Part glossary and progress controls;
4. draft one maintained English section/batch at a time;
5. source-check each English batch against verified Tamil;
6. whole-Part glossary reconciliation;
7. English editorial review;
8. whole-Part bilingual review;
9. release/readiness report;
10. release-ready synchronization;
11. final closure — **PASS / CLOSED / FROZEN**.

English is project-created and derived. Canonical Tamil always governs.

Do not use a published, web, remembered or standard English translation as textual authority.

## Boundary rule

A split boundary is classified only from the two adjacent physical source scans.

Permitted durable classes include, where source evidence supports them:

- `CLEAN / AUDITED`
- `GENUINE CONTINUATION / AUDITED`
- another explicitly described source-supported structural state.

Never reconstruct missing text across a split. If the next Part has not been supplied, the outgoing boundary remains **PENDING direct audit**.

## Canonical page-record baseline

A body-page record should use this structure, with actual values filled only from source evidence:

```yaml
---
scan_page: <global physical scan>
part: <1-18>
part_page: <local physical page>
printed_page: <visible folio or null>
work: "thenpandi-singam"
section: "<source-visible section/chapter label or structural label>"
page_type: "<body|front-matter|illustration|blank|other source-supported type>"
status: "needs-review"
visual_fidelity: "needs-review"
language: "ta"
source_filename: "<exact attached filename>"
transcription_method: "direct source-image transcription; PartNNN Pass 1"
---
```

Then use:

- `# <section/chapter heading>` only when structurally appropriate;
- `## Source transcription`;
- exact source transcription;
- `## Pass 1 notes`;
- later formal Pass2A / Pass2B / Pass3 review blocks.

Do not mark a newly transcribed page `verified`.

## Freeze rule

Once a Part reaches **FINAL CLOSED / FROZEN**, do not reopen canonical Tamil, assembled Tamil or maintained English merely for stylistic polishing.

A frozen Part changes only when a genuine source/evidence defect is demonstrated and the correction is explicitly tracked through the required controls.

## Current frontier

- Part001 source — **REGISTERED / COMPLETE / PASS**
- Part001 source file — `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_001_pages_1-26.pdf`
- Part001 global scans — **1–26**
- Part001 canonical records — **26/26 — scans1–26**
- Part001 Pass1 — **COMPLETE / PASS — 26/26 TEXT-COMPLETE**
- Part001 Pass2A — **COMPLETE / PASS — 26/26 REVIEWED — 14 source-text corrections; 0 unresolved**
- Part001 Pass2B — **COMPLETE / PASS — 26/26 REVIEWED — 5 lexical/spacing/punctuation corrections; 0 historical-glyph corrections; 0 unresolved**
- Part001 Pass3 — **COMPLETE / PASS — 26/26 REVIEWED — 0 textual corrections / 0 unresolved**
- Part001 Part audit — **PASS / COMPLETE**
- Part001 final metadata/status synchronization — **PASS / CLOSED**
- Part001 documentation synchronization — **PASS / COMPLETE**
- Part001 Tamil archival-ready — **PASS / CLOSED**
- Part001 assembled Tamil — **10/10 VERIFIED / PASS / CLOSED**
- Part001 assembled canonical coverage — **26/26**
- Part001 English planning/setup — **COMPLETE / PASS**
- Part001 reserved English batches — **E1–E4**
- Part001 planned English files — **10**
- Part001 English E1–E4 — **SOURCE-CHECKED / COMPLETE**
- Part001 English source coverage — **scans1–26**
- Part001 English glossary reconciliation — **RECONCILED / PASS**
- Part001 glossary files changed / terminology corrections — **4 / 7**
- Part001 unresolved glossary holds — **0**
- Part001 English editorial review — **PASS / CLOSED**
- Part001 editorial files reviewed / edited — **10 / 9**
- Part001 English-only editorial corrections — **24**
- Part001 unresolved editorial holds — **0**
- Part001 whole-Part bilingual review — **PASS / CLOSED**
- Part001 bilingual English-only corrections — **1**
- Part001 unresolved bilingual holds — **0**
- Part001 release/readiness — **PASS / CLOSED**
- Part001 unresolved release/readiness blockers — **0**
- Part001 release-ready synchronization — **PASS / CLOSED**
- Part001 final closure — **PASS / CLOSED / FROZEN**
- final-closed Parts — **2**
- active transcription Part — **Part003**
- Part002 source intake — **COMPLETE / PASS**
- Part002 global scans — **27–53**
- Part002 incoming 26→27 — **GENUINE CONTINUATION / AUDITED**
- Part002 outgoing / Part003 incoming 53→54 — **GENUINE CONTINUATION / AUDITED**
- Part002 Pass1 — **COMPLETE / PASS — 27/27 TEXT-COMPLETE**
- Part002 Pass2A — **COMPLETE / PASS — 27/27 REVIEWED — 1 correction / 0 unresolved**
- Part002 Pass2B — **COMPLETE / PASS — 27/27 REVIEWED — 5 lexical/spacing/punctuation corrections / 0 historical-glyph corrections / 0 unresolved**
- Part002 Pass3 — **COMPLETE / PASS — 27/27 REVIEWED — 0 textual corrections / 0 unresolved visual-structural questions**
- Part002 Part audit — **PASS / COMPLETE**
- Part002 final metadata/status synchronization — **PASS / CLOSED — 27/27 verified Tamil + visual**
- Part002 documentation synchronization — **PASS / COMPLETE**
- Part002 Tamil archival-ready — **PASS / CLOSED**
- Part002 assembled Tamil — **4/4 VERIFIED / PASS / CLOSED — 27/27 canonical coverage**
- Part002 English planning/setup — **COMPLETE / PASS — E5–E8 reserved / 4 planned files**
- Part002 E5–E8 — **SOURCE-CHECKED / COMPLETE — 4/4 translated / 4/4 source-checked / 0 holds**
- Part002 English glossary reconciliation — **RECONCILED / PASS — 1/4 files changed / 9 terminology corrections / 0 holds**
- Part002 English editorial review — **PASS / CLOSED — 4/4 reviewed / 4/4 edited / 27 corrections / 0 holds**
- Part002 whole-Part bilingual review — **PASS / CLOSED — 4/4 pairs / 3 further English-only corrections / 0 holds**
- Part002 release/readiness — **PASS / CLOSED — 0 blockers / 0 body changes**
- Part002 release-ready synchronization — **PASS / CLOSED — 0 post-release body drift**
- Part002 final closure — **PASS / CLOSED / FROZEN**
- final-closed Parts — **2**
- Part003 — **ACTIVE / ENGLISH PLANNING COMPLETE — E9 NEXT**
- Part001 unresolved English source-check holds — **0**
- Part001 translated/source-checked English files — **10/10 / 10/10**
- Part001 canonical Tamil — **26/26 verified**
- Part001 visual fidelity — **26/26 verified**
- outgoing 26→27 — **GENUINE CONTINUATION / AUDITED**
- Parts004–018 source metadata — **PENDING**
- Part002 canonical records — **27/27**
- Part003 source — `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_003_pages_54-78.pdf`
- Part003 local pages / global scans — **25 / 54–78**
- Part003 canonical records — **25/25**
- Part003 incoming 53→54 — **GENUINE CONTINUATION / AUDITED**
- Part003 outgoing 78→79 — **PENDING direct audit / source-limited**
- Part003 Pass1 — **COMPLETE / PASS — 25/25 TEXT-COMPLETE — scans54–78**
- Part003 Pass2A — **COMPLETE / PASS — 25/25 REVIEWED — 19 corrections / 0 unresolved**
- Part003 Pass2B — **COMPLETE / PASS — 25/25 REVIEWED — 5 lexical/spacing/punctuation corrections / 0 historical-glyph corrections / 0 unresolved**
- Part003 Pass3 — **COMPLETE / PASS — 25/25 REVIEWED — 0 textual corrections / 0 unresolved visual-structural questions**
- Part003 verified Tamil / visual pages — **25/25 / 25/25**
- exact next activity — **Part003 whole-Part audit scans54–78 / local pages1–25**


## Part003 whole-Part audit downstream state

- Part003 whole-Part audit — **PASS / COMPLETE**
- canonical coverage — **25/25 / scans54–78**
- duplicate / omitted scans — **0 / 0**
- unresolved Tamil / glyph / visual / structural questions — **0**
- page status promotions during audit — **0**
- outgoing 78→79 — **PENDING direct audit / source-limited**
- exact next activity — **Part003 final metadata/status synchronization — scans54–78 / 25 pages**
- durable audit — `PART_003_AUDIT.md`


## Part003 final metadata/status downstream state

- Part003 final metadata/status synchronization — **PASS / CLOSED**
- canonical Tamil — **25/25 verified**
- visual fidelity — **25/25 verified**
- needs-review Tamil / visual pages — **0 / 0**
- canonical Tamil body changes caused by status sync — **0**
- outgoing 78→79 — **PENDING direct audit / source-limited**
- exact next activity — **E9 draft + source-check — section14 / scan54**
- durable status sync — `PART_003_FINAL_STATUS_SYNC.md`


## Part003 documentation synchronization downstream state

- Part003 documentation synchronization — **PASS / COMPLETE**
- canonical Tamil — **25/25 verified**
- visual fidelity — **25/25 verified**
- page-map verified rows — **25/25**
- unresolved Tamil/glyph/visual/structural/documentation blockers — **0**
- outgoing 78→79 — **PENDING direct audit / source-limited**
- exact next activity — **E9 draft + source-check — section14 / scan54**
- durable documentation sync — `PART_003_DOCUMENTATION_SYNC.md`


## Part003 Tamil archival-ready downstream state

- Part003 Tamil archival-ready — **PASS / CLOSED**
- canonical Tamil — **25/25 verified**
- visual fidelity — **25/25 verified**
- needs-review Tamil / visual pages — **0 / 0**
- unresolved Tamil/glyph/visual/structural/documentation blockers — **0**
- outgoing 78→79 — **PENDING direct audit / source-limited**
- exact next activity — **E9 draft + source-check — section14 / scan54**
- durable archival-ready checkpoint — `PART_003_TAMIL_ARCHIVAL_READY.md`


## Part003 assembled Tamil downstream state

**PART003 ASSEMBLED TAMIL — COMPLETE / PASS / CLOSED — 4/4 VERIFIED.**

- canonical Tamil — **25/25 verified**
- visual fidelity — **25/25 verified**
- scans — **54–78**
- Part003 assembled files — **4/4 VERIFIED**
- inventory — `14-chapter-06-part003.md`, `15-chapter-07.md`, `16-chapter-08.md`, `17-chapter-09-part003.md`
- canonical scan coverage — **25/25**
- omissions / duplicates — **0 / 0**
- unsupported Tamil body insertion — **0**
- audit/review-note leakage — **0**
- canonical page mutations caused by assembly — **0**
- frozen Part001/Part002 assembled Tamil changes — **0**
- Part004 leakage — **0**
- unresolved assembly blockers — **0**
- incoming 53→54 — **GENUINE CONTINUATION / AUDITED**
- outgoing 78→79 — **PENDING direct audit / source-limited**
- exact next gate — **E9 draft + source-check — section14 / scan54**
- durable validation — `PART_003_ASSEMBLED_TAMIL_VALIDATION.md`


## Part003 English planning downstream state

**PART003 ENGLISH TRANSLATION PLANNING/SETUP — COMPLETE / PASS.**

- reserved batches — **E9–E12 / 4**
- planned maintained English files — **4**
- batch map — **E9 section14/scan54; E10 section15/scans55–61; E11 section16/scans62–70; E12 section17/scans71–78**
- translated/source-checked — **0/4 / 0/4**
- unresolved planning holds — **0**
- canonical / assembled Tamil edits caused by planning — **0 / 0**
- frozen Part001/Part002 English edits — **0**
- English literary prose drafted in planning — **0**
- Part004 leakage — **0**
- incoming 53→54 — **GENUINE CONTINUATION / AUDITED**
- outgoing 78→79 — **PENDING direct audit / source-limited**
- exact next gate — **E9 draft + source-check — section14 / scan54**
- durable controls — `translations/en/PART_003_TRANSLATION_PLAN.md`, `PART_003_GLOSSARY.md`, `PART_003_PROGRESS.md`


## Part003 E9–E12 English downstream state

- E9–E12 — **SOURCE-CHECKED / COMPLETE**
- maintained Part003 English files — **4/4**
- translated/source-checked — **4/4 / 4/4**
- physical source coverage — **scans54–78 / 25**
- unresolved English source-check holds — **0**
- canonical / assembled Tamil edits caused by English — **0 / 0**
- frozen Part001/Part002 English edits — **0**
- Part004 leakage — **0**
- outgoing 78→79 — **PENDING direct audit / source-limited / preserved**
- exact next gate — **Part003 whole-Part English glossary reconciliation across E9–E12**
- durable source-check controls — `translations/en/E9_SOURCE_CHECK.md` through `E12_SOURCE_CHECK.md`


## Part003 final closure downstream state

**PART003 FINAL CLOSURE — PASS / CLOSED / FROZEN**

- canonical Tamil — **25/25 verified**
- visual fidelity — **25/25 verified**
- assembled Tamil — **4/4 VERIFIED / PASS / CLOSED**
- maintained/source-checked English — **4/4 / 4/4**
- glossary reconciliation — **RECONCILED / PASS**
- English editorial review — **PASS / CLOSED**
- whole-Part bilingual review — **PASS / CLOSED**
- release/readiness — **PASS / CLOSED**
- release-ready synchronization — **PASS / CLOSED**
- unresolved closure blockers — **0**
- outgoing 78→79 — **PENDING direct audit / source-limited / preserved**
- Part004 leakage — **0**
- final-closed Parts — **3**
- exact next activity — **Part004 source intake when supplied**
- durable closure — `PART_003_FINAL_CLOSURE.md`

## Part004 documentation synchronization state

- Part004 documentation synchronization — **PASS / COMPLETE**
- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- page-map verified rows — **27/27**
- Pass1 — **COMPLETE / PASS — 27/27 TEXT-COMPLETE**
- Pass2A — **COMPLETE / PASS — 27/27 REVIEWED — 9 corrections / 0 unresolved**
- Pass2B — **COMPLETE / PASS — 27/27 REVIEWED — 19 lexical/spacing/punctuation corrections / 0 historical-glyph corrections / 0 unresolved**
- Pass3 — **COMPLETE / PASS — 27/27 REVIEWED — 0 textual corrections / 0 unresolved visual-structural questions**
- whole-Part audit — **PASS / COMPLETE**
- final metadata/status synchronization — **PASS / CLOSED**
- unresolved Tamil/glyph/visual/structural/documentation blockers — **0**
- canonical Tamil/body changes caused by documentation sync — **0**
- frozen Part001–Part003 body changes — **0**
- Part005 leakage — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- outgoing 105→106 — **PENDING direct audit / source-limited**
- exact next activity — **Part004 Tamil archival-ready checkpoint**
- durable documentation sync — `PART_004_DOCUMENTATION_SYNC.md`

## Part004 Tamil archival-ready downstream state

- Part004 Tamil archival-ready — **PASS / CLOSED**
- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- needs-review Tamil / visual pages — **0 / 0**
- page-map verified rows — **27/27**
- unresolved Tamil/glyph/visual/structural/documentation blockers — **0**
- canonical Tamil/body changes caused by checkpoint — **0**
- frozen Part001–Part003 body changes — **0**
- Part005 leakage — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- outgoing 105→106 — **PENDING direct audit / source-limited**
- exact next activity — **Part004 assembled Tamil construction + audit**
- durable archival-ready checkpoint — `PART_004_TAMIL_ARCHIVAL_READY.md`

## Part004 assembled Tamil downstream state

**PART004 ASSEMBLED TAMIL — COMPLETE / PASS / CLOSED — 4/4 VERIFIED.**

- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- scans — **79–105**
- assembled files — **4/4 VERIFIED**
- inventory — `18-chapter-09-part004.md`, `19-chapter-10.md`, `20-chapter-11.md`, `21-chapter-12-part004.md`
- canonical scan coverage — **27/27**
- omissions / duplicates — **0 / 0**
- unsupported Tamil body insertion — **0**
- audit/review-note leakage — **0**
- canonical page mutations caused by assembly — **0**
- frozen Part001–Part003 assembled Tamil changes — **0**
- Part005 leakage — **0**
- unresolved assembly blockers — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- outgoing 105→106 — **PENDING direct audit / source-limited**
- exact next activity — **Part004 English translation planning/setup — reserve E13–E16**
- durable validation — `PART_004_ASSEMBLED_TAMIL_VALIDATION.md`

## Part004 English planning downstream state

**PART004 ENGLISH TRANSLATION PLANNING/SETUP — COMPLETE / PASS.**

- reserved batches — **E13–E16 / 4**
- planned maintained English files — **4**
- batch map — **E13 section18/scan79; E14 section19/scans80–89; E15 section20/scans90–101; E16 section21/scans102–105**
- translated/source-checked — **0/4 / 0/4**
- unresolved planning holds — **0**
- English literary prose drafted during planning — **0**
- canonical / assembled Tamil edits caused by planning — **0 / 0**
- frozen Part001–Part003 English edits — **0**
- Part005 leakage — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- outgoing 105→106 — **PENDING direct audit / source-limited**
- exact next gate — **E13 draft + source-check — section18 / scan79**
- durable controls — `translations/en/PART_004_TRANSLATION_PLAN.md`, `translations/en/PART_004_GLOSSARY.md`, `translations/en/PART_004_PROGRESS.md`

