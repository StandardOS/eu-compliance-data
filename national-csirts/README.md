# The national CSIRTs of the EU member states, and where a CRA report goes

One row per national CSIRT (29 rows across the 27 member states; a state that lists two national teams has two rows), with the CSIRT designated as coordinator for the Cyber Resilience Act beside it.

## Columns

- `national_csirt`, `national_csirt_name`, `national_csirt_website`: the team the CSIRTs Network marks as the state's national CSIRT (the governmental team where none is marked). Sector teams (energy, health, research networks) are left out.
- `cra_coordinator`, `cra_coordinator_name`, `cra_coordinator_contact`: the CSIRT designated as coordinator under Article 14 of Regulation (EU) 2024/2847 (the CRA) for the state of a manufacturer's main establishment, as ENISA lists it; `cra_coordinator_differs` is "yes" where that body is not the national CSIRT (Croatia, Czech Republic).
- `cra_single_reporting_platform`: the single reporting platform of Article 16, where the early warning (24 hours), the vulnerability notification (72 hours) and the final report go from 11 September 2026.

## Sources

- CSIRTs Network member list, https://csirtsnetwork.eu (the members API), read 2026-09-04.
- ENISA, list of CSIRTs designated as coordinators, https://www.enisa.europa.eu/topics/product-security/single-reporting-platform-srp/list-of-csirts-designated-as-coordinators, listed 2026-09-10, read 2026-09-12.
- Regulation (EU) 2024/2847, Articles 14 and 16.

Last verified: 2026-09-12.
