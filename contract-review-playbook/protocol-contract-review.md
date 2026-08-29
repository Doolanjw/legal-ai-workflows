# Protocol CR-1: Contract Review Under Playbook

> **DEMONSTRATION MATERIAL.** This protocol is invented for a legal AI
> workflow demonstration. The company and playbook it references are
> fictional. It is not legal advice.

Governs any run in which the model reviews a counterparty contract
against the company negotiation playbook. The doctrine in one line:
the playbook holds the judgment, the model runs the comparison, and a
person rules at every gate.

## Scope of the model's authority

The model working under this protocol:

- MAY read the full contract stack, map it, compare it against the
  playbook, grade deviations, draft findings, draft proposed
  redlines, and draft proposed dispositions for gated items, each
  marked PROPOSED.
- MAY NOT rule on any item the playbook escalates. Every ESCALATE
  trigger met is routed to the decision maker the playbook names. A
  gated item is open until a person rules on it.
- MAY NOT accept, reject, or soften any playbook position, or grade
  a deviation as acceptable because it is common in the market. The
  playbook is the standard. Market commentary, if useful, appears as
  a note, never as a verdict.
- MAY NOT communicate with the counterparty, edit the contract text
  itself, or produce anything styled as final legal advice. The
  output is a review memo for counsel.

## Inputs

1. The complete contract stack: body, every order form, every
   schedule and exhibit, and any document incorporated by reference.
   If an incorporated document is unavailable, its absence is a
   finding, not a footnote.
2. The company negotiation playbook, current version, including its
   reading rules and severity scale, which this protocol adopts.
3. Deal context supplied by counsel, if any (data categories
   involved, deal value, incumbent status).

## The run

### Stage 1: Clause map

Build the inventory before forming any opinion.

1. STACK CENSUS: list every document in the stack with its sections.
   State the census total. Every numbered provision in every document
   appears in the map, mapped to one or more playbook families or
   marked NO FAMILY with a one line reason. One hundred percent
   coverage; an unmapped provision is a defect in the run.
2. CROSS-REFERENCE TABLE: every "notwithstanding," "except as,"
   "subject to," and "as set forth in" is resolved to its target, and
   the target is read and quoted. Per reading rule RR-2, a reference
   is not a summary of its target.
3. DEFINED TERM TABLE: every defined term used by a mapped provision
   is quoted with its definition. Per RR-5, terms are read by their
   definitions, not their labels.
4. FORMULA AND DATE REGISTER: every formula, rate, cap, escalator,
   notice period, cure period, and window in the stack, quoted with
   location, for Stage 3 recomputation.

### Stage 2: Playbook comparison

For each playbook family, in playbook order:

1. Assemble every provision the clause map assigned to the family,
   from every document in the stack.
2. State the playbook STANDARD and FALLBACK. Quote the contract's
   actual language with its location.
3. Verdict: CONFORMS (state at which level) or DEVIATES with a
   severity grade under the playbook scale.
4. ABSENCE CHECK per RR-3: for each family, state which expected
   protections are absent, with the playbook line that expects them.
   An absence is graded like any other deviation.
5. GATES: if any ESCALATE trigger is met, open a gate item: quote
   the trigger, quote the contract language that trips it, name the
   decision maker per the playbook, and state the decision question
   in one sentence. A proposed disposition may follow, marked
   PROPOSED.

### Stage 3: Interaction pass

Deviations that live in single clauses are the easy ones. This stage
hunts the ones that live between clauses.

1. PRECEDENCE WALK per RR-6: apply the stack's order of precedence
   provisions to every conflict identified anywhere in the run, and
   state each conflict's resolved outcome.
2. RECOMPUTATION per RR-4: rerun every formula and date in the
   register, including combinations across documents. Show the
   arithmetic. Adjectives are not findings; numbers are.
3. CAP AND REMEDY WALK: trace each indemnity and each remedy through
   every cap, waiver, exclusion, and sole remedy clause that touches
   it, and state what actually remains recoverable at the end of the
   trace.
4. EXIT WALK: enumerate every path out of the contract (non-renewal,
   cause, convenience, chronic failure, change of control), with the
   earliest date each is available and what each costs. A contract
   whose exits all fail is a CRITICAL finding whatever the individual
   clauses graded.
5. SURVIVAL WALK: list what survives termination, and check each
   survival against the playbook families it touches.

### Stage 4: Review memo

Assemble the memo for counsel:

1. Header: stack reviewed, playbook version, protocol version, run
   date, and the statement that nothing in the memo is ruled.
2. Summary table: every playbook family with verdict, severity, and
   gate status.
3. Findings, one per family plus any interaction findings, each
   carrying: the playbook line quoted, the contract language quoted
   with location, the analysis in plain sentences, the severity, a
   proposed redline in draftable language, and the gate routing if
   any.
4. HUMAN DECISION QUEUE: every gate item, numbered, with decision
   maker and decision question. The queue is the memo's most
   important section and appears in full even if empty ("no gates
   tripped" is itself a reportable result).
5. Coverage appendix: the Stage 1 map, showing every provision
   accounted for.

RECEIPTS REQUIREMENT (applies to every stage): every finding quotes
the contract language verbatim with its location AND quotes the
playbook line it is measured against. A finding without both is
rejected at verification. Quotations are verbatim and complete for
the proposition cited; an ellipsis that drops operative language is a
verification failure.

### Stage 5: Verification pass

Run by the model against the finished memo, cold, as the memo's
adversary. The job is to break the memo before the counterparty's
lawyers, or the signature, does.

1. RECEIPT AUDIT: reopen every quotation in the memo against the
   stack. Grade each VERBATIM, TRUNCATED (material language omitted),
   or WRONG (text or location does not match). Any TRUNCATED or WRONG
   grade is reported at the top of the output.
2. COVERAGE AUDIT: recheck the Stage 1 census against the stack.
   Every provision mapped, every mapped provision considered in some
   finding or marked NO FAMILY with reason.
3. ABSENCE RE-CHECK: rerun RR-3 for every family against the
   playbook's expected protections.
4. RECOMPUTATION: rerun all Stage 3 arithmetic independently.
5. SEVERITY CHALLENGE: for every finding graded below CRITICAL,
   state the strongest case for a higher grade, then either upgrade
   the finding or record why the grade stands. Mitigation credited in
   a finding is verified like any other claim: reopen the language
   the mitigation relies on and trace it through every clause that
   touches it.
6. GATE QUEUE COMPLETENESS: every ESCALATE trigger met anywhere in
   the run has a queue entry, and no queue entry lacks a named
   decision maker and a stated question.

Findings are reported with receipts, ordered by severity. A clean
check states what was checked, not just that nothing was found.

## Rules

- The playbook's reading rules RR-1 through RR-6 bind every stage.
- Every quotation carries a location (document, section). An
  unlocated quotation is a failed receipt.
- Severity grades come from the playbook scale and nowhere else.
- The model states uncertainty where it exists. "This clause is
  ambiguous and the readings diverge as follows" is a finding;
  silent selection of the friendlier reading is a defect.
- No stage relies on any answer key, checklist of known issues, or
  material outside the inputs listed above.

## Output

One review memo (Stage 4) and one verification report (Stage 5), each
carrying its receipts, ready for counsel to rule on the queue.

*Invented for demonstration. No real company, person, or agreement is
depicted.*
