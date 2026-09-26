# Part 005 — English Translation Plan — தென்பாண்டிச் சிங்கம்

Status: **PLANNING / SETUP — COMPLETE / PASS**

This is the control plan for the project-created English translation of **Part005 only**.

No English literary prose is created in this planning/setup gate.

## Authority hierarchy

1. `works/thenpandi-singam/pages/` — canonical verified Tamil; controlling authority.
2. `works/thenpandi-singam/sections/` — **PASS / CLOSED — Part005 4/4 VERIFIED** assembled Tamil reading layer.
3. `works/thenpandi-singam/translations/en/` — derived project-created English only.

If English conflicts with Tamil, canonical Tamil governs.

No published, web, remembered or standardized English translation is textual authority. English must not silently correct, regularize, modernize, fact-correct or rewrite the Tamil source layer.

## Part005 Tamil source state

Part005 is closed through Tamil archival and assembly:

- source — `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_005_pages_106-132.pdf`
- canonical scans — **106–132**
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
- unresolved Tamil / glyph / visual / status / assembly questions — **0**
- incoming 105→106 — **GENUINE CONTINUATION / AUDITED**
- outgoing 132→133 — **PENDING direct audit / source-limited**
- Part006 canonical records — **0**

No source PDF is reopened merely for English planning or drafting.

## Live collision check

Live `main` was inspected before reserving Part005 English identifiers.

Existing English batch controls:

- `E1_SOURCE_CHECK.md` through `E16_SOURCE_CHECK.md`
- **E17–E20 absent**

Existing maintained English literary section files:

- `translations/en/sections/00-front-matter.md` through
- `translations/en/sections/21-chapter-12-part004.md`
- planned section orders **22–25 absent**

Collision findings:

- existing English batches — **E1–E16**
- existing maintained English literary files — **22 / section_order 00–21**
- E17–E20 batch collisions — **0**
- planned section filenames 22–25 collisions — **0**

Therefore the reserved Part005 batch sequence is **E17–E20**.

## Part005 assembled Tamil source structure

Part005 contains **4 verified assembled Tamil files**:

1. `sections/22-chapter-12-part005.md` — scans106–110 — chapter12 Part005 continuation and close
2. `sections/23-chapter-13.md` — scans111–119 — chapter13
3. `sections/24-chapter-14.md` — scans120–129 — chapter14; scans121–122 are non-literary illustration / verso provenance only
4. `sections/25-chapter-15-part005.md` — scans130–132 — chapter15 Part005 portion, open at outgoing boundary

## Planned English batches

| Batch | Tamil assembled coverage | Planned English file | Scans |
|---|---|---|---:|
| **E17** | section22 — chapter12 Part005 continuation/close | `translations/en/sections/22-chapter-12-part005.md` | 106–110 |
| **E18** | section23 — chapter13 | `translations/en/sections/23-chapter-13.md` | 111–119 |
| **E19** | section24 — chapter14 | `translations/en/sections/24-chapter-14.md` | 120–129 |
| **E20** | section25 — chapter15 Part005 portion | `translations/en/sections/25-chapter-15-part005.md` | 130–132 |

Each batch must close **draft + source-check** before the next batch is considered closed.

Planned maintained Part005 English files — **4**.

Translated files at planning closure — **0/4**.  
Source-checked files at planning closure — **0/4**.

## Translation objective

Produce readable English that remains reversible to the verified Part005 Tamil evidence.

Preserve:

- narrator and speaker agency;
- chronology and information-release order;
- rhetorical questions, repetition, exclamations, sarcasm, rebuke, threat and emphatic phrasing;
- dialogue turns and paragraph structure where meaningful;
- source-visible chapter headings **13, 14, 15**;
- chapter12 continuation/close without inventing a repeated chapter heading;
- source-specific personal names, honorifics, offices, place forms and institutional labels;
- source-visible spacing / closed-form / colloquial variants where they carry evidence;
- displayed song / dance text as literary/display material without explanatory interpolation;
- non-rendering physical-source provenance comments;
- scans121–122 as non-literary source inserts without invented English prose;
- Part005 terminal state at scan132 without importing or inventing scan133 wording.

Do not add explanatory history, geography, biography, caste/community interpretation, political interpretation, religious explanation or literary commentary unless the Tamil source itself supplies it.

## Continuity with frozen Part004 English

Part004 English is **FINAL CLOSED / FROZEN**.

E17 continues chapter12 from the already frozen E16 boundary:

- do not modify `translations/en/sections/21-chapter-12-part004.md`;
- do not duplicate translated scan105 text in E17;
- translate only verified Part005 scans106–110;
- preserve **105→106 GENUINE CONTINUATION / AUDITED** as provenance;
- carry forward established source-facing terms only when the same Tamil form recurs;
- if Part005 uses a source-visible variant, preserve the Part005 evidence rather than forcing cosmetic uniformity.

## E17 source-visible English note lock

Scans109–110 contain an English historical/reference note already present in the source.

Rules:

- it is source material, not project-created translation;
- retain its wording and source-visible spelling / hyphenation / citation content faithfully in the maintained English layer;
- do not retranslate it;
- do not modernize, copyedit, fact-correct or silently normalize it;
- distinguish it from surrounding project-created English prose through source-check notes and preserved structure;
- any line-wrap normalization required by Markdown must not alter lexical content.

## Chapter13–15 structure locks

- E18 starts with source-visible chapter numeral **13** and stops at chapter13 close / scan119;
- E19 starts with source-visible chapter numeral **14** and stops at chapter14 close / scan129;
- scans121–122 generate **no invented English prose**; their non-rendering provenance remains explicit;
- E20 starts with source-visible chapter numeral **15** and stops exactly at scan132;
- chapter-closing ornaments and blank fields generate no English prose;
- recurring page furniture is excluded from the maintained English literary layer;
- source-boundary comments remain non-rendering provenance only.

## Boundary locks

Incoming:

- E17 starts at scan106 only;
- frozen E16 ends at scan105;
- **105→106 = GENUINE CONTINUATION / AUDITED**;
- no Part004 English prose is duplicated.

Outgoing:

- E20 ends at scan132 only;
- verified Tamil remains inside open chapter15 dialogue;
- **132→133 = PENDING direct audit / source-limited**;
- no Part006 Tamil/English wording may be imported;
- no semantic completion of chapter15 is permitted.

## Planning accounting

- reserved Part005 English batches — **E17–E20 / 4**
- planned maintained English files — **4**
- translated — **0/4**
- source-checked — **0/4**
- English literary prose drafted in planning — **0**
- unresolved planning holds — **0**
- canonical Tamil edits caused by planning — **0**
- assembled Tamil edits caused by planning — **0**
- frozen Parts001–004 English edits — **0**
- Part006 leakage — **0**

## Planning result

**PART005 ENGLISH TRANSLATION PLANNING / SETUP — COMPLETE / PASS**

## Exact next gate

**E18 draft + source-check — section23 / scans111–119.**

## E17 closure

- E17 — **SOURCE-CHECKED / COMPLETE**
- English file — `sections/22-chapter-12-part005.md`
- Tamil authority — `../../sections/22-chapter-12-part005.md`
- scans — **106–110**
- cumulative translated/source-checked — **1/4 / 1/4**
- literary/source blocks — **23 / 23**
- provenance comments — **5 / 5**
- source-visible English note on scans109–110 — **EXACT / preserved**
- unresolved source-check holds — **0**
- canonical / assembled Tamil edits — **0 / 0**
- frozen Parts001–004 English edits — **0**
- exact next gate — **E18 draft + source-check — section23 / scans111–119**
- durable source-check — `E17_SOURCE_CHECK.md`

