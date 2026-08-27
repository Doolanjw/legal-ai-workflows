# Discovery Response Workflow: AI-Native, With Verification Gates

A complete demonstration of how a litigation task actually gets done
with AI when the workflow is designed by someone who spent twenty
years doing the task and now tests AI systems for a living.

**The task:** defendant's responses to a first set of discovery (12
interrogatories, 10 requests for production) in an invented Tennessee
retaliatory discharge case, *Whitfield v. Cumberland Ridge Logistics,
LLC*, on a 23-document record.

**The design bet:** every AI demo looks impressive. The question that
matters is what catches the model when it is wrong. So the case
materials carry four deliberately planted traps, the kind that appear
in real files every day, and the workflow has to catch them without
ever being told they exist.

## The four traps

1. **The privileged keyword match.** An attorney-client email thread
   textually matches a request for production, down to containing the
   phrase "decision to terminate." A keyword pass produces it; a
   privilege waiver follows.
2. **The date conflict.** The termination memo says the decision
   followed a March 30 review. The client's own HR notes record the
   decision as confirmed March 26. An interrogatory asks, under oath,
   when each decision was made.
3. **The over-answer bait.** An interrogatory asks one narrow
   question: state the reason for the termination. The record is rich
   enough that a helpful drafter volunteers the whole defense
   narrative, including facts that hand the plaintiff a causation
   argument.
4. **The dual-posture document.** One unsigned severance draft is
   responsive to two different requests carrying two different
   objection postures. Folder-based processing produces it under one
   number while objecting under the other.

The full map is in [TRAP-KEY.md](case/TRAP-KEY.md), which was
withheld from every AI stage during the run. The traps were caught
blind or not at all.

## The workflow

Five stages, each governed by a written protocol
([protocols/](protocols/)), each executed by a separate AI agent that
never saw the answer key, with counsel's judgment at the ruled
decision points:

1. **Intake**: requests parsed into a checklist; scope notes; counsel
   sets every objection posture.
2. **Triage**: 100 percent document coverage; every responsiveness
   call cited to the exact passage; an uncited call is a failed call.
3. **Privilege gate**: a written four-prong test; three
   classifications and no fourth; designed to over-refer, never to
   over-clear; borderline calls route to a human with the uncertain
   prong stated.
4. **Drafting**: shells under counsel's postures; answers scoped to
   the question asked; volunteering is a defect.
5. **Verification**: a fresh agent that wrote none of it grades
   everything cold: every citation reopened, every date cross-checked
   against every document, scope audited sentence by sentence,
   privilege leak search, completeness reconciliation.

## What happened

- All four traps caught, plus the bonus beat (an email where counsel
  is merely copied gets routed to human review rather than
  auto-cleared or auto-withheld).
- 111 citations audited at verification: zero failures.
- The interrogatory that invited over-answering got a one-sentence
  scoped answer. The date conflict was flagged for counsel instead of
  sworn. The privileged thread was withheld and logged, with the log
  describing the communication without revealing the advice.

**The contrast exhibit:** the same interrogatory was separately
drafted by a capable AI assistant with full record access and no
protocols
([outputs/stage4-rog7-NAIVE-baseline.md](outputs/stage4-rog7-NAIVE-baseline.md)).
The result is fluent, organized, cited throughout, and wrong three
ways at once: it narrates the substance of privileged legal advice in
a sworn answer, swears to a contradicted timeline without noticing
the contradiction sitting in adjacent sentences, and volunteers 27
sentences beyond the question's scope. The verification report grades
it in full. Fluency is not accuracy. That is why the gates exist.

**The unplanned finding:** the blind verification pass also surfaced
a date defect in the case materials that the author (I) had not
planted and did not know existed. It is preserved, with its
disposition, in the
[Stage 5 report](outputs/stage5-verification-report.md) addendum and
the trap key's production QA note. The gate does not care whose work
it is checking.

## How to read this exhibit

1. [protocols/00-WORKFLOW-MAP.md](protocols/00-WORKFLOW-MAP.md), the
   doctrine in one page.
2. [outputs/00-README-RUN-OF-SHOW.md](outputs/00-README-RUN-OF-SHOW.md),
   the artifact map.
3. The naive baseline, then the protocol Rog 7 answer inside
   [outputs/stage4-response-shells.md](outputs/stage4-response-shells.md),
   side by side.
4. The [verification report](outputs/stage5-verification-report.md),
   which is the heart of the method.
5. The [case materials](case/) last, if you want to see the world the
   workflow ran against.

**Recorded walkthrough (9 minutes):** the author walks the full
workflow on these artifacts, traps and all:
[youtu.be/UjKrFztOvA8](https://youtu.be/UjKrFztOvA8)

## Provenance and disclaimer

Every party, document, name, and fact is invented; any resemblance to
real persons or entities is coincidental. The bar number in the
served requests is deliberately fictional. Nothing here is legal
advice, and none of this content derives from any client, employer,
or platform engagement. Built with Claude and Claude Code under
written protocols; authored and directed by Jonathan W. Doolan.
