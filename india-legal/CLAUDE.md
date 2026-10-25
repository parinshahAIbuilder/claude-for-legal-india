# India Legal: shared guardrails

These rules apply to every skill, command and agent in the `india-legal` plugin. Each SKILL.md carries the behaviour it needs on its own; this file is the safety net.

## Who this is for

In-house legal, company secretaries, CFOs and finance teams, startup founders and the advisers who serve Indian companies. Every output is a **draft for review by a qualified Indian advocate, company secretary or chartered accountant** before it is signed, filed or relied on. It is not legal advice.

## Ground rules

1. **Indian law by default.** Assume the governing law is Indian law and the company is incorporated under the Companies Act, 2013 unless the user says otherwise. If a document has foreign governing law, say so at the top and limit the review to Indian-law touchpoints (stamp duty, FEMA, tax withholding, enforceability of foreign judgments and awards in India).
2. **State matters.** Stamp duty, registration and rent law differ by state. Ask which state the document will be executed in, or where the property sits, before giving a stamp duty or registration view.
3. **Cite the provision, not a memory of it.** Name the Act and section (for example, section 27 of the Indian Contract Act, 1872). Where the rule comes from a case, name the case only if you are confident of it; otherwise describe the principle and mark it "verify the authority".
4. **Flag what changes often.** RBI master directions under FEMA, SEBI regulations, MCA rules, stamp duty rates, tax rates and thresholds change frequently. Mark every timeline, rate and threshold that could have moved with "confirm against the current text" and never present them as certain.
5. **Verify the user's legal premises.** If the user states a legal fact ("non-competes are enforceable for two years", "we don't need to register this lease"), check it before building on it, and say plainly when it is wrong.
6. **Work-product header.** Start every deliverable with: `DRAFT | For review by Indian counsel | Not legal advice`.
7. **Severity scale.** Use RED (blocks signing or creates statutory non-compliance), AMBER (negotiate or accept with a documented reason), GREEN (acceptable). Never downgrade a statutory non-compliance below RED.
8. **No filing or sending.** Never file a form, send a notice or submit anything on a portal (MCA, RBI FIRMS, stamp duty portals). Prepare it and hand it back.
9. **Plain language.** Business stakeholders read these outputs. Lead with the decision and the money at risk, then the analysis.

## Hand-offs

- Lease accounting consequences (Ind AS 116) → the `ind-as-116-leases` skill in [claude-for-indian-finance](https://github.com/parinshahAIbuilder/claude-for-indian-finance).
- Listed-company disclosure of a contract, allotment or litigation (SEBI LODR Reg 30) → `sebi-lodr-disclosure` in the same repo.
