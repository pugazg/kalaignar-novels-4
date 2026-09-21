# Project Handover — தென்பாண்டிச் சிங்கம்

## Repository

- repository: `pugazg/kalaignar-novels-4`
- branch: `main`
- **LIVE MAIN IS AUTHORITATIVE**
- active work: `works/thenpandi-singam/`

## Project state

- work: **தென்பாண்டிச் சிங்கம்**
- author: **கலைஞர் மு. கருணாநிதி**
- source packaging reported by user: **18 split PDF files**, each not more than **50 MB**
- exact filenames / source-family ID / complete physical extent / split page ranges / hashes: **PENDING source intake**
- source PDFs: **working inputs only; do not commit to Git**
- canonical global `scan_page`: begins at the first physical scan of the complete source and never resets at Part boundaries
- canonical page records: **0**
- assembled Tamil files: **0**
- English files: **0**
- final-closed Parts: **0**
- unresolved source-reading questions: **0 because transcription has not started**

## Workflow authority

Follow `works/thenpandi-singam/THENPANDI_SINGAM_ARCHIVAL_GUIDELINES.md`.

The workflow is deliberately aligned to the maintained **பாயும்புலி பண்டாரக வன்னியன்** process:

source intake → Pass1 → Pass2A → Pass2B → Pass3 → Part audit → final status sync → documentation sync → Tamil archival-ready → assembled Tamil → English planning/source-check → glossary reconciliation → editorial review → bilingual review → release/readiness → release-ready sync → final closure/freeze.

## Mandatory Part lock

Only one Part is canonically active at a time.

A subsequent Part may be opened before closure only to inspect its first scan as a **boundary witness** for the active Part. Boundary-witness inspection must not create, import or paraphrase canonical body text for the subsequent Part.

Do not start canonical Part002 transcription until Part001 is **FINAL CLOSED / FROZEN**.

## Source-registration frontier

| Part | Source | Local extent | Global scan range | SHA-256 | State |
|---|---|---:|---|---|---|
| 001 | pending attachment | pending | pending | pending | **NEXT — SOURCE INTAKE** |
| 002–018 | pending attachment | pending | pending | pending | BLOCKED behind active-Part lock |

The authoritative detailed ledger is `SOURCE_PART_REGISTRY.md`.

## Exact next activity

When the first split PDF is attached:

1. register its exact filename and file size;
2. calculate SHA-256;
3. determine exact local physical page count;
4. assign the correct global scan range beginning at scan 1;
5. inspect source structure, printed pagination and first/last physical scans;
6. create/complete `SOURCE_INTAKE_PART_001.md`;
7. establish whether Part002's first scan is needed as a boundary witness;
8. only then begin **Part001 Pass1**.

Do not invent source metadata before the file is available.
