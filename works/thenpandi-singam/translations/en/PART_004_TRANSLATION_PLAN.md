# Part 004 — English Translation Plan — தென்பாண்டிச் சிங்கம்

Status: **ENGLISH TRANSLATION PLANNING/SETUP — COMPLETE / PASS — E13 NEXT**

This is the control plan for the project-created English translation of **Part004 only**.

No English literary prose is created in this planning/setup gate.

## Authority hierarchy

1. `works/thenpandi-singam/pages/` — canonical verified Tamil; controlling authority.
2. `works/thenpandi-singam/sections/` — **PASS / CLOSED — Part004 4/4 VERIFIED** assembled Tamil reading layer.
3. `works/thenpandi-singam/translations/en/` — derived project-created English only.

If English conflicts with Tamil, canonical Tamil governs.

No published, web, remembered or standardized English translation is textual authority. English must not silently correct, regularize, modernize, fact-correct or rewrite the Tamil source layer.

## Part004 Tamil source state

Part004 is closed through Tamil archival and assembly:

- source — `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_004_pages_79-105.pdf`
- canonical scans — **79–105**
- canonical Tamil records — **27/27 verified**
- visual fidelity — **27/27 verified**
- Pass1 / Pass2A / Pass2B / Pass3 — **COMPLETE / PASS**
- whole-Part audit — **PASS / COMPLETE**
- final metadata/status synchronization — **PASS / CLOSED**
- documentation synchronization — **PASS / COMPLETE**
- Tamil archival-ready — **PASS / CLOSED**
- assembled Tamil — **PASS / CLOSED — 4/4 VERIFIED**
- assembled canonical coverage — **27/27**
- omissions / duplicates — **0 / 0**
- unsupported Tamil body insertion — **0**
- unresolved Tamil / historical-glyph / visual / status / assembly questions — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED**
- outgoing 105→106 — **PENDING direct audit / source-limited**
- Part005 canonical records — **0**

No source PDF is reopened merely for English planning or drafting.

## Live collision check

Live `main` was inspected before reserving Part004 English identifiers.

Existing English batch controls:

- `E1_SOURCE_CHECK.md` through `E12_SOURCE_CHECK.md`

Existing maintained English literary section files:

- `translations/en/sections/00-front-matter.md` through
- `translations/en/sections/17-chapter-09-part003.md`

Collision findings:

- existing English batches — **E1–E12**
- existing maintained English literary files — **18 / section_order 00–17**
- E13–E16 batch collisions — **0**
- planned section filenames 18–21 collisions — **0**

Therefore the reserved Part004 batch sequence is **E13–E16**.

## Part004 assembled Tamil source structure

Part004 contains **4 verified assembled Tamil files**:

1. `sections/18-chapter-09-part004.md` — scan79 — chapter9 continuation and close
2. `sections/19-chapter-10.md` — scans80–89 — chapter10
3. `sections/20-chapter-11.md` — scans90–101 — chapter11; scans97–98 are non-literary illustration/verso source inserts
4. `sections/21-chapter-12-part004.md` — scans102–105 — chapter12 Part004 portion, open at outgoing boundary

## Planned English batches

| Batch | Tamil assembled coverage | Planned English file | Scans |
|---|---|---|---:|
| **E13** | section18 — chapter9 Part004 continuation/close | `translations/en/sections/18-chapter-09-part004.md` | 79 |
| **E14** | section19 — chapter10 | `translations/en/sections/19-chapter-10.md` | 80–89 |
| **E15** | section20 — chapter11 | `translations/en/sections/20-chapter-11.md` | 90–101 |
| **E16** | section21 — chapter12 Part004 portion | `translations/en/sections/21-chapter-12-part004.md` | 102–105 |

Each batch must close **draft + source-check** before the next batch is considered closed.

Planned maintained Part004 English files — **4**.

Translated files at planning closure — **0/4**.  
Source-checked files at planning closure — **0/4**.

## Translation objective

Produce readable English that remains reversible to the verified Part004 Tamil evidence.

Preserve:

- narrator and speaker agency;
- chronology and information-release order;
- rhetorical questions, repetition, exclamations, sarcasm, rebuke, threat and emphatic phrasing;
- dialogue turns and paragraph structure where meaningful;
- source-visible chapter headings **10, 11, 12**;
- chapter9 continuation/close without inventing a repeated chapter heading;
- source-specific personal names, honorifics, offices, place forms and institutional labels;
- source-visible spaced/closed name variants where they carry evidence;
- the three displayed rhythmic / jati lines on scan87 as literary/display material, without explanatory interpolation;
- non-rendering physical-source provenance comments;
- scans97–98 as non-literary source inserts without invented English prose;
- Part004 terminal state at scan105 without importing or inventing scan106 wording.

Do not add explanatory history, geography, biography, caste/community interpretation, political interpretation, religious explanation or literary commentary unless the Tamil source itself supplies it.

## Continuity with frozen Part003 English

Part003 English is **FINAL CLOSED / FROZEN**.

E13 continues chapter9 from the already frozen E12 boundary:

- do not modify `translations/en/sections/17-chapter-09-part003.md`;
- do not duplicate translated scan78 text in E13;
- translate only verified Part004 scan79;
- preserve **78→79 GENUINE CONTINUATION / AUDITED** as provenance;
- carry forward established source-facing terms only when the same Tamil form recurs;
- if Part004 uses a source-visible variant, preserve the Part004 evidence rather than forcing cosmetic uniformity.

## Chapter10–12 structure locks

- E14 starts with source-visible chapter numeral **10** and stops at chapter10 close / scan89;
- E15 starts with source-visible chapter numeral **11** and stops at chapter11 close / scan101;
- scans97–98 generate **no invented English prose**; their non-rendering provenance must remain explicit;
- E16 starts with source-visible chapter numeral **12** and stops exactly at scan105;
- chapter-closing ornaments and blank lower fields generate no English prose;
- recurring page furniture is excluded from the maintained English literary layer;
- source-boundary comments remain non-rendering provenance only.

## Source-specific name / term discipline

`PART_004_GLOSSARY.md` is the active Part004 glossary.

Carry forward already source-checked project forms only where the same Tamil form recurs. Source-visible variants remain evidence and must not be silently normalized.

Any new Part004 transliteration, colonial title, military term or name handling not already locked must be established during E13–E16 source-check and recorded in the glossary rather than filled from outside knowledge.

## Source-era / colonial-title discipline

Part004 contains dialogue and narration involving `கர்னல் துரை`, `வெள்ளை அய்யர்`, English/colonial soldiers and military/political action.

Rules:

- translate only from immediate Tamil context;
- preserve narrator/speaker attribution and tone;
- do not add external colonial history or modern political interpretation;
- `துரை` may be rendered context-sensitively while preserving source register;
- do not silently replace source names/titles with externally standardized historical forms;
- do not turn source rhetoric into project commentary.

## Source-check standard

For every batch:

1. compare English against verified assembled Tamil and, where needed, canonical source-transcription blocks;
2. account for every literary paragraph/dialogue/display block;
3. preserve source order and physical-source provenance;
4. record unresolved holds explicitly;
5. require canonical Tamil edits = **0** and assembled Tamil edits = **0** unless a genuinely new upstream defect is independently demonstrated;
6. preserve 78→79 audited continuity without changing frozen Part003 English;
7. preserve scans97–98 as non-literary structural source records;
8. preserve the 105→106 source-limited boundary;
9. require Part005 leakage = **0**.

## Outgoing 105→106 lock

- scan105 remains inside chapter12;
- verified Tamil ends inside an open dialogue after `அது என்னால் முடியும்.`;
- Part005 / scan106 is unavailable;
- **105→106 = PENDING direct audit / source-limited**;
- E16 translates scans102–105 only;
- do not import, translate, paraphrase or semantically complete from scan106;
- retain a non-rendering pending-boundary provenance marker;
- English must end exactly where the verified scan105 Tamil ends.

## Post-batch Part004 gates

After E16:

1. Part004 whole-Part English glossary reconciliation across E13–E16;
2. Part004 English editorial review;
3. Part004 whole-Part bilingual review;
4. Part004 release/readiness report;
5. Part004 release-ready synchronization;
6. Part004 final closure.

Part005 canonical transcription remains blocked until Part004 final closure.

## Planning gate result

**PART004 ENGLISH TRANSLATION PLANNING/SETUP — COMPLETE / PASS**

- reserved batches — **E13–E16 / 4**
- planned maintained English files — **4**
- translated files — **0/4**
- source-checked files — **0/4**
- unresolved planning holds — **0**
- canonical Tamil edits caused by planning — **0**
- assembled Tamil edits caused by planning — **0**
- English literary prose drafted in planning — **0**
- frozen Part001–Part003 English edits — **0**
- Part005 leakage — **0**
- incoming 78→79 — **GENUINE CONTINUATION / AUDITED / frozen Part003 English unchanged**
- outgoing 105→106 — **PENDING direct audit / source-limited**

## Exact next gate

**E13 draft + source-check — section18 / scan79.**
