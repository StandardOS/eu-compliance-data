# Which certification bodies can issue an ISO 42001 certificate, by EU member state

All 27 national accreditation registers, read on **2026-09-25**.
**12 certification bodies in 3 member states** hold ISO/IEC 42001 in their accredited scope. 12 registers answer none, and 12 cannot answer a scope query at all.

## Files

- `registers.csv` and `registers.json`: one row per member state, with the accreditation body, the answer, the bodies named where there are any, and what the register does.

## The three answers, and why the difference matters

- **bodies**: the register names them. Every one was verified by opening the body's own scope document or scope table, not by trusting that a search matched its page.
- **zero**: the register answers, and the answer is none. Every zero was calibrated first with the same query for **ISO/IEC 27001**. If that returns nothing either, the row is `unanswered` instead. Two registers return zero for both and would otherwise have produced a confident false zero, one of them for the member state with the most bodies.
- **unanswered**: the register exists and cannot answer this question. The `how_the_register_answers` column says what it does instead. One register is unanswered by choice: it sits behind a bot check, and bypassing bot detection is not something we do for a number.

## What this is not

It is not a directory of certification bodies and it is not a ranking. Each national register is the authority for its own country; this is a dated reading of them, published so the reading can be checked and redone. No payment was taken or offered for any entry, in either direction.

One thing to know before relying on a certificate: the global database of accredited certificates does not carry ISO/IEC 42001 as a standard at all, so a certificate to it cannot be verified there the way an ISO/IEC 27001 certificate can. Accredited scope is held nationally, in the registers this file reads.

Last verified: 2026-09-25. Accreditation for a new standard is granted month by month, so re-read the register before acting on a row.
