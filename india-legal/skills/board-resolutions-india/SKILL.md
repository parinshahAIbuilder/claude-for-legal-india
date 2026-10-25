---
name: board-resolutions-india
description: >
  Draft board resolutions, circular resolutions, shareholder (ordinary / special)
  resolutions, explanatory statements, notices and certified true copies for Indian
  companies under the Companies Act, 2013 and Secretarial Standards SS-1 / SS-2, and
  tell the user which approvals and MCA filings (MGT-14 and others) each action
  needs. Use when the user mentions board resolution, circular resolution, special
  resolution, EGM, AGM notice, explanatory statement, certified true copy, MGT-14,
  authorised signatory, bank account opening, borrowing limits, or any corporate
  action needing approval in India.
argument-hint: "[describe the action] [company type: private / public / listed]"
---

# Board and Shareholder Resolutions (India)

## Step 1: map the approval path

For the action described, decide and show in a table:

| Question | How to decide |
|---|---|
| Board or shareholders? | Check the Act section for the action and the articles |
| Meeting or circulation? | Matters under s. 179(3) (and the rules under it) must be passed at a board meeting, not by circulation: for example, making calls, authorising buyback, issuing securities, borrowing, investing funds, granting loans or guarantees, approving financial statements and the board's report, diversifying the business, approving amalgamation or takeover. Other matters can go by circular resolution under s. 175 (draft and notes to all directors, approved by a majority entitled to vote, noted at the next meeting) |
| Ordinary or special resolution? | For example: alteration of articles (s. 14), change of registered office between states, preferential allotment (s. 62(1)(c)), ESOP (s. 62(1)(b)), borrowing beyond paid-up capital, free reserves and securities premium (s. 180(1)(c)), loans and investments beyond s. 186 limits, related-party transactions above thresholds (s. 188, ordinary resolution with interested shareholders not voting) |
| Interested directors? | Disclosure under s. 184; interested directors do not vote and are not counted for quorum on that item |
| Filing? | MGT-14 within 30 days for special resolutions and other resolutions listed in s. 117(3) (private companies have exemptions for certain board resolutions; confirm the current exemption). Other forms as the action needs: DIR-12 (director changes), INC-22 (office), SH-7 (capital), PAS-3 (allotment), CHG-1 (charge) |
| Listed company? | Add SEBI LODR: prior intimation, outcome within 30 minutes, Reg 23 RPT approvals, e-voting for shareholder resolutions |

Confirm timelines and exemptions against the current Act and rules before relying on them.

## Step 2: draft

**Board resolution** in the standard Indian format:

> "RESOLVED THAT pursuant to the provisions of Section [x] and other applicable provisions, if any, of the Companies Act, 2013 read with the rules made thereunder (including any statutory modification or re-enactment thereof for the time being in force) and the Articles of Association of the Company, consent of the Board be and is hereby accorded to …
>
> RESOLVED FURTHER THAT [name, designation] be and is hereby authorised to sign, execute and file all documents, forms and returns and to do all such acts, deeds and things as may be necessary to give effect to this resolution."

**Shareholder resolution** with an explanatory statement under s. 102: material facts, the interest of directors and KMP, and any documents available for inspection.

**Certified true copy**: header with company name, CIN and registered office; "Certified true copy of the resolution passed by the Board of Directors at its meeting held on [date] at [place / through video conferencing]"; the resolution; signature of a director or the company secretary with DIN / membership number.

**Minutes** extracts follow SS-1 (board) and SS-2 (general meetings).

## Step 3: hand back

1. Approval path table.
2. Drafts (board resolution, notice and explanatory statement if needed, certified true copy).
3. Filing checklist with form numbers, deadlines (marked "confirm"), attachments and fees basis.
4. Open questions (articles provisions, existing limits approved by shareholders, interested directors).

## Failure modes

- Passing a s. 179(3) matter by circulation.
- Borrowing beyond the s. 180(1)(c) limit with only a board resolution.
- Missing MGT-14 for a special resolution, which attracts additional fees and penalties.
- Copying an authorisation resolution that names a director who has since resigned.

## Guardrails

- Start every deliverable with `DRAFT | For review by Indian counsel | Not legal advice`.
- Treat every timeline, rate and threshold above as a working baseline and mark it "confirm against the current text"; RBI, SEBI, MCA, stamp and tax rules change often.
- Check the user's stated legal premises before building on them, and say plainly when one is wrong.
- Never file, send or submit anything; prepare it and hand it back.
- The fuller shared guardrails are in this plugin's `CLAUDE.md`.
