# TED tender mentions: ISO 27001 against SOC 2, and the rest

How often EU public procurement notices mention each standard. Full-text
mentions in Tenders Electronic Daily (TED), the EU's own procurement
portal, counted through its public search API, which answers without a
key, so every number here can be re-run by anyone.

## Files

- `snapshot.csv`: the rolling 365-day and 30-day counts per term, observed 2026-09-12. The headline: 3,405 notices mention ISO 27001 against 104 for SOC 2, 32.7 to 1.
- `monthly.csv` and `monthly.json`: the same terms per calendar month for the twelve full months before 2026-09-14, by publication date.
- `by-country.csv`: the 365-day counts per buyer country (EU-27, EEA, Switzerland, UK), observed 2026-09-12.
- `candidates.csv`: 13 management-system standards and frameworks over the 365 days to 25 September 2026, observed 2026-09-25. Counted to answer which standard an EU buyer actually asks a supplier for: ISO 9001 leads at 17,124 notices, ISO 14001 follows at 9,937, ISO 27001 is third at 3,417, and SOC 2 is 105, which is what an American attestation looks like in European procurement.

## The query

Endpoint: `POST https://api.ted.europa.eu/v3/notices/search` with a body of
`{"query": "<expert query>", "fields": ["publication-number"], "limit": 1}`;
the count is `totalNoticeCount` in the answer. The expert query per term is
every spelling joined by OR, and a publication-date window:

```
(FT~"ISO 27001" OR FT~"ISO/IEC 27001" OR FT~"ISO27001") AND publication-date>=20250901 AND publication-date<=20250930
```

One term was tried and is deliberately absent from `candidates.csv`: eIDAS returned 214,714 notices, which is not demand. The word appears in the electronic-signature boilerplate of ordinary submission instructions ("submissions must be signed in accordance with eIDAS"), not as a requirement on the supplier, so the count measures the portal's own paperwork. A full-text count is only a demand signal where the term names something the supplier must hold.

Spellings counted per term: iso27001: "ISO 27001", "ISO/IEC 27001", "ISO27001"; iso9001: "ISO 9001", "ISO9001"; iso42001: "ISO 42001", "ISO/IEC 42001", "ISO42001"; soc2: "SOC 2", "SOC2"; nis2: "NIS2", "NIS 2".

## What the numbers are, and are not

These are mentions. A notice matches if the string appears anywhere in it,
for any reason, a buyer describing its own certification included.
"Mentioned in N notices" is defensible; "required by N tenders" is not,
and this dataset does not support it. The ratio between two standards
survives that caveat, because it compares mentions with mentions under the
same method.

Source: Tenders Electronic Daily, Publications Office of the European Union,
https://ted.europa.eu, API documentation at https://docs.ted.europa.eu.
Last verified: 2026-09-14.
