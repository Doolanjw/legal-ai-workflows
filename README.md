# Legal AI Workflows

Working demonstrations of AI-native legal workflow design with
verification built in, by Jonathan W. Doolan: twenty years of Tennessee
civil litigation (1,000+ matters, roughly 20 bench trials to judgment),
now working full time in AI evaluation as a legal domain expert
building adversarial evaluations for frontier AI models.

The design doctrine behind everything here, in one line: **the model
drafts, the record governs, and a written gate stands between every
draft and the signature.**

## The flagship exhibit

### [Discovery Response Workflow](discovery-response-workflow/)

A complete, end-to-end demonstration: a realistic (wholly invented)
Tennessee employment case with 23 documents and a served set of 22
discovery requests, run through a five-stage AI workflow with written
protocols and deterministic verification. Four failure traps were
planted in the case materials by design; the corpus also contains a
deliberately naive baseline draft for contrast.

**Recorded walkthrough (9 minutes):** [youtu.be/UjKrFztOvA8](https://youtu.be/UjKrFztOvA8)

The numbers, each verifiable in the artifacts:

| Measure | Result |
|---|---|
| Documents triaged, coverage | 23 of 23, every call cited to a passage |
| Planted traps caught by the workflow | 4 of 4, plus one bonus routing beat |
| Citations audited at verification | 111, zero failures |
| Naive baseline (no protocols), same task | 4 privilege failures, 3 record conflicts sworn unflagged, 27 of 28 sentences out of scope |
| Traps visible to any AI stage | 0 (the answer key was withheld from every stage; verification worked blind) |

The part I did not plan: the blind verification pass also caught a
date defect in my own case materials that I had not planted and did
not know was there. The finding, the disposition, and the correction
are preserved in the Stage 5 report. A gate that grades everything
does not care whose work it is checking. That is the point.

## The second exhibit

### [Contract Review Under a Negotiation Playbook](contract-review-playbook/)

Law firms and legal departments run on banks of frozen judgment:
decisions made once, by someone senior, written down so they do not
have to be made again at midnight by someone junior. A negotiation
playbook is exactly such a bank. What AI changes is that the bank
becomes executable. The model can hold every position, chase every
cross-reference, and recompute every formula without getting tired
on page forty. The scarce work, the work this exhibit is about, is
encoding the judgment in the first place and deciding where a person
must still rule.

The setup: a wholly invented vendor SaaS agreement (33 sections, an
order form, two schedules) with seven traps planted in it, each
built to beat fluent reading a different way. One hides in a
schedule, one is split across two documents, one lives in the
interaction of clauses that each look fine, one is an absence, one
rides the order of precedence, one is a legal power dressed as an
operational document, and one is a borrowed privacy label doing
trade secret damage. Against it: a buyer side playbook (twelve
clause families, each with a standard position, a fallback, and an
escalation trigger that routes the decision to a named human), a
written review protocol, and a verification pass that regrades the
review the way opposing counsel would.

The run caught six of the seven traps outright and routed ten
decisions to the people the playbook names. The seventh trap it
caught halfway: the model flagged the asymmetric carve-out in the
liability section but quoted around the sentence that empties the
security cap, and credited a protection that was not there. The
blind verification pass reopened every quotation, caught the
elision, and completed the finding with the answer key still closed
to it. I kept that sequence in the record on purpose. A perfect
scorecard would tell you less about the design than a recovered
failure does, and the recovery is the design: receipts make elision
visible, and a written gate stands between every draft and the
signature here too.

The numbers, each verifiable in the artifacts:

| Measure | Result |
|---|---|
| Traps planted, caught | 7 planted, 6 caught in the memo, 1 completed at verification, 0 escaped |
| Receipts audited at verification | 34 reopened, 2 elided quotes caught (the seventh trap), 1 locator slip corrected |
| Stack coverage | 56 of 56 provisions mapped, every finding quoted to clause and playbook line |
| Human gates routed | 10, each to a named decision role, none ruled by the model |
| Naive baseline, same paper, no protocol | 0 of 7 traps caught, 1 grazed, graded the draft "in line with market" |

The files:

- [the-contract.md](contract-review-playbook/the-contract.md): the
  invented vendor draft, traps included
- [negotiation-playbook.md](contract-review-playbook/negotiation-playbook.md):
  the frozen judgment bank, twelve families, standard, fallback,
  escalate
- [trap-key.md](contract-review-playbook/trap-key.md): the seven
  traps, where planted, why fluent review misses each, what the
  correct catch looks like
- [protocol-contract-review.md](contract-review-playbook/protocol-contract-review.md):
  the written protocol governing the run, authority, stages, gates,
  receipts
- [review-output.md](contract-review-playbook/review-output.md): the
  review memo the run produced, deviation findings with receipts and
  the human decision queue
- [verification-report.md](contract-review-playbook/verification-report.md):
  the blind verification pass, the trap scoring, and the naive
  baseline contrast

As with everything in this repository, every company, person, and
term is invented, and nothing is legal advice.

## Related work

- [AI Governance Program Framework](https://github.com/Doolanjw):
  an operational governance kit (use case intake, four tier risk
  classification aligned to the EU AI Act and NIST AI RMF, governance
  RACI, training plans), designed for deployment rather than academic
  reference.
- *The Combination Engine* (2026): a 43,000-word book on AI-assisted
  patent search and cross-domain innovation discovery, written with
  AI under my direction as a working demonstration of governed AI
  use. [Amazon](https://www.amazon.com/dp/B0GX34MMFR)

## Important notes

Every case, party, document, and fact in this repository is invented.
Nothing here is legal advice, and nothing here reflects any client,
employer, or platform engagement. The demonstration exists to show
workflow and verification design, not to provide templates for actual
litigation use.

## License

[CC BY 4.0](LICENSE): reuse freely with attribution.

## Contact

GitHub: [Doolanjw](https://github.com/Doolanjw) |
LinkedIn: [jonathanwdoolan](https://www.linkedin.com/in/jonathanwdoolan)
