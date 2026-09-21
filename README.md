# கலைஞர் புதினங்கள் — தென்பாண்டிச் சிங்கம் மின்னாக்கக் களஞ்சியம்

> **LIVE `main` IS AUTHORITATIVE.**
>
> **Source scans are the authority.** Split source PDFs are working inputs and are not committed to Git.

## Active work

- work: **தென்பாண்டிச் சிங்கம்**
- work directory: `works/thenpandi-singam/`
- source packaging: **18 split PDF Parts prepared by the user as the working source set**
- split-file size policy: each source Part is **not more than 50 MB**
- exact source filenames, physical-page ranges, printed-page ranges, byte sizes, SHA-256 values and total physical extent: **PENDING source intake**
- canonical `scan_page`: global across the complete work; **never reset at a Part boundary**
- current state: **repository workflow scaffold initialized; source ingestion not yet started**
- active Part: **Part001 — PENDING ATTACHMENT / SOURCE INTAKE**

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
- `works/thenpandi-singam/indexes/page-map.md` — canonical physical-page map
- `works/thenpandi-singam/pages/` — canonical per-scan Tamil records
- `works/thenpandi-singam/sections/` — assembled verified Tamil reading layer
- `works/thenpandi-singam/translations/en/` — project-created English layer

## Source-fidelity rules

Preserve source wording, punctuation, paragraphing, dialogue structure, displayed text, page order, historical glyph identity, printed pagination, illustrations/non-text matter and genuine split-boundary continuations. Do not normalize a source reading merely because a modern spelling looks more familiar.

Final `verified` status is assigned only after the whole-Part Tamil verification chain and Part audit have passed.

## Exact next activity

**Ingest Part001** when its split PDF is attached: record exact filename, local physical extent, global scan range, byte size and SHA-256; inspect the first/last scan and establish Part001 source intake before transcription begins.
