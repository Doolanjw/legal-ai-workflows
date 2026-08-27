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
