# தென்பாண்டிச் சிங்கம் — Source Part Registry

This ledger records the user's **18 split source PDFs**.

**Do not fill an unknown field by inference.** Populate each row only after the corresponding file is attached and inspected.

| Part | Exact source filename | Local physical pages | Global scan range | File size (bytes) | SHA-256 | Source intake | Final state |
|---:|---|---:|---|---:|---|---|---|
| 001 | `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_001_pages_1-26.pdf` | 26 | 1–26 | 49,818,511 | `73e4879c416368cb1789138aacfdbfa18ef84a3722f9074c41b590aff176ea8f` | **COMPLETE / PASS** | **FINAL CLOSED / FROZEN** |
| 002 | `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_002_pages_27-53.pdf` | 27 | 27–53 | 48,679,196 | `232e63ee990e368783b6767b178057815493f636f492ad6a9bd481bd74a3423b` | **COMPLETE / PASS** | **ACTIVE / Pass1 next** |
| 003 | pending | pending | pending | pending | pending | blocked | not started |
| 004 | pending | pending | pending | pending | pending | blocked | not started |
| 005 | pending | pending | pending | pending | pending | blocked | not started |
| 006 | pending | pending | pending | pending | pending | blocked | not started |
| 007 | pending | pending | pending | pending | pending | blocked | not started |
| 008 | pending | pending | pending | pending | pending | blocked | not started |
| 009 | pending | pending | pending | pending | pending | blocked | not started |
| 010 | pending | pending | pending | pending | pending | blocked | not started |
| 011 | pending | pending | pending | pending | pending | blocked | not started |
| 012 | pending | pending | pending | pending | pending | blocked | not started |
| 013 | pending | pending | pending | pending | pending | blocked | not started |
| 014 | pending | pending | pending | pending | pending | blocked | not started |
| 015 | pending | pending | pending | pending | pending | blocked | not started |
| 016 | pending | pending | pending | pending | pending | blocked | not started |
| 017 | pending | pending | pending | pending | pending | blocked | not started |
| 018 | pending | pending | pending | pending | pending | blocked | not started |

## Part001 registered source facts

- source family / archive identifier: **TVA_BOK_0065559**
- no usable embedded/parsed text layer
- rendered source page images are controlling
- source-visible edition: **பதிமூன்றாம் பதிப்பு — ஆகஸ்ட்,, 2021**
- source-visible publication-page extent: **480 pages**
- Part001 body evidence: scan13 = printed page1; scan26 = printed page14
- incoming boundary: **NONE**
- outgoing 26→27: **PENDING Part002 direct witness**

## Part002 registered source facts

- source family / archive identifier: **TVA_BOK_0065559**
- local pages — **27**
- global scans — **27–53**
- no usable embedded/parsed text layer
- rendered source page images are controlling
- first scan — printed page **15**, chapter3 continuation
- last scan — printed page **41**, chapter6 open continuation
- incoming 26→27 — **GENUINE CONTINUATION / AUDITED**
- outgoing 53→54 — **PENDING direct audit / source-limited**
- canonical Part002 page records — **0/27**
- exact intake record — `SOURCE_INTAKE_PART_002.md`

## Registration rules

For each Part, record:

- exact attachment filename as supplied;
- exact local physical page count;
- continuous global `scan_page` range;
- byte size;
- SHA-256;
- whether a usable embedded text layer exists;
- first/last physical scan structure;
- visible printed-page range only where directly established;
- incoming/outgoing boundary state only after direct adjacent-scan comparison.

Part001 starts the global sequence. Each later Part begins immediately after the previous Part's final global physical scan; the actual number is calculated from inspected local extents, never from an assumed split size.

## Current totals

- registered Parts: **2 / 18**
- registered physical scans: **53**
- canonical page records: **26**
- final-closed Parts: **1**
- active transcription Part: **Part002**
- Part001 Pass2A: **COMPLETE / PASS — 26/26 REVIEWED — 14 corrections / 0 unresolved**
- Part001 Pass2B: **COMPLETE / PASS — 26/26 REVIEWED — 5 lexical/spacing/punctuation corrections / 0 historical-glyph corrections / 0 unresolved**
- Part001 Pass3: **COMPLETE / PASS — 26/26 REVIEWED — 0 corrections / 0 unresolved**
- Part001 audit: **PASS / COMPLETE**
- Part001 final status sync: **PASS / CLOSED — 26/26 verified**
- Part001 documentation synchronization: **PASS / COMPLETE**
- Part001 Tamil archival-ready: **PASS / CLOSED**
- Part001 assembled Tamil: **10/10 VERIFIED / PASS / CLOSED**
- Part001 English planning/setup: **COMPLETE / PASS**
- reserved English batches: **E1–E4**
- planned English files: **10**
- English E1–E4: **SOURCE-CHECKED / COMPLETE**
- English source coverage: **scans1–26**
- English glossary reconciliation: **RECONCILED / PASS**
- glossary files changed / terminology corrections: **4 / 7**
- unresolved glossary holds: **0**
- English editorial review: **PASS / CLOSED**
- editorial files reviewed / edited: **10 / 9**
- English-only editorial corrections: **24**
- unresolved editorial holds: **0**
- whole-Part bilingual review: **PASS / CLOSED**
- bilingual English-only corrections: **1**
- unresolved bilingual holds: **0**
- release/readiness: **PASS / CLOSED**
- unresolved release/readiness blockers: **0**
- release-ready synchronization: **PASS / CLOSED**
- Part002 state: **SOURCE INTAKE COMPLETE / PASS — Pass1 NEXT**
- Part002 canonical records: **0/27**
- final closure: **PASS / CLOSED / FROZEN**
- translated/source-checked: **10/10 / 10/10**
- exact next gate: **Part002 Pass1 scans27–36 / local pages1–10**
