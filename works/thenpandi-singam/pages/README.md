# Canonical Tamil Page Records — தென்பாண்டிச் சிங்கம்

This directory contains the canonical per-physical-scan Tamil evidence layer.

No page record is created until the corresponding split PDF is registered.

## Minimum front matter

```yaml
---
scan_page: <global physical scan>
part: <1-18>
part_page: <local physical page>
printed_page: <visible folio or null>
work: "thenpandi-singam"
section: "<source-supported label>"
page_type: "<source-supported page type>"
status: "needs-review"
visual_fidelity: "needs-review"
language: "ta"
source_filename: "<exact registered source filename>"
transcription_method: "direct source-image transcription; PartNNN Pass 1"
---
```

## Page lifecycle

New Pass1 records remain:

- `status: "needs-review"`
- `visual_fidelity: "needs-review"`

They are promoted only after:

Pass2A + Pass2B + Pass3 + whole-Part audit → final metadata/status synchronization.

Formal review notes must remain source-facing and distinguish textual corrections, historical-glyph decisions, structural verification and unresolved questions.

Never use later assembled Tamil or English as authority to overwrite source evidence.
