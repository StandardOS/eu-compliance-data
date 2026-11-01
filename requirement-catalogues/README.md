# Six EU requirement catalogues, one row per requirement, six languages

- `cra.csv` / `cra.json`: Cyber Resilience Act, Regulation (EU) 2024/2847, 111 rows, read 2026-10-18.
- `nis2.csv` / `nis2.json`: NIS2, Directive (EU) 2022/2555, 34 rows, read 2026-10-18.
- `dora.csv` / `dora.json`: DORA, Regulation (EU) 2022/2554, 158 rows, read 2026-09-12.
- `gdpr.csv` / `gdpr.json`: GDPR, Regulation (EU) 2016/679, 108 rows, read 2026-10-18.
- `ai-act.csv` / `ai-act.json`: AI Act, Regulation (EU) 2024/1689, 151 rows, read 2026-09-12.
- `data-act.csv` / `data-act.json`: Data Act, Regulation (EU) 2023/2854, 154 rows, read 2026-10-18.

## What a row is

One requirement an organisation owes under the instrument: an obligation, a duty, a deadline, a clause or a control (`kind`), with the exact provision (`statute`), who it applies to as the instrument's own roles (`applies`: manufacturer, importer, essential entity, financial entity, controller, deployer, data holder and so on), and, where one holds, the ISO/IEC 27001:2022 clauses and Annex A controls whose records evidence it (`iso27001`; our reading, checkable against the two texts, never a claim that one conformity is the other).

Per language (`en`, `de`, `fr`, `nl`, `es`, `da`):

- `title_<lang>`: the customer sentence, one imperative line addressed to the company, under ten words in English and inside twelve in the others. Ours.
- `text_<lang>`: the provision as the Official Journal words it in that language. The Union's.

`clock` carries the deadline where the row is one (hours or days from an anchor such as awareness, or a fixed date); `applies_from` the application date where the instrument phases in; `note` a derogation or reading the row needs beside its text.

## Sources

The Official Journal of the European Union, in the six languages, through EUR-Lex (https://eur-lex.europa.eu) and the CELLAR resource service (https://publications.europa.eu/resource/celex/), read on the date each file names. The mapping to ISO/IEC 27001 is ours and is labelled as ours wherever it surfaces.
