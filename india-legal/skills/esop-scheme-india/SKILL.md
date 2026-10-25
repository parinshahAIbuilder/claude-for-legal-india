---
name: esop-scheme-india
description: >
  Design and draft an Employee Stock Option Plan for an Indian company: the scheme
  document, board and shareholder resolutions, grant letter, vesting schedule and
  exercise mechanics, with the Companies Act rules for unlisted companies, SEBI SBEB
  Regulations for listed companies, income-tax treatment (perquisite at exercise,
  startup deferral), Ind AS 102 accounting and an employee FAQ. Use when the user
  mentions ESOP, stock options, ESOP pool, vesting, grant letter, SAR, phantom stock,
  sweat equity, or employee equity in India.
argument-hint: "[company type: unlisted / startup / listed] [pool size %] [key terms]"
---

# ESOP Scheme (India)

## Inputs

Company type (unlisted private / public, DPIIT-recognised startup, listed), pool size, eligible employees (including directors of subsidiaries, if any), vesting and cliff, exercise price approach, exercise window after leaving, trust route or direct route, and the latest valuation.

## Rules to apply

**Unlisted companies** (Companies Act s. 62(1)(b) and Rule 12 of the Companies (Share Capital and Debentures) Rules, 2014; confirm current text):
- Special resolution of shareholders approving the scheme, with the prescribed disclosures in the explanatory statement.
- Minimum one year between grant and vesting.
- Employees who are promoters, or directors holding (directly or indirectly) more than 10% of equity, are not eligible, except in a startup for the period allowed by the rules.
- Independent directors cannot get options.
- Options cannot be transferred, pledged or hypothecated.
- Exercise price is free to set (often at or near fair value; discounts create a bigger perquisite).
- Disclosures in the board's report each year.

**Listed companies**: SEBI (Share Based Employee Benefits and Sweat Equity) Regulations, 2021: compensation committee, shareholder approval, separate approval for grants to employees of group companies or grants of 1% or more to an individual, trust rules on secondary acquisition, disclosures and in-principle approval from the exchanges before allotment.

**Tax**:
- At exercise: the difference between fair market value on the exercise date and the exercise price is a perquisite taxed as salary (s. 17(2)(vi)); the employer deducts TDS. For unlisted shares, FMV comes from a SEBI-registered merchant banker's valuation.
- Eligible startups (s. 80-IAC) can defer the tax and TDS on the perquisite until the earliest of the end of the prescribed period from the end of the year of allotment, sale of the shares, or leaving the company. Confirm the current deferral period.
- At sale: capital gains on the difference between sale price and the FMV taxed at exercise.

**Accounting**: Ind AS 102 (or the ICAI guidance note under IGAAP): fair value at grant date (Black-Scholes or binomial), expensed over the vesting period with true-up for forfeitures.

## Workflow

1. Confirm the inputs and the company type; stop and explain if an intended grantee is ineligible.
2. Recommend pool size, vesting (four years with a one-year cliff is common), exercise window and good / bad leaver treatment, with the trade-offs.
3. Draft the scheme document: definitions, administration, eligibility, pool, grant, vesting, exercise, lapse, adjustments for corporate actions, liquidity / buyback, tax, amendment, governing law.
4. Draft the board resolution, shareholder special resolution and explanatory statement.
5. Draft the grant letter template and the vesting schedule.
6. Write a one-page employee FAQ in plain language (what you get, when, what it costs, tax at exercise and sale).
7. Give the compliance calendar: MGT-14 for the special resolution, register of options (SH-6), allotment filings (PAS-3) on exercise.

## Output

Scheme document, resolutions, grant letter, vesting table, employee FAQ, compliance checklist, and a short note on the Ind AS 102 charge with an illustrative calculation.

## Failure modes

- Granting options to a 10%+ shareholder director in a non-startup.
- Vesting less than one year from grant.
- Forgetting that the employee owes tax at exercise even though there is no liquidity.
- Phantom stock or SARs drafted as if they were options (they are cash-settled and follow different rules).

## Guardrails

- Start every deliverable with `DRAFT | For review by Indian counsel | Not legal advice`.
- Treat every timeline, rate and threshold above as a working baseline and mark it "confirm against the current text"; RBI, SEBI, MCA, stamp and tax rules change often.
- Check the user's stated legal premises before building on them, and say plainly when one is wrong.
- Never file, send or submit anything; prepare it and hand it back.
- The fuller shared guardrails are in this plugin's `CLAUDE.md`.
