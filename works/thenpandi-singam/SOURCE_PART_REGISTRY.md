# தென்பாண்டிச் சிங்கம் — Source Part Registry

This ledger records the user's **18 split source PDFs**.

**Do not fill an unknown field by inference.** Populate each row only after the corresponding file is attached and inspected.

| Part | Exact source filename | Local physical pages | Global scan range | File size (bytes) | SHA-256 | Source intake | Final state |
|---:|---|---:|---|---:|---|---|---|
| 001 | pending | pending | pending | pending | pending | **NEXT** | not started |
| 002 | pending | pending | pending | pending | pending | blocked | not started |
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

- registered Parts: **0 / 18**
- supplied/inspected physical scans: **0**
- canonical page records: **0**
- final-closed Parts: **0**
