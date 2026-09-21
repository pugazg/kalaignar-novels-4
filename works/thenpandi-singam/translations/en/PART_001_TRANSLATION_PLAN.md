# Part 001 — English Translation Plan — தென்பாண்டிச் சிங்கம்

Status: **E1–E4 SOURCE-CHECKED / COMPLETE**

This is the control plan for the project-created English translation of **Part001 only**.

No English literary prose is created in this planning/setup gate.

## Authority hierarchy

1. `works/thenpandi-singam/pages/` — canonical verified Tamil; controlling authority.
2. `works/thenpandi-singam/sections/` — **PASS / CLOSED — 10/10 VERIFIED** assembled Tamil reading layer.
3. `works/thenpandi-singam/translations/en/` — derived project-created English only.

If English conflicts with Tamil, canonical Tamil governs.

No published, web, remembered or standard English translation is textual authority. English must not silently correct, regularize, modernize, fact-correct or rewrite the Tamil source layer.

## Part001 Tamil source state

Part001 is closed through Tamil archival and assembly:

- source — `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_001_pages_1-26.pdf`
- canonical scans — **1–26**
- novel-body printed pages — **1–14** on scans13–26
- canonical Tamil records — **26/26 verified**
- visual fidelity — **26/26 verified**
- Pass1 / Pass2A / Pass2B / Pass3 — **COMPLETE / PASS**
- Part audit — **PASS / COMPLETE**
- final metadata/status synchronization — **PASS / CLOSED**
- documentation synchronization — **PASS / COMPLETE**
- Tamil archival-ready — **PASS / CLOSED**
- assembled Tamil — **PASS / CLOSED — 10/10 VERIFIED**
- assembled canonical coverage — **26/26**
- omissions / duplicates — **0 / 0**
- unresolved Tamil / historical-glyph / visual / status questions — **0**
- incoming boundary — **NONE / source start**
- outgoing 26→27 — **PENDING direct audit / source-limited because Part002 is not supplied**
- Part002 canonical records — **0**

No source PDF is reopened merely for English planning or drafting.

## Batch-number collision check

Before this plan was created, the live English workspace contained only `README.md`.

Confirmed:
- existing English source-check batch controls — **0**
- existing maintained English literary section files — **0**
- existing Part001 translation-plan/glossary/progress controls — **0**
- E1–E4 collisions — **0**

Therefore the authorized Part001 batch sequence is **E1–E4**.

## Translation objective

Produce readable English that remains reversible to the verified Part001 Tamil evidence.

Preserve:
- narrator and speaker agency;
- chronology and information-release order;
- source praise, criticism, political/historical claims and judgments as source voice rather than project voice;
- rhetorical questions, repetition, exclamations, irony, wordplay and emphatic phrasing;
- paragraph/dialogue/display structure where meaningful;
- source-visible section/chapter structure;
- source-specific personal names, honorifics, offices, place forms and institutional labels;
- source quotations, literary references, work titles and proverbial language without importing published/standard English wording;
- front-matter bibliographic/provenance content that is present in canonical Tamil;
- the Part001 terminal state at scan26 without importing or inventing scan27 wording.

Do not add explanatory history, geography, biography, caste/community interpretation, political interpretation, religious explanation or literary commentary unless the Tamil source itself supplies it.

## Part001 assembled source structure

Part001 contains **10 verified assembled Tamil files**:

1. `00-front-matter.md` — scans1–4
2. `01-kathai-pirandha-kathai.md` — scan5 — `கதை பிறந்த கதை!`
3. `02-pathippurai.md` — scan6 — `பதிப்புரை`
4. `03-v-suba-manickam-paarattu.md` — scan7 — `பெரும்புலவர் வ.சுப. மாணிக்கம் பாராட்டு!`
5. `04-balasubramaniyam-pugazhaaram.md` — scan8 — `டாக்டர் பாலசுப்பிரமணியம் புகழாரம்`
6. `05-thirukkuralmani-thirunavukkarasu-paarattu.md` — scans9–10
7. `06-anbazhaganar-paarattu.md` — scans11–12
8. `07-chapter-01.md` — scans13–16 — chapter1
9. `08-chapter-02.md` — scans17–23 — chapter2
10. `09-chapter-03-part001.md` — scans24–26 — chapter3 Part001 portion, open at outgoing boundary

## Planned English batches

The established Part001 pattern is retained: preliminary matter is grouped into E1, followed by one chapter-unit batch each.

| Batch | Tamil assembled coverage | Planned English file(s) | Scans |
|---|---|---|---:|
| **E1** | sections00–06 — front matter + prefaces/praise material | `sections/00-front-matter.md`; `01-how-the-story-was-born.md`; `02-publishers-note.md`; `03-v-suba-manickam-appreciation.md`; `04-dr-balasubramaniyam-tribute.md`; `05-thirukkuralmani-thirunavukkarasu-appreciation.md`; `06-professor-anbazhagan-appreciation.md` | 1–12 |
| **E2** | section07 — chapter1 | `sections/07-chapter-01.md` | 13–16 |
| **E3** | section08 — chapter2 | `sections/08-chapter-02.md` | 17–23 |
| **E4** | section09 — chapter3 Part001 portion | `sections/09-chapter-03-part001.md` | 24–26 |

Each batch must close **draft + source-check** before the next batch is considered closed.

Planned maintained English files — **10**.

Translated files at planning closure — **0/10**.  
Source-checked files at planning closure — **0/10**.

## Working section-title renderings

These are project working renderings for filenames/headings and may be refined only through explicit English source-check/editorial control:

| Tamil source title | Working English handling |
|---|---|
| `தென்பாண்டிச் சிங்கம்` | **Thenpandi Singam** |
| `கதை பிறந்த கதை!` | **How the Story Was Born!** |
| `பதிப்புரை` | **Publisher's Note** |
| `பெரும்புலவர் வ.சுப. மாணிக்கம் பாராட்டு!` | **V. Suba. Manickam — Appreciation** |
| `டாக்டர் பாலசுப்பிரமணியம் புகழாரம்` | **Tribute by Dr. Balasubramaniyam** |
| `திருக்குறள்மணி திருநாவுக்கரசு பாராட்டு!` | **Thirukkuralmani Thirunavukkarasu — Appreciation** |
| `பேராசிரியர் அன்பழகனார் பாராட்டு` | **Professor Anbazhagan — Appreciation** |
| chapter numerals `1`, `2`, `3` | retain numeric chapter headings |

Do not replace source honorifics/titles with external standardized biographical labels.

## Structural locks

### Front matter / preliminary matter

E1 must preserve:
- repeated source title/author displays;
- the copy-provenance donation insert as source text, not as translator commentary;
- publisher/address/publication details;
- source edition chronology exactly as represented in verified Tamil, including source irregularities;
- all preface/praise speaker attributions;
- the 19-5-1983 release-event heading and internal displayed heading on scans11–12;
- non-rendering source-boundary provenance comments.

Illustrations, publisher emblems, copy stamps and handwritten accession marks that are classified non-body remain non-body and receive no invented English prose.

### Chapters 1–3

- chapter1 — scans13–16; E2 stops at chapter1 close;
- chapter2 — scans17–23; E3 stops at chapter2 close;
- chapter3 — scans24–26; E4 stops exactly at the Part001 terminal scan;
- source-visible rhetorical question sequences, dialogue turns and emphatic punctuation remain structurally meaningful;
- blank lower fields on scans16 and23 create no English body.

### Outgoing 26→27

- scan26 remains inside chapter3;
- Part002 / scan27 is unavailable;
- **26→27 = PENDING direct audit / source-limited**;
- E4 translates scan24–26 only;
- do not import, translate, paraphrase or semantically complete from scan27;
- retain a non-rendering pending-boundary provenance marker;
- English must end exactly where the verified scan26 Tamil ends.

## Names, source variants and glossary discipline

`PART_001_GLOSSARY.md` is the active glossary.

Rules:
- use conservative source-facing romanization for names and terms;
- preserve meaningful source variants by occurrence rather than silently homogenizing them;
- do not substitute external/official spellings merely for familiarity;
- culturally or administratively specific terms may remain transliterated where a forced modern English equivalent would distort the source;
- when the source itself explains a term, let the source explanation carry the meaning instead of adding translator exposition;
- canonical Tamil is never changed to enforce English consistency;
- working English title/name forms may be changed only through explicit English source-check/editorial control.

## Political / historical source framing

Part001 includes source narration and quoted praise about Tamil identity, self-respect, historical rule, white/colonial dominance, Kattabomman/Ettappan comparisons, Nayak rule and local polities.

Translation rules:
- preserve speaker/narrator attribution;
- do not convert a quoted or narrated source claim into project commentary;
- do not fact-correct source history or political framing inside the literary translation;
- distinguish source forms such as `வெள்ளையர்` from any different Tamil label rather than silently normalizing all occurrences to a single external historical category;
- add no current political interpretation.

## Community / social labels

The source uses labels such as `கள்ளர்`, `மறவர்`, `அகம்படியர்` and discusses `அம்பலக்காரர்` and named `நாடு` units.

Rules:
- preserve source terminology and attribution;
- do not add modern caste/community classification, legal category or ethnographic explanation;
- do not modernize `நாடு`, `கோட்டம்`, `வளநாடு`, `மண்டலம்` into unsupported present-day administrative equivalents;
- use the source's own explanatory passages to establish meaning.

## Religious / ritual source framing

Part001 includes Pillaiyar/Vinayakar worship, temple honors, `முளைப்பாரி`, `பரிவட்டம்`, `திருவிளையாடற் புராணம்` and related ritual vocabulary.

Rules:
- translate only what the source supplies;
- retain source-specific terms/transliterations where useful;
- do not add theological, ritual or mythological exposition from outside sources;
- preserve source variants such as `பிள்ளையார்` / `விநாயகர்` by occurrence.

## Source-check standard

For every batch:
1. compare English against verified assembled Tamil and, where needed, canonical source-transcription blocks;
2. account for every literary paragraph/dialogue/display block;
3. preserve source order and physical-source provenance;
4. record unresolved holds explicitly;
5. require canonical Tamil edits = **0** and assembled Tamil edits = **0** unless a genuinely new upstream defect is independently demonstrated;
6. preserve the 26→27 source-limited boundary;
7. require Part002 leakage = **0**.

## Post-batch whole-Part gates

After E4:
1. Part001 whole-Part glossary reconciliation;
2. Part001 English editorial review;
3. Part001 whole-Part bilingual review;
4. Part001 release/readiness report;
5. Part001 release-ready synchronization;
6. Part001 final closure.

Part002 remains blocked until final Part001 closure.

## Planning gate result

**PART001 ENGLISH TRANSLATION PLANNING/SETUP — COMPLETE / PASS**

- reserved batches — **E1–E4 / 4**
- planned maintained English files — **10**
- translated files — **0/10**
- source-checked files — **0/10**
- unresolved planning holds — **0**
- canonical Tamil edits caused by planning — **0**
- assembled Tamil edits caused by planning — **0**
- English literary prose drafted in planning — **0**
- Part002 leakage — **0**
- outgoing 26→27 — **PENDING direct audit / source-limited**

## Exact next gate

**E1 draft + source-check — sections00–06 / scans1–12.**

Do not begin E2 until E1 closes **SOURCE-CHECKED / COMPLETE**.


## E1–E4 draft / source-check closure

All four planned Part001 English batches are now complete:

- E1 — **SOURCE-CHECKED / COMPLETE — scans1–12 / 7 files**
- E2 — **SOURCE-CHECKED / COMPLETE — scans13–16 / 1 file**
- E3 — **SOURCE-CHECKED / COMPLETE — scans17–23 / 1 file**
- E4 — **SOURCE-CHECKED / COMPLETE — scans24–26 / 1 file**

Closure accounting:
- maintained Part001 English files — **10/10**
- translated files — **10/10**
- source-checked files — **10/10**
- physical source coverage — **scans1–26 / all 26 supplied pages**
- unresolved English source-check holds — **0**
- canonical Tamil edits caused by English — **0**
- assembled Tamil edits caused by English — **0**
- Part002 leakage — **0**
- outgoing 26→27 boundary integrity — **PASS / PENDING retained**
- unsupported semantic completion beyond scan26 — **0**

Durable source-check records:
- `E1_SOURCE_CHECK.md`
- `E2_SOURCE_CHECK.md`
- `E3_SOURCE_CHECK.md`
- `E4_SOURCE_CHECK.md`

## Exact next gate

Perform **Part001 whole-Part English glossary reconciliation across E1–E4**.

Do not begin editorial review until glossary reconciliation closes.


## Whole-Part glossary reconciliation closure

**RECONCILED / PASS**

- English files checked — **10/10**
- files changed by glossary reconciliation — **4/10**
- English terminology occurrences corrected — **7**
- deliberate source variants retained — **PASS**
- unresolved glossary holds — **0**
- canonical / assembled Tamil edits — **0 / 0**
- Part002 leakage — **0**
- 26→27 pending-boundary integrity — **PASS**

Durable record: `GLOSSARY_RECONCILIATION.md`.

## Current exact next gate

**Part001 English editorial review across all 10 maintained English files / scans1–26.**

Editorial review must preserve the reconciled glossary locks and the pending 26→27 boundary. Do not begin bilingual review until editorial review closes.


## English editorial review closure

**PASS / CLOSED**

- English files reviewed — **10/10**
- files edited — **9/10**
- English-only editorial corrections — **24**
- unresolved editorial holds — **0**
- canonical / assembled Tamil edits — **0 / 0**
- glossary locks altered — **0**
- Part002 leakage — **0**
- 26→27 pending-boundary integrity — **PASS**

Durable record: `TRANSLATION_REVIEW.md`.

## Current exact next gate

**Part001 whole-Part bilingual review across Tamil + English / scans1–26.**

Do not begin release/readiness until bilingual review closes.


## Whole-Part bilingual review closure

**PASS / CLOSED**

- Tamil/English section pairs — **10/10**
- scans reviewed — **1–26**
- editorial corrections rechecked — **24/24 PASS**
- glossary corrections rechecked — **7/7 PASS**
- further bilingual English-only corrections — **1**
- unresolved bilingual holds — **0**
- canonical / assembled Tamil edits — **0 / 0**
- Part002 leakage — **0**
- 26→27 pending-boundary integrity — **PASS**

Durable record: `BILINGUAL_REVIEW.md`.

## Current exact next gate

**Part001 release/readiness report.**

Do not begin release-ready synchronization, final Part001 closure or Part002 canonical transcription until release/readiness closes.


## Release/readiness closure

**PASS / CLOSED**

- unresolved release/readiness blockers — **0**
- maintained English files — **10/10**
- Part002 leakage — **0**
- outgoing 26→27 — **PENDING / source-limited / preserved**

Durable record: `RELEASE_REPORT.md`.

Current next gate: **Part001 release-ready synchronization**, then final closure.


## Part001 final closure downstream state

**PART001 FINAL CLOSURE — PASS / CLOSED / FROZEN**

- canonical Tamil — **26/26 verified**
- visual fidelity — **26/26 verified**
- assembled Tamil — **10/10 VERIFIED / PASS / CLOSED**
- English maintained/source-checked — **10/10 / 10/10**
- glossary reconciliation — **RECONCILED / PASS**
- English editorial review — **PASS / CLOSED**
- whole-Part bilingual review — **PASS / CLOSED**
- release/readiness — **PASS / CLOSED**
- release-ready synchronization — **PASS / CLOSED**
- unresolved closure blockers — **0**
- canonical / assembled / English body drift after release readiness — **0 / 0 / 0**
- Part002 leakage — **0**
- outgoing 26→27 — **PENDING direct audit / source-limited / preserved**
- Part002 — **NEXT / AWAITING SOURCE INTAKE / NOT REGISTERED**
- Part002 canonical records — **0**
- exact next activity — **Part002 source intake when supplied**

Boundary-only evidence completion after Part002 arrives may update provenance/boundary controls but must not reopen frozen Part001 body text without a genuine independently demonstrated source defect.


## Post-freeze boundary evidence completion — Part002 intake

Part002 is now **SOURCE INTAKE COMPLETE / PASS**.

- source — `TVA_BOK_0065559_தென்பாண்டிச்_சிங்கம்_2021_part_002_pages_27-53.pdf`
- Part002 global scans — **27–53**
- direct adjacent comparison — **26→27 = GENUINE CONTINUATION / AUDITED**
- same chapter3 dialogue continues directly — **PASS**
- printed pagination — **14→15**
- frozen Part001 canonical / assembled / English body changes — **0 / 0 / 0**
- inferred bridge text — **0**
- Part002 canonical records — **0/27**
- Part002 outgoing 53→54 — **PENDING direct audit / source-limited**
- exact next activity — **Part002 Pass1 scans27–36 / local pages1–10**

Part001 remains **FINAL CLOSED / FROZEN**.
