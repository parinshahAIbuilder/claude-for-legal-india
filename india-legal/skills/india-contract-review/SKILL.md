---
name: india-contract-review
description: >
  Review a commercial contract (MSA, vendor agreement, services agreement, NDA,
  distribution, SaaS, consultancy) under Indian law and return a RED / AMBER / GREEN
  issues table, a redline memo and a business summary. Checks the Indian Contract Act
  (validity, restraint of trade, penalty vs liquidated damages), Specific Relief Act,
  Arbitration and Conciliation Act (seat, venue, institution), stamp duty and
  execution, GST and TDS clauses, DPDP Act data protection, and FEMA where a party is
  foreign. Use when the user says "review this contract", "Indian law review", "NDA
  review India", "is this clause enforceable in India", or uploads an agreement with
  an Indian party.
argument-hint: "[path to contract] [our side: customer / vendor] [state of execution]"
---

# India Contract Review

## Inputs

The contract, which side we are on, the commercial context (value, term, criticality), the state where it will be executed and stamped, and the house playbook if one exists. If the playbook is missing, review against market-standard positions for an Indian mid-size company and say so.

## Review battery

Work through every item. Quote the clause number for each finding.

| # | Area | What to check |
|---|---|---|
| 1 | Parties and capacity | Correct legal names, CIN / LLPIN, registered office, authorised signatory backed by a board resolution or power of attorney |
| 2 | Validity | Free consent, lawful consideration and object (Contract Act ss. 10, 14–23); agreements void for uncertainty (s. 29) |
| 3 | Restraint of trade | Post-termination non-compete or non-solicit of customers is generally void under s. 27; restraints during the term are usually upheld. Flag and suggest a confidentiality-based alternative |
| 4 | Limitation of legal proceedings | Clauses that cut short the limitation period or bar remedies absolutely are void under s. 28; exclusive jurisdiction of one competent Indian court is fine |
| 5 | Damages | Liquidated damages and penalties are both capped at reasonable compensation under s. 74; the stated sum is the ceiling, not an automatic award. Check indemnity scope, caps, carve-outs (fraud, IP, confidentiality, data breach) and consequential loss exclusions |
| 6 | Specific performance | After the 2018 amendment to the Specific Relief Act, specific performance is the general rule for most contracts; check whether that suits our side |
| 7 | Dispute resolution | Seat (decides court supervision) vs venue; institution (MCIA, IAMC, DIAC, SIAC, ICC) or ad hoc; number of arbitrators; language; interim relief under s. 9; for a foreign party, enforceability of the award in India |
| 8 | Stamp duty and execution | Instrument type under the applicable state Stamp Act, duty payable, who pays, e-stamping, execution in counterparts. Unstamped or under-stamped instruments are inadmissible in evidence until the deficit and penalty are paid, so stamp before signing |
| 9 | Tax clauses | GST: prices exclusive or inclusive, invoice and GSTIN requirements, ITC protection if the supplier fails to file. TDS: section (194C, 194J, 194I, 194Q, 195) and grossing-up language. Reverse charge for imports of services |
| 10 | Data protection | Digital Personal Data Protection Act, 2023: roles (data fiduciary / processor), purpose limitation, breach notification, cross-border transfer, deletion on termination |
| 11 | Foreign party | FEMA: payment currency, remittance documentation (Form 15CA / 15CB), guarantees by or to non-residents, governing law |
| 12 | Term and exit | Auto-renewal and notice periods, termination for convenience, lock-in, transition assistance, survival |
| 13 | IP | Ownership of deliverables, licence-back, moral rights waiver (Copyright Act s. 57 limits waiver), open-source |
| 14 | Compliance | Anti-bribery, MSME payment terms (45-day limit under the MSMED Act if the supplier is a registered micro or small enterprise; ties to section 43B(h) of the Income-tax Act) |

## Output

1. Work-product header.
2. **One-paragraph summary** for the business: sign / sign with changes / do not sign, and the top three risks in rupees where possible.
3. **Issues table**: clause, issue, severity (RED / AMBER / GREEN), why it matters, proposed redline.
4. **Redline language** for every RED and AMBER item, ready to paste.
5. **Execution checklist**: stamp duty (state, article, amount or basis), signatories and authority, counterparts, registration if needed.
6. Open questions for the business owner.

## Failure modes

- Treating a post-termination non-compete as enforceable because the counterparty is foreign.
- Confusing venue with seat.
- Ignoring stamp duty until a dispute, when the document cannot be relied on in evidence.
- Accepting a supplier-favourable GST clause that leaves us exposed to ITC loss.

## Guardrails

- Start every deliverable with `DRAFT | For review by Indian counsel | Not legal advice`.
- Treat every timeline, rate and threshold above as a working baseline and mark it "confirm against the current text"; RBI, SEBI, MCA, stamp and tax rules change often.
- Check the user's stated legal premises before building on them, and say plainly when one is wrong.
- Never file, send or submit anything; prepare it and hand it back.
- The fuller shared guardrails are in this plugin's `CLAUDE.md`.
