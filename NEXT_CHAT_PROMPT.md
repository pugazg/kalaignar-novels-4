# NEXT CHAT PROMPT — தென்பாண்டிச் சிங்கம் / Part007 English translation planning/setup

Continue directly in `pugazg/kalaignar-novels-4`, branch `main`, active work `works/thenpandi-singam/`. **LIVE MAIN IS AUTHORITATIVE.**

## Durable frozen state

Parts **001–006 are FINAL CLOSED / FROZEN**.

Do not reopen their canonical Tamil, assembled Tamil or maintained English merely to plan Part007 English.

## Part007 Tamil authority

- source — `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_007_pages_160-186.pdf`
- scans — **160–186 / 27**
- canonical Tamil / visual fidelity — **27/27 verified / 27/27 verified**
- Tamil archival-ready — **PASS / CLOSED**
- assembled Tamil — **COMPLETE / PASS / CLOSED — 3/3 VERIFIED**
- assembled inventory:
  1. `sections/30-chapter-18-part007.md` — scans160–163 — chapter18 continuation and close
  2. `sections/31-chapter-19.md` — scans164–173 — complete chapter19
  3. `sections/32-chapter-20.md` — scans174–186 — complete chapter20
- assembled exact regeneration — **3/3 PASS**
- canonical source-transcription coverage — **27/27**
- omissions / duplicates / unsupported Tamil insertion / audit-note leakage — **0 / 0 / 0 / 0**
- incoming **159→160 — GENUINE CONTINUATION / AUDITED**
- outgoing **186→187 — PENDING direct audit / source-limited**
- Part008 leakage — **0**

Durable validation:

`works/thenpandi-singam/PART_007_ASSEMBLED_TAMIL_VALIDATION.md`

## Collision snapshot at assembly closure

Snapshot only — **recheck live main before reserving anything**.

At assembled-body head `1dc1c4e1f5a92e2048ffeff7d5df0988dcf58cb2`:

- existing English source-check controls — **E1–E24**
- existing maintained English section orders — **00–29**
- candidate non-colliding Part007 batch range — **E25–E27**
- candidate maintained English section orders — **30–32**
- candidate ranges reserved by assembly — **0**

## Exact next activity

Perform **Part007 English translation planning/setup** only.

### Mandatory live collision recheck

Before creating/reserving controls:

- enumerate live `works/thenpandi-singam/translations/en/E*_SOURCE_CHECK.md` controls;
- enumerate live `works/thenpandi-singam/translations/en/sections/` maintained English files;
- confirm whether **E25–E27** are still absent;
- confirm whether maintained English section orders **30–32** are still absent;
- if any collision exists, do **not** overwrite; choose the next contiguous non-colliding range and record the reason;
- reserve identifiers only after this live recheck.

### Planned source mapping if E25–E27 remain free

- **E25** — Tamil authority `sections/30-chapter-18-part007.md` — scans160–163 — planned English `translations/en/sections/30-chapter-18-part007.md`
- **E26** — Tamil authority `sections/31-chapter-19.md` — scans164–173 — planned English `translations/en/sections/31-chapter-19.md`
- **E27** — Tamil authority `sections/32-chapter-20.md` — scans174–186 — planned English `translations/en/sections/32-chapter-20.md`

### Planning controls to create

Create:

- `works/thenpandi-singam/translations/en/PART_007_TRANSLATION_PLAN.md`
- `works/thenpandi-singam/translations/en/PART_007_GLOSSARY.md`
- `works/thenpandi-singam/translations/en/PART_007_PROGRESS.md`

Planning/setup must create **no literary English prose** and no maintained English section files.

### Authority hierarchy

1. verified canonical Part007 `pages/` — controlling Tamil textual authority;
2. verified Part007 assembled `sections/` — maintained Tamil reading-layer authority;
3. project-created English — derived only.

No published/web/remembered English translation is textual authority. Do not silently modernize, fact-correct, normalize or reinterpret the Tamil.

### Structural / continuity locks for planning

E25 / chapter18 continuation:

- begins at scan160 only;
- do not repeat chapter numeral **18** because the maintained Tamil section30 is a continuation from frozen Part006 section29;
- do not modify frozen `translations/en/sections/29-chapter-18-part006.md`;
- do not duplicate translated scan159 wording;
- preserve **159→160 GENUINE CONTINUATION / AUDITED** as provenance;
- scan163 closes chapter18; ornaments produce no English prose.

E26 / chapter19:

- source-supported chapter numeral **19** retained;
- scans164–173 only;
- preserve 166→167, 168→169 and 172→173 continuity;
- scan173 closes chapter19; ornaments produce no English prose.

E27 / chapter20:

- source-supported chapter numeral **20** retained;
- scans174–186 only;
- preserve 179→180, 183→184 and 184→185 continuity;
- scan186 closes chapter20; ornaments produce no English prose;
- preserve **186→187 PENDING direct audit / source-limited**;
- no Part008 / scan187 Tamil or English wording may be imported or inferred.

### Glossary setup

Build Part007 glossary controls from recurring verified Tamil terms/names/forms in sections30–32 and prior frozen terminology where the same Tamil form recurs. Preserve source-specific names, honorifics, offices, places, colloquial forms and source-era distinctions. Do not add explanatory history, biography, geography, politics, religion or literary commentary not present in Tamil.

### Planning accounting required

At closure record:

- reserved Part007 English batches — **3**
- planned maintained English files — **3**
- translated — **0/3**
- source-checked — **0/3**
- English literary prose drafted in planning — **0**
- unresolved planning / glossary holds — **0**
- canonical Tamil edits caused by planning — **0**
- assembled Tamil edits caused by planning — **0**
- frozen Parts001–006 English body edits — **0**
- Part008 leakage — **0**

Synchronize README, HANDOVER, WORKFLOW_STATUS, source registry, archival guidelines, assembled-Tamil validation, Tamil archival-ready checkpoint, `translations/en/README.md`, and `NEXT_CHAT_PROMPT.md`.

If planning/setup closes successfully and E25–E27 are confirmed/reserved, set exact next activity to **E25 draft + source-check — section30 / scans160–163**.
