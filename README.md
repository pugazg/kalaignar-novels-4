# கலைஞர் புதினங்கள் — தென்பாண்டிச் சிங்கம் மின்னாக்கக் களஞ்சியம்

> **LIVE `main` IS AUTHORITATIVE.**
>
> **Source scans are the authority.** Split source PDFs are working inputs and are not committed to Git.

## Active work

- work: **தென்பாண்டிச் சிங்கம்**
- work directory: `works/thenpandi-singam/`
- source packaging: **18 split PDF Parts prepared by the user**
- split-file size policy: each source Part is **not more than 50 MB**
- source family / archive identifier: **TVA_BOK_0065559**
- complete physical extent: **pending intake of Parts002–018**
- registered Parts: **1/18**
- canonical `scan_page`: global across the complete work; **never resets at a Part boundary**
- source PDFs committed to Git: **0**

## Part001 — SOURCE INTAKE COMPLETE

- source: `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_001_pages_1-26.pdf`
- local physical pages: **26**
- global scans: **1–26**
- bytes: **49,818,511**
- SHA-256: `73e4879c416368cb1789138aacfdbfa18ef84a3722f9074c41b590aff176ea8f`
- text layer: **absent / no usable parsed text exposed**
- controlling authority: **rendered source page images**
- source-visible edition: **பதிமூன்றாம் பதிப்பு — ஆகஸ்ட் 2021**
- source-visible publication-page extent: **480 pages**
- numbered novel body begins at **scan13 / printed page1**
- scan26 carries **printed page14**
- incoming boundary: **NONE — physical source begins at scan1**
- outgoing **26→27**: **PENDING direct audit when Part002 is supplied**
- canonical Part001 page records: **20/26 — scans1–20**
- Part001 Pass1: **IN PROGRESS — 20/26 TEXT-COMPLETE**
- Part002 canonical records: **0**

## Workflow baseline

This repository follows the maintained workflow used for **பாயும்புலி பண்டாரக வன்னியன்** in `pugazg/kalaignar-novels`.

For each Part, finish the complete workflow before starting canonical transcription of the next Part:

1. source intake and checksum registration
2. Pass 1 — complete physical capture/transcription
3. Pass 2A — direct textual verification
4. Pass 2B — independent lexical / historical-glyph reread
5. Pass 3 — visual / structural verification
6. whole-Part audit
7. final metadata/status synchronization
8. documentation synchronization
9. Tamil archival-ready checkpoint
10. assembled Tamil construction + audit
11. English translation planning/setup
12. English draft + source-check batches
13. whole-Part glossary reconciliation
14. English editorial review
15. whole-Part bilingual review
16. release/readiness report
17. release-ready synchronization
18. final closure — **PASS / CLOSED / FROZEN**

A later Part may be inspected only as an adjacent **boundary witness** until the active Part is closed. Boundary inspection must not create canonical text for the later Part.

## Core controls

- `HANDOVER.md` — current durable project state and exact next action
- `works/thenpandi-singam/THENPANDI_SINGAM_ARCHIVAL_GUIDELINES.md` — controlling workflow
- `works/thenpandi-singam/SOURCE_PART_REGISTRY.md` — 18-Part source intake ledger
- `works/thenpandi-singam/SOURCE_INTAKE_PART_001.md` — registered Part001 source intake
- `works/thenpandi-singam/indexes/page-map.md` — physical-page map
- `works/thenpandi-singam/pages/` — canonical per-scan Tamil records
- `works/thenpandi-singam/sections/` — assembled verified Tamil reading layer
- `works/thenpandi-singam/translations/en/` — project-created English layer

## Exact next activity

Continue **Part001 Pass1 — global scans21–26 / local pages21–26**.

scans1–20 are text-complete. Keep every created page record at `status: "needs-review"` and `visual_fidelity: "needs-review"`. Do not begin Pass2A until Pass1 covers all **26** Part001 scans. Keep **26→27** pending until Part002 is supplied.
