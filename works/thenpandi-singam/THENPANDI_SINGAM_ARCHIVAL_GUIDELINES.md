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

## Part004 whole-Part English glossary reconciliation downstream state

**PART004 WHOLE-PART ENGLISH GLOSSARY RECONCILIATION — RECONCILED / PASS.**

- scope — **E13–E16 / 4 maintained English files / scans79–105**
- maintained/source-checked English — **4/4 / 4/4**
- source coverage — **27/27 scans**
- block-count mismatches — **0**
- provenance-comment mismatches — **0**
- deliberate source-visible variants preserved — **PASS**
- accidental English source-form inconsistencies corrected — **3 occurrences**
- affected English files — **E14 / E15**
- remaining `வாளுக்கு வேலி / வாளுக்குவேலி` English variant mismatches — **0**
- canonical / assembled Tamil edits — **0 / 0**
- frozen Part001–Part003 English edits — **0**
- Part005 leakage — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- scans97–98 — **non-literary provenance only**
- 104→105 — **physical continuation preserved**
- outgoing 105→106 — **PENDING direct audit / source-limited**
- durable reconciliation — `translations/en/PART_004_GLOSSARY_RECONCILIATION.md`
- exact next activity — **Part004 English editorial review across all 4 maintained English files / scans79–105**

## Part004 English editorial review downstream state

**PART004 ENGLISH EDITORIAL REVIEW — PASS / CLOSED.**

- scope — **E13–E16 / 4 maintained English files / scans79–105**
- English-only editorial repairs — **35**
- E13 / E14 / E15 / E16 repairs — **3 / 13 / 16 / 3**
- literary/display blocks — **144 Tamil / 144 English**
- provenance comments — **25 Tamil / 25 English / EXACT**
- block-count mismatches — **0**
- provenance-comment mismatches — **0**
- source-visible glossary variant mismatches — **0**
- E14 scan87 jati lines — **3/3 unchanged**
- scans97–98 — **non-literary provenance only / 0 English prose**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- 104→105 — **physical continuation preserved**
- outgoing 105→106 — **PENDING direct audit / source-limited**
- final E16 quotation — **intentionally open / preserved**
- canonical / assembled Tamil edits — **0 / 0**
- frozen Part001–Part003 English edits — **0**
- Part005 leakage — **0**
- unresolved editorial holds — **0**
- durable review — `translations/en/PART_004_EDITORIAL_REVIEW.md`
- exact next activity — **Part004 whole-Part bilingual review across scans79–105**

## Part004 whole-Part bilingual review downstream state

**PART004 WHOLE-PART BILINGUAL REVIEW — PASS / CLOSED.**

- pairs — **4/4 PASS**
- physical source coverage — **scans79–105 / 27**
- literary/display blocks — **144 Tamil / 144 English**
- provenance comments — **25 / 25 EXACT**
- editorial repair sites rechecked — **35/35**
- further bilingual English-only corrections — **6**
- unresolved bilingual holds — **0**
- canonical / assembled Tamil edits — **0 / 0**
- frozen Part001–Part003 English edits — **0**
- Part005 leakage — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- scans97–98 — **non-literary provenance only**
- 104→105 — **physical continuation preserved**
- outgoing 105→106 — **PENDING direct audit / source-limited**
- durable review — `translations/en/PART_004_BILINGUAL_REVIEW.md`
- exact next activity — **Part004 release/readiness report**

## Part004 release/readiness and release-ready synchronization

- release/readiness — **PASS / CLOSED**
- release/readiness record — `translations/en/PART_004_RELEASE_REPORT.md`
- release-ready synchronization — **PASS / CLOSED**
- release-ready record — `PART_004_RELEASE_READY_SYNC.md`
- canonical / assembled / maintained-English body changes in these gates — **0 / 0 / 0**
- unresolved release/synchronization blockers — **0**
- outgoing 105→106 — **PENDING direct audit / source-limited**

## Part004 final closure downstream state

**PART004 FINAL CLOSURE — PASS / CLOSED / FROZEN**

- source scans — **79–105 / 27**
- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- assembled Tamil — **4/4 VERIFIED / PASS / CLOSED**
- maintained/source-checked English — **4/4 / 4/4**
- glossary reconciliation — **RECONCILED / PASS**
- English editorial review — **PASS / CLOSED**
- whole-Part bilingual review — **PASS / CLOSED**
- release/readiness — **PASS / CLOSED**
- release-ready synchronization — **PASS / CLOSED**
- unresolved closure blockers — **0**
- canonical / assembled / maintained-English body changes after release-ready sync — **0 / 0 / 0**
- Part005 leakage — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- scans97–98 — **non-literary provenance only**
- outgoing 105→106 — **PENDING direct audit / source-limited / preserved**
- final-closed Parts — **4**
- Part005 — **NEXT / AWAITING SOURCE INTAKE / NOT REGISTERED**
- exact next activity — **Part005 source intake when supplied**
- durable closure — `PART_004_FINAL_CLOSURE.md`

## Part005 source intake downstream state

**PART005 SOURCE INTAKE — COMPLETE / PASS**

- source — `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_005_pages_106-132.pdf`
- bytes — **48,768,215**
- SHA-256 — `4eaeef2e68daa5082662001f8906ca10ae207e95975a4207d3cdadd52708455b`
- local pages — **27**
- global scans — **106–132**
- registered Parts / scans — **5/18 / 132**
- canonical Part005 records — **0/27**
- active transcription Part — **Part005**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- frozen Part004 canonical / assembled / maintained-English body changes — **0 / 0 / 0**
- chapter12 continuation/close — **scans106–110**
- chapter13 opener — **scan111**
- chapter14 opener — **scan120**
- scans121–122 — **illustration / illustration-verso blank / no literary body**
- chapter15 opener — **scan130**
- last supplied scan — **132 / printed116 / chapter15 open**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- Part006 leakage — **0**
- exact next activity — **Part005 Pass1 scans116–125 / local pages11–20**
- durable intake — `SOURCE_INTAKE_PART_005.md`

## Part005 Pass1 Batch 1 downstream state

- Part005 Pass1 — **ACTIVE — 10/27 TEXT-COMPLETE**
- completed scans — **106–115 / local pages1–10**
- canonical Part005 records — **10/27**
- total canonical repository records — **115**
- status / visual fidelity — **needs-review / needs-review on 10/10**
- source-backed final reread corrections — **2 / scans112, 114**
- unresolved Pass1 holds — **0**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- scan110 — chapter12 close after source-visible English reference note
- scan111 — illustrated chapter13 opener / no visible folio
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass1 scans116–125 / local pages11–20**
- durable progress — `PART_005_PASS1_PROGRESS.md`

## Part005 Pass1 Batch 2 downstream state

- Part005 Pass1 — **ACTIVE — 20/27 TEXT-COMPLETE**
- completed scans — **106–125 / local pages1–20**
- Batch 2 — **scans116–125 / local pages11–20 / 10/10 TEXT-COMPLETE**
- canonical Part005 records — **20/27**
- total canonical repository records — **125**
- status / visual fidelity — **needs-review / needs-review on 20/20**
- scan119 — chapter13 close / three closing ornaments
- scan120 — illustrated chapter14 opener / no visible folio
- scans121–122 — **non-text illustration / verso structural records**
- 120→121–122→123 — `கூனிக் குறுகிக் / காட்சியளித்தது.` preserved with no invented bridge
- 124→125 — `அம்பலக்காரர் / மேல் என்ன குற்றம்?`
- unresolved Pass1 holds — **0**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass1 FINAL scans126–132 / local pages21–27**
- durable progress — `PART_005_PASS1_PROGRESS.md`

## Part005 Pass1 FINAL downstream state

- Part005 Pass1 — **COMPLETE / PASS — 27/27 TEXT-COMPLETE**
- completed scans — **106–132 / local pages1–27**
- canonical Part005 records — **27/27**
- total canonical repository records — **132**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- verified promotions during Pass1 — **0**
- non-literary structural records — **2 / scans121–122**
- chapter12 close — **scan110**
- chapter13 opener / close — **scans111 / 119**
- chapter14 opener / close — **scans120 / 129**
- chapter15 opener — **scan130**
- final-batch direct-source corrections — **2 / scans128, 131**
- unresolved Pass1 holds — **0**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- exact next activity — **Part005 Pass2A scans106–115 / local pages1–10**
- durable Pass1 record — `PART_005_PASS1_PROGRESS.md`

## Part005 Pass2A Batch 1 downstream state

- Part005 Pass2A — **ACTIVE — 10/27 REVIEWED**
- reviewed — **scans106–115 / local pages1–10**
- source-text correction occurrences — **3**
- affected scans — **113, 115**
- zero-correction scans — **106–112, 114**
- scans109–110 source-visible English reference note — **PASS**
- unresolved Pass2A questions — **0**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass2A scans116–125 / local pages11–20**
- durable progress — `PART_005_PASS2A_PROGRESS.md`

## Part005 Pass2A Batch 2 downstream state

- Part005 Pass2A — **ACTIVE — 20/27 REVIEWED**
- reviewed — **scans116–125 / local pages11–20**
- cumulative reviewed — **scans106–125 / local pages1–20**
- Batch 2 source-text correction occurrences — **1 / scan125**
- Batch 2 correction — `இழிந்திருக்கக்` → `இகழ்ந்திருக்கக்`
- Batch 2 zero-correction scans — **116–124**
- cumulative source-text correction occurrences — **4**
- cumulative affected scans — **113, 115, 125**
- scans121–122 structural review — **PASS / no literary text invented**
- 120→121–122→123 continuation — **PASS / no bridge wording**
- 124→125 continuation — **PASS**
- unresolved Pass2A questions — **0**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass2A FINAL scans126–132 / local pages21–27**
- durable progress — `PART_005_PASS2A_PROGRESS.md`

## Part005 Pass2A FINAL downstream state

- Part005 Pass2A — **COMPLETE / PASS — 27/27 REVIEWED**
- final batch — **scans126–132 / local pages21–27**
- final-batch source-text corrections — **3 occurrences / scans126, 131**
- final-batch correction details:
  - scan126 — `சௌக்கியமோ?` → `செளக்கியமோ?`
  - scan131 — `அனுப்பப்படுகிறது` → `அனுப்பப்படு கிறது`
  - scan131 — `வேண்டுமென்றுதான்` → `வேண்டும் மென்றுதான்`
- scan128 Pass1 note typo — `தனல்` → `தணல்`; canonical body already correct / not counted as source-text correction
- cumulative source-text correction occurrences — **7**
- cumulative affected scans — **113, 115, 125, 126, 131**
- unresolved Pass2A questions — **0**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass2B scans106–115 / local pages1–10**
- durable progress — `PART_005_PASS2A_PROGRESS.md`

## Part005 Pass2B Batch 1 downstream state

- Part005 Pass2B — **ACTIVE — 10/27 REVIEWED**
- reviewed — **scans106–115 / local pages1–10**
- lexical / spacing / punctuation corrections — **2**
- correction sites:
  - scan108 — `“மேஜர் கிரே” கொல்லப்பட்டு` → `“மேஜர் கிரே”, கொல்லப்பட்டு`
  - scan114 — `விழி இரண்டு வேல்! வேல்!` → `விழி யிரண்டும் வேல்! வேல்!`
- affected scans — **108, 114**
- zero-correction scans — **106, 107, 109, 110, 111, 112, 113, 115**
- historical-glyph corrections — **0**
- Pass2A supersessions — **0**
- scans109–110 source-visible English historical/reference note — **PASS / unchanged**
- unresolved Pass2B questions — **0**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass2B scans116–125 / local pages11–20**
- durable progress — `PART_005_PASS2B_PROGRESS.md`

## Part005 Pass2B Batch 2 downstream state

- Part005 Pass2B — **ACTIVE — 20/27 REVIEWED**
- reviewed — **scans116–125 / local pages11–20**
- cumulative reviewed — **scans106–125 / local pages1–20**
- Batch 2 lexical / spacing / punctuation corrections — **0**
- Batch 2 historical-glyph corrections — **0**
- Batch 2 Pass2A supersessions — **0**
- Batch 2 zero-correction scans — **116–125**
- cumulative Pass2B lexical / spacing / punctuation corrections — **2 / scans108, 114**
- cumulative historical-glyph corrections — **0**
- cumulative Pass2A supersessions — **0**
- scans121–122 structural review — **PASS / no literary text invented**
- 120→121–122→123 continuation — **PASS / no bridge wording**
- 124→125 continuation — **PASS**
- scan125 Pass2A `இகழ்ந்திருக்கக்` — **PASS / retained**
- unresolved Pass2B questions — **0**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass2B FINAL scans126–132 / local pages21–27**
- durable progress — `PART_005_PASS2B_PROGRESS.md`

## Part005 Pass2B FINAL downstream state

- Part005 Pass2B — **COMPLETE / PASS — 27/27 REVIEWED**
- final batch — **scans126–132 / local pages21–27**
- final-batch lexical / spacing / punctuation corrections — **2 / scan131**
- final-batch correction details:
  - scan131 — `வேண்டும் மென்றுதான்` → `வேண்டு மென்றுதான்` — source-visible line-break form / **fresh Pass2B supersedes Pass2A**
  - scan131 — `குதிரை சாட்டு வேண்டாமென்று` → `குதிரை சாரட்டு வேண்டாமென்று` — source lexical form
- cumulative Pass2B lexical / spacing / punctuation corrections — **4 / scans108, 114, 131**
- cumulative historical-glyph corrections — **0**
- cumulative Pass2A supersessions — **1 / scan131**
- zero-correction Pass2B scans — **24**
- scan129 chapter14 close / three ornaments — **PASS**
- scan130 illustrated chapter15 opener / no source-visible folio — **PASS**
- scan131 `அனுப்பப்படு கிறது` — **PASS / retained**
- scan132 terminal open dialogue — **PASS**
- unresolved Pass2B questions — **0**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass3 scans106–115 / local pages1–10**
- durable progress — `PART_005_PASS2B_PROGRESS.md`

## Part005 Pass3 Batch 1 downstream state

- Part005 Pass3 — **ACTIVE — 10/27 REVIEWED**
- reviewed — **scans106–115 / local pages1–10**
- Pass3 textual corrections — **0**
- unresolved visual / structural questions — **0**
- scan110 — English reference-note continuation + chapter12 close + three ornaments + intentional blank lower field — **PASS**
- scan111 — illustrated chapter13 opener / displayed numeral 13 / mounted-warrior illustration / no source-visible folio — **PASS**
- scans109–110 English historical/reference note placement and page structure — **PASS / text unchanged**
- scan115 stamp / handwritten marks — **physical annotations only / not canonical prose**
- 105→106 — **PASS**
- 108→109 — **PASS**
- 109→110 — **PASS**
- 112→113 — **PASS**
- 114→115 — **PASS**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass3 scans116–125 / local pages11–20**
- durable progress — `PART_005_PASS3_PROGRESS.md`

## Part005 Pass3 Batch 2 downstream state

- Part005 Pass3 — **ACTIVE — 20/27 REVIEWED**
- reviewed — **scans116–125 / local pages11–20**
- cumulative reviewed — **scans106–125 / local pages1–20**
- Pass3 textual corrections — **0**
- unresolved visual / structural questions — **0**
- scan119 — chapter13 close / three ornaments — **PASS**
- scan120 — illustrated chapter14 opener / displayed numeral 14 / mounted-warrior illustration / no source-visible folio — **PASS**
- scans121–122 — non-literary illustration / illustration-verso — **STRUCTURAL PASS / no literary text invented**
- 120→121–122→123 — `கூனிக் குறுகிக் / காட்சியளித்தது.` — **PASS / no bridge wording**
- 124→125 — `அம்பலக்காரர் / மேல் என்ன குற்றம்?` — **PASS**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 Pass3 FINAL scans126–132 / local pages21–27**
- durable progress — `PART_005_PASS3_PROGRESS.md`

## Part005 Pass3 FINAL downstream state

- Part005 Pass3 — **COMPLETE / PASS — 27/27 REVIEWED**
- final batch — **scans126–132 / local pages21–27**
- Pass3 textual corrections — **0**
- unresolved visual / structural questions — **0**
- scan128 internal imagined-speech display / quotation hierarchy — **PASS**
- scan129 chapter14 close / three centered ornaments — **PASS**
- scan130 illustrated chapter15 opener / displayed numeral 15 / mounted-warrior illustration / no source-visible folio — **PASS**
- scan132 terminal open dialogue — **PASS**
- 126→127 — **PASS**
- 128→129 — **PASS**
- 129→130 chapter14→15 transition — **PASS**
- 130→131 — **PASS**
- 131→132 — **PASS**
- status / visual fidelity — **needs-review / needs-review on 27/27**
- status promotions — **0**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 whole-Part audit — scans106–132 / local pages1–27**
- durable progress — `PART_005_PASS3_PROGRESS.md`

## Part005 whole-Part audit downstream state

- Part005 whole-Part audit — **PASS / COMPLETE**
- canonical coverage — **27/27 / scans106–132**
- duplicate / omitted canonical scans — **0 / 0**
- `part_page` continuity — **1–27 / PASS**
- source-filename consistency — **27/27**
- Pass1 / Pass2A / Pass2B / Pass3 evidence — **27/27 / 27/27 / 27/27 / 27/27**
- Pass2A corrections — **7 occurrences / scans113, 115, 125, 126, 131**
- Pass2B corrections — **4 occurrences / scans108, 114, 131**
- historical-glyph corrections — **0**
- Pass2A supersessions — **1 / scan131**
- unresolved Tamil / glyph / visual / structural questions — **0**
- unsupported body insertion — **0**
- audit/review-note leakage into literary transcription — **0**
- page-status promotions during audit — **0**
- status / visual fidelity remain — **needs-review / needs-review on 27/27**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- exact next activity — **Part005 final metadata/status synchronization — scans106–132 / 27 pages**
- durable audit — `PART_005_AUDIT.md`

## Part005 final metadata/status downstream state

- Part005 final metadata/status synchronization — **PASS / CLOSED**
- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- page-map verified rows — **27/27**
- needs-review Tamil / visual pages — **0 / 0**
- canonical Tamil body changes caused by status sync — **0**
- unresolved Tamil / glyph / visual / structural questions — **0**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- frozen Parts001–004 body edits — **0**
- Part006 leakage — **0**
- exact next activity — **Part005 documentation synchronization**
- durable status sync — `PART_005_FINAL_STATUS_SYNC.md`

## Part005 documentation synchronization downstream state

- Part005 documentation synchronization — **PASS / COMPLETE**
- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- page-map verified rows — **27/27**
- needs-review Tamil / visual pages — **0 / 0**
- Pass1 / Pass2A / Pass2B / Pass3 — **all COMPLETE / PASS**
- whole-Part audit — **PASS / COMPLETE**
- final metadata/status synchronization — **PASS / CLOSED**
- unresolved Tamil / glyph / visual / structural / documentation blockers — **0**
- canonical Part005 page-file changes caused by documentation sync — **0**
- canonical Tamil/body changes caused by documentation sync — **0**
- verified status-field changes caused by documentation sync — **0**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- frozen Parts001–004 body changes — **0**
- Part006 leakage — **0**
- exact next activity — **Part005 Tamil archival-ready checkpoint**
- durable documentation sync — `PART_005_DOCUMENTATION_SYNC.md`

## Part005 Tamil archival-ready downstream state

- Part005 Tamil archival-ready — **PASS / CLOSED**
- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- needs-review Tamil / visual pages — **0 / 0**
- page-map verified rows — **27/27**
- Pass1 / Pass2A / Pass2B / Pass3 — **all COMPLETE / PASS**
- whole-Part audit — **PASS / COMPLETE**
- final metadata/status synchronization — **PASS / CLOSED**
- documentation synchronization — **PASS / COMPLETE**
- unresolved Tamil / glyph / visual / structural / documentation blockers — **0**
- canonical Part005 page-file changes caused by checkpoint — **0**
- canonical Tamil/body changes caused by checkpoint — **0**
- verified status-field changes caused by checkpoint — **0**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- frozen Parts001–004 body changes — **0**
- Part006 leakage — **0**
- exact next activity — **Part005 assembled Tamil construction + audit**
- durable archival-ready checkpoint — `PART_005_TAMIL_ARCHIVAL_READY.md`

## Part005 assembled Tamil downstream state

**PART005 ASSEMBLED TAMIL — COMPLETE / PASS / CLOSED — 4/4 VERIFIED.**

- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- scans — **106–132 / 27**
- assembled files — **4/4 VERIFIED**
- inventory — `22-chapter-12-part005.md`, `23-chapter-13.md`, `24-chapter-14.md`, `25-chapter-15-part005.md`
- canonical source-transcription records accounted — **27/27**
- non-empty canonical source-transcription blocks represented — **25/25**
- non-literary records — **2 / scans121–122 / provenance only**
- omissions / duplicates — **0 / 0**
- unsupported Tamil body insertion — **0**
- audit/review/workflow-note leakage — **0**
- canonical page mutations caused by assembly — **0**
- frozen Parts001–004 assembled Tamil changes — **0**
- Part006 leakage — **0**
- unresolved assembly blockers — **0**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- exact next activity — **Part005 English translation planning/setup — reserve E17–E20**
- durable validation — `PART_005_ASSEMBLED_TAMIL_VALIDATION.md`

## Part005 English planning downstream state

**PART005 ENGLISH TRANSLATION PLANNING / SETUP — COMPLETE / PASS.**

- live collision check — **PASS**
- existing batch controls before setup — **E1–E16**
- existing maintained English section orders before setup — **00–21**
- reserved Part005 batches — **E17–E20**
- planned maintained English files — **4**
- batch/file mapping — **E17→22 / E18→23 / E19→24 / E20→25**
- translated/source-checked at planning closure — **0/4 / 0/4**
- English literary prose drafted during planning — **0**
- unresolved planning / glossary holds — **0**
- canonical Tamil edits caused by planning — **0**
- assembled Tamil edits caused by planning — **0**
- frozen Parts001–004 English edits — **0**
- scans109–110 source-visible English note — **source material / preserve without modernization**
- scans121–122 — **non-literary provenance only / 0 planned English prose**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- Part006 leakage — **0**
- exact next gate — **E17 draft + source-check — section22 / scans106–110**
- durable controls — `translations/en/PART_005_TRANSLATION_PLAN.md`, `PART_005_GLOSSARY.md`, `PART_005_PROGRESS.md`

## Part005 E17 English downstream state

**E17 — SOURCE-CHECKED / COMPLETE.**

- English file — `translations/en/sections/22-chapter-12-part005.md`
- Tamil authority — `sections/22-chapter-12-part005.md`
- source scans — **106–110**
- cumulative Part005 translated/source-checked — **1/4 / 1/4**
- Tamil / English literary-source blocks — **23 / 23**
- provenance comments — **5 / 5**
- source-visible English note on scans109–110 — **EXACT / preserved as source-language material**
- omitted / duplicated blocks — **0 / 0**
- unresolved E17 source-check holds — **0**
- canonical / assembled Tamil edits caused by E17 — **0 / 0**
- frozen Parts001–004 English edits — **0**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- Part006 leakage — **0**
- exact next gate — **E18 draft + source-check — section23 / scans111–119**
- durable source-check — `translations/en/E17_SOURCE_CHECK.md`
