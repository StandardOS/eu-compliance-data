# StandardOS open datasets

The public data behind the compliance product at https://getstandardos.com: what EU
procurement asks for, what a certification audit costs in days, where a
CRA report goes, when the AI Act applies, and what six EU instruments
require, row by row, in six languages. Every file names its source and the
date it was last verified; every number can be re-run against the source.

| Dataset | What | Rows |
|---|---|---|
| [ted-tender-mentions](ted-tender-mentions/) | ISO 27001, ISO 9001, ISO 42001, SOC 2 and NIS2 mentions in TED procurement notices: 365-day snapshot, month by month, by country, with the query | 12 months, 32 countries |
| [iaf-audit-days](iaf-audit-days/) | Auditor days for an initial certification audit by headcount, ISO 9001 (IAF MD 5) and ISO 27001 worked examples | 15 bands, 4 examples |
| [national-csirts](national-csirts/) | The 27 member states' national CSIRTs with the CSIRT designated as coordinator for CRA reports and the single reporting platform | 29 |
| [ai-act-dates](ai-act-dates/) | Every application date of the AI Act as amended by the 2026 omnibus, with the provision | 14 |
| [iso-9001-transition](iso-9001-transition/) | ISO 9001:2026, published 16 September 2026, and the five accreditation transition dates to it | 5 |
| [iso-42001-accredited-bodies](iso-42001-accredited-bodies/) | Which certification bodies can issue an ISO 42001 certificate, by member state, read from all 27 national registers | 27 |
| [nis2-transposition-measures](nis2-transposition-measures/) | Every national measure the member states have communicated to the Commission as transposing NIS2, one row per measure, as the EUR-Lex register holds it | 305 |
| [requirement-catalogues](requirement-catalogues/) | The CRA, NIS2, DORA, GDPR, AI Act and Data Act as one row per requirement: statute, roles, the customer sentence and the provision in en, de, fr, nl, es, da | Cyber Resilience Act 111, NIS2 34, DORA 158, GDPR 108, AI Act 151, Data Act 154 |

## Licence

[Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)
(see LICENSE): share and adapt for any purpose, including commercially, with
credit and a link. Attribution looks like "ISO 9001 transition dates,
StandardOS, https://getstandardos.com, CC BY 4.0".
The Official Journal texts quoted in the catalogues are
the European Union's; reuse of EU law texts is permitted under the Union's
reuse policy (Decision 2011/833/EU) with the source acknowledged. The
CSIRTs Network and ENISA list the teams; TED is the Publications Office's.

Every dataset's README names its source, who holds the rights in it and
the date it was last read. Where a source is not freely publishable,
index.json says what is taken from it. No text, clause heading or control
title of an ISO or CEN standard is in these files: those are sold under
licence and are not ours to put under CC BY.

## Updates

This repository mirrors https://getstandardos.com/datasets and is updated
with each StandardOS release; every file keeps the date its source was
last read. A correction is welcome as an issue, with the source that shows
the right value.
