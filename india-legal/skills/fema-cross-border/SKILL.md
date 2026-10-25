---
name: fema-cross-border
description: >
  Work out the FEMA and RBI compliance for an Indian company's cross-border
  transaction — foreign investment into India (FDI: allotment, transfer, downstream
  investment), overseas investment by an Indian company or resident (ODI / OPI),
  external commercial borrowings (ECB), GIFT City IFSC units, and the related
  reporting (FC-GPR, FC-TRS, DI, ODI forms, APR, ECB-2, FLA). Produces a compliance
  path, document list, timeline and late-fee exposure. Use when the user mentions
  FEMA, RBI, FDI, foreign investor, FC-GPR, FC-TRS, ODI, overseas subsidiary, APR,
  ECB, FIRMS portal, LSF, compounding, GIFT City, or a foreign parent or subsidiary.
argument-hint: "[describe the transaction: who pays whom, instrument, amount, countries]"
---

# FEMA Cross-Border Compliance

FEMA rules sit in the Foreign Exchange Management Act, 1999, the rules and regulations under it (NDI Rules 2019, Overseas Investment Rules and Regulations 2022, Mode of Payment and Reporting Regulations), and RBI master directions. They change often. Every timeline and threshold below is a working baseline: confirm against the current master direction before filing. The company's AD bank is the first stop for most filings.

## Step 1: classify the transaction

| Type | Typical examples |
|---|---|
| FDI (inbound) | Issue of shares / CCPS / CCDs to a non-resident; transfer between resident and non-resident; share swap |
| Downstream investment | An Indian company with foreign investment investing in another Indian company |
| ODI (outbound) | Indian company setting up or acquiring an overseas entity; financial commitment by way of equity, debt or guarantee |
| OPI | Investment in listed foreign securities or small unlisted holdings without control |
| ECB | Borrowing in foreign currency or INR from a non-resident lender |
| IFSC | Units in GIFT City IFSC are treated as persons resident outside India for FEMA purposes; transactions between a mainland entity and an IFSC unit are cross-border |

## Step 2: check eligibility and pricing

- **FDI**: sector cap and route (automatic / government), instrument eligibility (equity, fully and mandatorily convertible preference shares and debentures, share warrants), pricing not below fair value on issue and the pricing rules on transfer, investor from a country sharing a land border with India needs government approval.
- **ODI**: financial commitment limits relative to net worth, bona fide business activity, no structures prohibited by the rules, valuation for acquisitions, round-tripping restrictions.
- **ECB**: eligible borrower and lender, minimum average maturity, all-in-cost ceiling, end-use restrictions, automatic vs approval route.

## Step 3: reporting timeline (confirm each)

| Event | Form | Usual deadline |
|---|---|---|
| Receipt of FDI money | KYC through AD bank | Promptly on receipt |
| Allotment to non-resident | FC-GPR (FIRMS portal) | Within 30 days of allotment; allot within 60 days of receipt of funds or refund |
| Transfer resident ↔ non-resident | FC-TRS | Within 60 days of transfer or receipt of consideration, whichever is earlier |
| Downstream investment | Form DI | Within 30 days of allotment |
| Foreign liabilities and assets | FLA return | By 15 July each year |
| ODI financial commitment | Form ODI (through AD bank) | At or before remittance |
| ODI annual performance | APR | By 31 December each year, based on audited accounts |
| Disinvestment / restructuring of ODI | As prescribed | Within the window in the regulations |
| ECB | Form ECB for LRN before drawdown; ECB-2 monthly return | Monthly return within 7 working days of month-end |

Late reporting usually attracts a late submission fee (LSF) under the reporting regulations; beyond the LSF window or for substantive contraventions, the route is compounding with RBI. Quantify the exposure on the facts and say which route applies.

## Step 4: tax touchpoints

Withholding on payments to non-residents (s. 195 and the treaty), Form 15CA / 15CB for remittances, transfer pricing for related-party transactions, and the equalisation levy or GST on imported services where relevant. Flag; do not compute treaty positions without the treaty text and the tax residency certificate.

## Output

1. Work-product header.
2. Classification and route in two lines.
3. Eligibility and pricing checks with pass / fail / open.
4. Step-by-step compliance path with forms, owners and dates.
5. Document checklist (valuation certificate, KYC, FIRC, board resolutions, share certificates or demat credit, CS / CA certificates).
6. Exposure note if any filing is late: LSF or compounding, with the reasoning.

## Failure modes

- Treating an optionally convertible instrument as FDI.
- Allotting after the 60-day window without refunding.
- Forgetting the APR every year for each overseas entity.
- Treating an IFSC unit as resident for FEMA purposes.
- Missing government approval for an investor from a land-border country.

## Guardrails

- Start every deliverable with `DRAFT | For review by Indian counsel | Not legal advice`.
- Treat every timeline, rate and threshold above as a working baseline and mark it "confirm against the current text"; RBI, SEBI, MCA, stamp and tax rules change often.
- Check the user's stated legal premises before building on them, and say plainly when one is wrong.
- Never file, send or submit anything; prepare it and hand it back.
- The fuller shared guardrails are in this plugin's `CLAUDE.md`.
