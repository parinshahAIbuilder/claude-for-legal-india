---
name: leave-licence-review
description: >
  Review an Indian commercial lease or leave-and-licence agreement (offices, retail,
  warehouses, co-working, managed offices) from the tenant / licensee or landlord
  side. Checks lease vs licence character, registration and stamp duty by state,
  lock-in and exit, escalation, security deposit, fit-out and reinstatement, CAM and
  GST, TDS under section 194-I, title and approvals, and flags the Ind AS 116 impact.
  Use when the user mentions lease deed, leave and licence, rent agreement, office
  lease, lock-in, escalation, security deposit, landlord, or uploads a property
  agreement in India.
argument-hint: "[path to agreement] [our side: tenant / landlord] [state and city]"
---

# Commercial Lease and Leave-and-Licence Review

## Inputs

The agreement, our side, the state and city of the property, the business plan for the premises (term needed, fit-out spend), and any term sheet. Ask for title documents and the occupancy certificate if diligence is in scope.

## Review battery

| # | Area | What to check |
|---|---|---|
| 1 | Character | Lease (interest in property, Transfer of Property Act s. 105) vs leave and licence (permission to use, Indian Easements Act s. 52). The label is not decisive; exclusive possession and the substance decide. Note the consequence for eviction and rent-control protection in that state |
| 2 | Registration | Leases from year to year or for more than one year must be registered (Registration Act s. 17). Some states, for example Maharashtra, require registration of leave-and-licence agreements regardless of term. An unregistered document that must be registered cannot be relied on to prove the lease terms. Confirm the rule for the state |
| 3 | Stamp duty | Rate and basis under the state Stamp Act (usually on average annual rent plus deposit or interest on it, scaled by term). State who pays. Compute an estimate and mark it "confirm on the state portal" |
| 4 | Term and lock-in | Lock-in for each side, renewal options and rent on renewal, early exit penalties. Match against the business plan and fit-out payback |
| 5 | Rent and escalation | Rent-free / fit-out period, escalation rate and frequency, market reset clauses, rent on area (carpet vs chargeable / super built-up; loading %) |
| 6 | Security deposit | Months of rent, interest (usually none), refund timeline, deduction rights, interest for late refund |
| 7 | CAM and outgoings | CAM basis, caps, audit rights, property tax and society charges, electricity and DG |
| 8 | Tax | GST at the applicable rate on commercial rent and CAM (landlord's GSTIN on invoice so the tenant gets ITC); TDS under s. 194-I (rate for land / building vs plant and machinery; confirm current rates); reverse charge where the landlord is unregistered and the law requires it |
| 9 | Fit-out and reinstatement | Approval process, ownership of fit-outs, reinstatement obligation at exit (cost exposure), landlord's contribution |
| 10 | Use and approvals | Permitted use matches zoning and the occupancy certificate; fire NOC; signage; 24x7 access; sub-licensing rights (critical for co-working and managed offices) |
| 11 | Title | Landlord's title, mortgage (lender NOC needed), society / association consent, power of attorney chain |
| 12 | Default and exit | Cure periods, landlord's right to disconnect services (usually unenforceable without due process), force majeure, termination for building defects |
| 13 | Dispute resolution | Arbitration seat and institution; note that eviction under state rent laws may not be arbitrable |

## Accounting flag

If the tenant reports under Ind AS, note that the lease term judgment (lock-in plus reasonably certain renewals), escalations and rent-free period drive the Ind AS 116 liability. Hand off to `ind-as-116-leases` for the schedule.

## Output

1. Work-product header.
2. Summary: sign / sign with changes / do not sign, with total cash commitment over lock-in and full term in ₹ crore.
3. Issues table with severity and redlines.
4. Execution checklist: stamp duty estimate, registration, signatories, lender NOC.
5. Commercial summary table: area, rent per sq ft, escalation, lock-in, deposit, CAM, term.

## Failure modes

- Signing an unregistered long-term lease to save stamp duty, then being unable to enforce the lock-in.
- Quoting rent on super built-up area without stating the loading.
- Missing a sub-licensing prohibition for a co-working business.

## Guardrails

- Start every deliverable with `DRAFT | For review by Indian counsel | Not legal advice`.
- Treat every timeline, rate and threshold above as a working baseline and mark it "confirm against the current text"; RBI, SEBI, MCA, stamp and tax rules change often.
- Check the user's stated legal premises before building on them, and say plainly when one is wrong.
- Never file, send or submit anything; prepare it and hand it back.
- The fuller shared guardrails are in this plugin's `CLAUDE.md`.
