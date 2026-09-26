# NEXT CHAT PROMPT — தென்பாண்டிச் சிங்கம் / Part005 English translation planning/setup

Continue directly in `pugazg/kalaignar-novels-4`, branch `main`, active work `works/thenpandi-singam/`. **LIVE MAIN IS AUTHORITATIVE.**

## Durable frozen state

Parts **001–004 are FINAL CLOSED / FROZEN**.

Do not reopen their canonical Tamil, assembled Tamil or maintained English merely to plan Part005 English.

## Part005 authoritative Tamil state

Source:

- `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_005_pages_106-132.pdf`
- bytes — **48,768,215**
- SHA-256 — `4eaeef2e68daa5082662001f8906ca10ae207e95975a4207d3cdadd52708455b`
- global scans — **106–132 / 27**

Tamil gates:

- source intake — **COMPLETE / PASS**
- Pass1 — **COMPLETE / PASS — 27/27 TEXT-COMPLETE**
- Pass2A — **COMPLETE / PASS**
- Pass2B — **COMPLETE / PASS**
- Pass3 — **COMPLETE / PASS**
- whole-Part audit — **PASS / COMPLETE**
- final metadata/status synchronization — **PASS / CLOSED**
- documentation synchronization — **PASS / COMPLETE**
- Tamil archival-ready — **PASS / CLOSED**
- assembled Tamil — **COMPLETE / PASS / CLOSED — 4/4 VERIFIED**

Current canonical state:

- canonical Tamil — **27/27 verified**
- visual fidelity — **27/27 verified**
- unresolved Tamil / glyph / visual / structural / documentation blockers — **0**

Durable assembled validation:

`works/thenpandi-singam/PART_005_ASSEMBLED_TAMIL_VALIDATION.md`

## Part005 assembled Tamil inventory

1. `works/thenpandi-singam/sections/22-chapter-12-part005.md` — scans **106–110**
2. `works/thenpandi-singam/sections/23-chapter-13.md` — scans **111–119**
3. `works/thenpandi-singam/sections/24-chapter-14.md` — scans **120–129**
4. `works/thenpandi-singam/sections/25-chapter-15-part005.md` — scans **130–132**

Assembly audit:

- canonical source-transcription records accounted — **27/27**
- non-empty canonical blocks represented — **25/25**
- scans121–122 — **non-literary provenance only / 0 literary prose**
- omissions / duplicates — **0 / 0**
- unsupported Tamil body insertion — **0**
- audit/review/workflow-note leakage — **0**
- canonical page mutations caused by assembly — **0**
- frozen Parts001–004 assembled Tamil changes — **0**
- Part006 leakage — **0**
- unresolved assembly blockers — **0**

## Locked structural / boundary state

- section22 continues chapter12 from scan106 and does **not** duplicate frozen Part004 scan105;
- scans109–110 contain a source-visible English historical/reference note that is source material and must not be silently rewritten or fact-corrected;
- section23 carries chapter13;
- section24 carries chapter14 with scans121–122 as non-literary provenance only;
- section25 carries chapter15 only through scan132;
- incoming **105→106 = GENUINE CONTINUATION / AUDITED**;
- outgoing **132→133 = PENDING direct audit / source-limited**;
- no Part006 / scan133 wording has been imported or inferred.

## Exact next activity

Perform **Part005 English translation planning/setup**.

### Collision check

Before reserving identifiers, inspect live `works/thenpandi-singam/translations/en/`.

Expected pre-setup state:

- existing source-check batches — **E1–E16**
- existing maintained English section files — section orders **00–21**
- expected next non-colliding batches — **E17–E20**
- expected planned English section orders — **22–25**

Do not rely on the expectation if live `main` differs.

### Planned mapping if collision-free

- **E17** — Tamil section22 / scans106–110 → `translations/en/sections/22-chapter-12-part005.md`
- **E18** — Tamil section23 / scans111–119 → `translations/en/sections/23-chapter-13.md`
- **E19** — Tamil section24 / scans120–129 → `translations/en/sections/24-chapter-14.md`
- **E20** — Tamil section25 / scans130–132 → `translations/en/sections/25-chapter-15-part005.md`

### Planning/setup requirements

Create:

- `works/thenpandi-singam/translations/en/PART_005_TRANSLATION_PLAN.md`
- `works/thenpandi-singam/translations/en/PART_005_GLOSSARY.md`
- `works/thenpandi-singam/translations/en/PART_005_PROGRESS.md`

Rules:

- English is project-created derived text; canonical Tamil remains controlling authority;
- use only verified canonical / assembled Tamil and already source-checked project forms from frozen Parts001–004;
- do not use published/web/remembered English as textual authority;
- do not add external history, biography, political interpretation, caste/community interpretation, religious explanation or literary commentary;
- do not silently normalize source-visible Tamil variants merely for English consistency;
- preserve speaker agency, chronology, information-release order, rhetoric, dialogue turns and display structure;
- E17 continues chapter12 from frozen Part004 E16; do not modify or duplicate frozen Part004 English;
- the scans109–110 source-visible English historical/reference note is already source material: planning must preserve it faithfully rather than retranslating, modernizing or fact-correcting it;
- E18 begins with source-visible chapter numeral **13**;
- E19 begins with source-visible chapter numeral **14**; scans121–122 generate **0 English literary prose** and remain provenance only;
- E20 begins with source-visible chapter numeral **15** and stops exactly at scan132;
- preserve **132→133 = PENDING direct audit / source-limited** and do not infer Part006 English;
- English literary prose drafted during planning/setup — **0**;
- canonical Tamil edits caused by planning — **0**;
- assembled Tamil edits caused by planning — **0**;
- frozen Parts001–004 English edits — **0**;
- Part006 leakage — **0**.

Planning/setup must close **COMPLETE / PASS** before drafting E17.

If planning/setup passes, exact next gate:

**E17 draft + source-check — section22 / scans106–110.**
