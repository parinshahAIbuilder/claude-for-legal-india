---
name: sha-investment-review
description: >
  Review or draft the investment documents for an Indian private company round:
  term sheet, shareholders' agreement (SHA), share subscription agreement (SSA) and
  the articles. Covers CCPS / CCD / equity instruments, valuation and FEMA pricing
  for foreign investors, private placement and preferential allotment process under
  the Companies Act (sections 42 and 62), investor rights (board seat, ROFR, tag,
  drag, anti-dilution, liquidation preference, information and affirmative votes),
  founder obligations and the closing checklist. Use when the user mentions SHA,
  SSA, term sheet, investment agreement, CCPS, funding round, angel / VC round,
  anti-dilution, liquidation preference, or allotment to investors in India.
argument-hint: "[path to term sheet / SHA / SSA] [our side: company / founders / investor]"
---

# SHA and Investment Documents (India)

## Inputs

The documents, our side, round size and pre-money valuation, instrument, investor residency (resident / non-resident / FPI / AIF), whether the company is a DPIIT-recognised startup, current cap table and the existing articles.

## Review battery

| # | Area | What to check |
|---|---|---|
| 1 | Instrument | Equity, CCPS or CCD. For non-resident investors, only fully and mandatorily convertible instruments count as FDI; optionally convertible instruments are debt (ECB rules). Conversion formula, conversion triggers, floor and cap |
| 2 | Pricing | Issue price backed by a valuation report: registered valuer for Companies Act purposes; for non-residents, not below fair value by an internationally accepted method certified by a CA, SEBI-registered merchant banker or practising cost accountant (FEMA NDI Rules). Income-tax angel tax provisions under s. 56(2)(viib) were removed for allotments from AY 2025-26; confirm the position for the allotment date |
| 3 | Sectoral cap and route | FDI automatic vs government route for the company's sector; downstream investment if the company invests further |
| 4 | Process | Board approval, special resolution for preferential allotment (s. 62(1)(c)), private placement offer letter (PAS-4) to identified persons, money received from the investor's own bank account into a separate bank account, allotment within 60 days of receipt or refund within 15 days thereafter, return of allotment (PAS-3) within 15 days of allotment, MGT-14 for the special resolution. Confirm current timelines |
| 5 | Economic rights | Liquidation preference (1x non-participating is market; flag participating or >1x), anti-dilution (broad-based weighted average is market; flag full ratchet), dividend on CCPS (usually nominal, non-cumulative) |
| 6 | Control rights | Board seats and observer, quorum requiring investor director, affirmative vote matters (keep to genuinely material matters so the business can run), information rights |
| 7 | Transfer rights | Lock-in on founders, ROFR / ROFO, tag-along, drag-along (threshold, minimum price, reps limited to title and capacity), exit timeline (IPO / strategic sale / buyback) and what happens if exit is not achieved |
| 8 | Founder terms | Vesting / reverse vesting, non-compete (enforceable during association; post-exit only as part of a sale of goodwill under s. 27 exception), good leaver / bad leaver |
| 9 | Enforceability | Rights must be written into the articles to bind the company and future shareholders; check the amended articles mirror the SHA. For public companies, transfer restrictions are enforceable only as contracts between shareholders (s. 58(2)) |
| 10 | FEMA reporting | FC-GPR on the FIRMS portal within 30 days of allotment; KYC of the remitter; FC-TRS for secondary transfers; annual FLA return. Confirm current timelines |
| 11 | Warranties and indemnity | Disclosure letter, caps, baskets, survival, founder personal liability (resist uncapped) |
| 12 | Stamp duty | Stamp duty on issue of shares (0.005% under the Indian Stamp Act as amended, collected through the depository or paid on the certificate) and on the SHA / SSA under the state Stamp Act |

## Output

1. Work-product header.
2. Deal summary: instrument, amount, post-money, investor stake fully diluted, key economic and control terms in one table.
3. Issues table with RED / AMBER / GREEN for our side and proposed language.
4. Pro-forma cap table after the round (and after ESOP pool top-up if the term sheet requires it pre-money).
5. Closing checklist with owners and statutory deadlines.
6. Articles amendment checklist.

## Failure modes

- Accepting an option-pool top-up "pre-money" without showing founders the real dilution.
- Issuing CCPS to a non-resident below FEMA fair value.
- Forgetting that the separate bank account and 60-day allotment rule apply even to small rounds.
- SHA rights that never make it into the articles.

## Guardrails

- Start every deliverable with `DRAFT | For review by Indian counsel | Not legal advice`.
- Treat every timeline, rate and threshold above as a working baseline and mark it "confirm against the current text"; RBI, SEBI, MCA, stamp and tax rules change often.
- Check the user's stated legal premises before building on them, and say plainly when one is wrong.
- Never file, send or submit anything; prepare it and hand it back.
- The fuller shared guardrails are in this plugin's `CLAUDE.md`.
