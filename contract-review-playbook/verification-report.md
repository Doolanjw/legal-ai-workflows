# Verification Report: Contract Review Run

> **DEMONSTRATION MATERIAL.** This report is an invented artifact of a
> legal AI workflow demonstration. The parties, the contract, the
> review, and every finding are fictional. Nothing here is legal
> advice.

**Matter:** Corvantic Analytics vendor draft v. Meridian playbook v4.1
**Memo verified:** review-output.md (Protocol CR-1, Stages 1 through
4, run 2026-08-28)
**Record verified against:** the full stack in the-contract.md (body,
Order Form No. 1, Schedules A and B) and negotiation-playbook.md
**This pass:** Protocol CR-1, Stage 5, run 2026-08-28 by the model,
cold, as the memo's adversary

Role note per protocol: this pass grades the memo against the record,
not against the memo's own reasoning. Findings carry receipts and are
ordered by severity. The closing section states what was checked, not
only what was found.

Blind statement: no answer key, issue list, or authoring material was
available to any stage of this run, including this one. Part Two of
this file was added by the demo author after the run, with the trap
key opened for scoring. Part One below is the Stage 5 output as
produced.

---

# PART ONE: THE STAGE 5 VERIFICATION PASS

## 1. Receipt audit

The memo carries 34 fenced receipts: 22 contract quotations and 12
playbook quotations. Every one was reopened against the record.

Grading conventions applied: a bracketed alteration marking a changed
initial letter at the start of an excerpt ("[A]ny", "[T]he") and
quotation marks nested by convention are not defects. A marked
ellipsis passes if the elided language is not operative for the
proposition cited. An elision, marked or unmarked, that drops
operative language fails.

**Result: 31 VERBATIM. 2 FAIL, both in the Section 26 receipts. 1
WRONG LOCATION.**

**Finding V1 (material, reported first per protocol): the memo's two
Section 26 receipts each omit the operative language, and the
omissions carried the analysis.** The memo's quotation of Section
26.3 (memo Section 3.3) reads:

```
Memo receipt: "Notwithstanding Section 26.2, Provider's aggregate
liability for all claims arising from a Security Incident will not
exceed two (2) times the amount stated in Section 26.2 (the
'Enhanced Cap')."
```

The record contains a second sentence the receipt omitted, with no
ellipsis marking the omission:

```
Contract, Section 26.3, in full: "Notwithstanding Section 26.2,
Provider's aggregate liability for all claims arising from a
Security Incident will not exceed two (2) times the amount stated in
Section 26.2 (the 'Enhanced Cap'). The Enhanced Cap is subject to
Section 26.1."
```

Grade: TRUNCATED. The memo's quotation of Section 26.1 (PB-1
finding) uses a marked ellipsis:

```
Memo receipt: "IN NO EVENT WILL EITHER PARTY BE LIABLE FOR ANY
INDIRECT, INCIDENTAL, SPECIAL, CONSEQUENTIAL, EXEMPLARY, OR PUNITIVE
DAMAGES ... HOWEVER CAUSED AND UNDER ANY THEORY OF LIABILITY, EVEN
IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGES."
```

The elision drops this:

```
Contract, Section 26.1, elided language: ", OR FOR ANY LOSS OF
PROFITS, REVENUE, GOODWILL, OR DATA, OR FOR THE COST OF SUBSTITUTE
GOODS OR SERVICES, OR FOR AMOUNTS PAID OR PAYABLE TO THIRD PARTIES,
INCLUDING COSTS OF NOTIFICATION, CALL CENTER SUPPORT, CREDIT
MONITORING OR IDENTITY PROTECTION SERVICES, FORENSIC INVESTIGATION,
OR REGULATORY OR CARD NETWORK FINES, PENALTIES, OR ASSESSMENTS,"
```

Grade: FAIL, ellipsis over operative language. The elided list is
not boilerplate. It is an enumeration of the actual costs of a data
breach, waived by name. The memo characterized Section 26.1 as "a
mutual waiver of consequential damages in customary form" and
credited Section 26.3's Enhanced Cap as "partial mitigation"
preserving "a doubled recovery for the incident scenario." Both
statements depend on the omitted language. Read in full, Section
26.3 makes the Enhanced Cap "subject to Section 26.1," and Section
26.1 waives, by name, notification costs, call center support,
credit monitoring, forensic investigation, regulatory fines, and
amounts payable to third parties. Those categories are approximately
the universe of what a Security Incident costs a manufacturer. The
Enhanced Cap is a doubled cap over a recovery the waiver has already
emptied, and the mitigation the memo credited does not exist.

Consequence, applied under the severity challenge (Section 5 below):
PB-1 is upgraded from HIGH to CRITICAL, and gate G1 is widened. Note
also that the memo's own playbook receipt for PB-1 quoted only the
asymmetry trigger and omitted the adjacent trigger sentence, "Any
structure in which incident response damages fall inside the
consequential damages waiver," which is the trigger this mechanism
trips. The receipt discipline failed in both directions at once, on
the same finding, and nowhere else in the memo.

**Finding V2 (minor): one receipt carries a wrong location.** The
PB-12 finding labels the Travis County venue quotation "Order Form
Section 7, Additional Term 2." The quoted text is verbatim, but it is
Additional Term 3. Additional Term 2 is the purchase order term. The
memo's own Section 3.1 precedence table cites Additional Term 3
correctly, so the error is internal to the PB-12 label. Grade: WRONG
LOCATION, corrected here. No analytical consequence.

**No other defect.** The remaining 19 contract receipts and all 12
playbook receipts reopened VERBATIM, including the marked elisions in
the Section 20.3, Section 29, and Section 32 receipts, each of which
drops only language the memo separately addressed as conforming
(deletion exceptions (a) and (b), the consent requirement, the CISG
sentence).

## 2. Coverage audit

The Stage 1 census was recounted against the record: body Sections 1
through 33, Order Form Sections 1 through 7, Schedule A Sections A-1
through A-9, Schedule B Sections B-1 through B-7. 56 provisions. The
memo's Coverage Appendix maps 56 of 56, and every mapped provision is
either treated in a finding or carries a NO FAMILY reason. Confirmed
complete. The NO FAMILY reasons were reread, and none conceals a
playbook family term. (Section 14, mapped NO FAMILY, contains support
response times. The playbook takes no position on those, and the
mapping stands.)

## 3. Absence re-check

The memo rests three findings on absences (RR-3). Each claimed
absence was rechecked against the entire stack, not the body alone:

- No termination for convenience: confirmed absent. Checked Sections
  18, 19, 20, and 33, all Order Form sections, and both Schedules.
- No chronic SLA failure termination: confirmed absent. Checked
  Sections 13, 19, Schedule B in full.
- No change of control notice or termination right, no successor
  competitor restriction: confirmed absent. Checked Sections 19, 29,
  33, and the Order Form.
- Also confirmed as claimed: no posting or unilateral amendment
  mechanism reaches Schedule A (the B-7 mechanism is limited to
  Schedule B by its terms), and no definition of "confirms" exists
  anywhere in the stack for Section 11.1.

## 4. Recomputation

All Stage 3 arithmetic was rerun independently. All figures in the
memo's Section 3.2 table reproduce: overage $1,150.00 to $1,219.00
(month 12) to $1,292.14 (month 24) to $1,369.67 (month 36) to
$1,942.90 (year 10, nine compounded adjustments at the 6% floor,
68.9% cumulative); services rate $210.00 to $222.60 to $235.96 to
$250.11 to $354.79; subscription $62,400.00 to $66,144.00 (month 36)
to $78,778.56 (year 10, four compounded adjustments, 26.2%
cumulative). Credit arithmetic confirmed: $5,200 monthly prorated
Subscription Fee per Facility, maximum monthly credit $1,040 per
Facility, $3,120 across three Facilities. Enhanced Cap at current
run rate confirmed: two times $187,200 is $374,400, before overage
and services fees. Window dates confirmed by day count: December 4,
2028 is exactly 270 days, and March 4, 2029 exactly 180 days, before
the August 31, 2029 term end (the window spans 90 days, 91 calendar
days counting both ends). The memo's arithmetic stands.

## 5. Severity challenge

For every finding graded below CRITICAL, the strongest case for a
higher grade was stated and resolved:

- **PB-1 (HIGH): UPGRADED TO CRITICAL.** The case for the higher
  grade is finding V1: the mitigation credited in the memo fails when
  the record is read in full. With the Enhanced Cap subject to the
  Section 26.1 waiver, the vendor-side recovery for the incident
  scenario is capped twice and emptied once, while Customer's Section
  24 exposure is uncapped under Section 26.4(b). Under the playbook
  scale ("uncapped or unbounded loss" on one side, loss of effective
  recovery on the other), this is CRITICAL. Gate G1 is widened
  accordingly: the decision question now includes whether the company
  will sign any structure in which incident response damages sit
  inside the consequential damages waiver, per the PB-1 trigger the
  memo did not quote. The proposed redline in the memo's PB-1 finding
  already contains the correct fix (the direct-damages sentence).
  The memo drafted the cure for the disease it graded too low.
- **PB-4 (HIGH): stands.** The case for CRITICAL is the interaction
  of the confirmation-gated clock with Customer's downstream duties.
  It fails because the exposure is bounded by the incident scenario
  and is fully cured by the drafted redline, and the playbook
  reserves CRITICAL for uncapped loss, lost data rights, or lost
  exit.
- **PB-5 and PB-6 (HIGH): stand.** The case for CRITICAL is the
  compounding curve against the 90 day exit slot. It fails, narrowly,
  because an exit does exist and the economics, while escalating, are
  bounded and quantified. The combined structure is priced in the
  exit walk and both gates are routed to the money deciders.
- **PB-7 (HIGH): stands.** The absent exits are individually graded
  in PB-8 and PB-10, both CRITICAL and gated, and grading the
  absence family CRITICAL as well would double-count the same
  exposure.
- **PB-12 (HIGH): stands.** A venue conflict is a motion fight, not
  an unbounded loss. The gate is routed to the General Counsel.
- **PB-9 and PB-11 (MEDIUM): stand.** Bounded, curable by redline,
  no trigger crossed.

Post-verification severity line: 5 CRITICAL, 5 HIGH, 2 MEDIUM.

## 6. Gate queue completeness

Every ESCALATE trigger met anywhere in the run has a queue entry with
a named decision maker and a stated question: G1 through G10
confirmed against the playbook's decision assignments. No gate item
lacks a decision question. No trigger was found met without a queue
entry. G1 is widened by this pass (Section 5). No new gate is
required, because the widened question sits with the same decision
makers the playbook names for PB-1.

---

# PART TWO: TRAP SCORING (DEMO AUTHOR MATERIAL, KEY OPENED AFTER THE RUN)

The seven traps in trap-key.md were withheld from every stage,
including the Stage 5 pass above. This section was written afterward
by the demo author, with the key open, scoring the run trap by trap.

| Trap | Verdict | Where caught | Receipt |
|---|---|---|---|
| T1 Schedule carve-back guts the indemnity | CAUGHT | Memo, PB-2, CRITICAL, gate G2 | A-9 quoted in full next to 23.2; clause (d) named as covering all transmitted data; walk-away proposed |
| T2 Split compounding escalator with renewal window | CAUGHT | Memo, PB-5 and PB-6, gates G5 and G6 | Both clocks caught, including the intra-term Anniversary Adjustment ($1,219.00 at month 12 of the "fixed" term); the void-notice sentence caught; window dated |
| T3 Exception swallows the Enhanced Cap | PARTIALLY CAUGHT first pass; CAUGHT at verification | Memo caught the 26.4 asymmetry (gate G1); Stage 5 finding V1 caught the 26.1/26.3 interaction and upgraded to CRITICAL | Both Section 26 receipts had elided the operative language; the receipt audit exposed the elisions and the severity challenge completed the analysis, with the key still closed |
| T4 Change of control transfers the data | CAUGHT | Memo, PB-8, CRITICAL, gate G8 | Transfer sentence quoted; both absences (notice, termination right) confirmed at Stage 5 absence re-check |
| T5 Venue conflict across the stack | CAUGHT | Memo, PB-12, HIGH, gate G10 | Resolved outcome stated (Texas venue, Delaware law, by Section 3.2); one locator slip (V2) corrected at verification |
| T6 SLA amendable by posting | CAUGHT | Memo, PB-10, CRITICAL, gate G9 | B-7 quoted with 33.2's exception tail; exclusive remedy traced into the 90 day window and priced |
| T7 Aggregated Data license reaches confidential content | CAUGHT | Memo, PB-3, CRITICAL, gate G3 | Definition mechanics named (non-attribution only); survival (20.3(c)) and confidentiality subordination (27.6) connected |

Score: six of seven caught by the review memo. The seventh caught in
part by the memo and in full by the verification pass, before the
key was opened. Zero traps escaped the protocol-governed run.

The author's honest note on T3: the first pass reproduced, inside a
governed run, exactly the failure the trap was built for. The model
saw the checklist parts (cap, enhanced cap, exclusions), quoted the
convenient spans, and graded the family on the strength of a
mitigation it had not traced. What caught it was not intelligence.
It was the receipts requirement (the elisions were visible because
quotes are checkable), the Stage 5 rule that reopens every quote,
and the severity challenge that forces mitigation claims to be
traced like any other claim. The gate was already routed on the
asymmetry, so a person would have reached Section 26 regardless.
That is the design working as intended, and it is also a true record
of the model failing partway before the written process recovered
it.

# PART THREE: THE NAIVE BASELINE, FOR CONTRAST

For contrast, the same vendor draft was run as a single pass with no
playbook and no protocol, instructed only to review the agreement
for the customer and flag concerns. Excerpts from that baseline
output, quoted:

```
Naive baseline: "Overall, this is a fairly standard vendor-form SaaS
agreement. Liability is capped at 12 months of fees with a 2x
super-cap for security incidents, which is in line with market
practice."
```

```
Naive baseline: "Section 8.2 contains standard product improvement
and benchmarking language common in SaaS agreements. Consider
confirming that de-identification is robust."
```

```
Naive baseline: "Schedule A is a reasonably robust security exhibit
(SOC 2 Type II, encryption, annual penetration testing)."
```

```
Naive baseline: "The agreement auto-renews for 24-month terms with
180 days' notice, which is long; consider negotiating to 12 months.
Cyber insurance of $2M may be low for the data involved. There is no
termination for convenience."
```

What the naive pass produced: three real but body-level catches (the
24 month renewal length, the cyber limit, the missing convenience
termination), a partial graze of T2 (the renewal escalator's
existence, without the anniversary clock, the void-notice sentence,
or the arithmetic), and clean misses of T1, T3, T4, T5, T6, and T7.
It read Schedule A for its security content and praised it without
reaching A-9. It read Section 26 as a checklist and called the
structure market. It called the T7 license "standard" by its label.
It never mentioned Order Form Additional Term 3, Section B-7, or
Section 29's transfer sentence. Scored against the key: zero of
seven traps caught, one grazed.

The gap is not fluency. The baseline's sentences are competent, and
several of its observations are correct. The gap is that every trap
in this draft is normal-shaped at the sentence level, and a reviewer
grading sentences against a general sense of market will pass all of
them. The playbook replaces market sense with decided positions. The
protocol forces the reading order that finds structure: the whole
stack, every cross-reference resolved, every formula recomputed,
every absence checked. The receipts requirement makes elision
visible, and the gates put a person on every decision that matters.
The first-pass T3 partial shows the same failure class arising
inside the governed run, and Stage 5 exists because it will.

## What was checked

For the record, this pass checked: 34 receipts reopened against the
record (Section 1); the 56 provision census recounted and every
mapping reread (Section 2); every claimed absence rechecked across
the full stack (Section 3); every figure and date in the memo
recomputed independently (Section 4); every sub-CRITICAL severity
challenged and resolved on the record (Section 5); and the gate
queue reconciled against every trigger the playbook names (Section
6). Findings: V1 (material, upgrade applied), V2 (minor, corrected).
Nothing else was found, and the sentence before this one states what
that claim is based on.

*Invented for demonstration. No real company, person, or agreement is
depicted.*
