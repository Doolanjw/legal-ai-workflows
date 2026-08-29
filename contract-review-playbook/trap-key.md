# TRAP KEY (DEMO AUTHOR MATERIAL)

THIS FILE IS NOT PART OF THE REVIEWED RECORD. It is the demo author's
answer key for the contract review exhibit. The vendor draft, the
parties, and every term and figure are invented fiction for a legal
AI workflow demonstration. This file is withheld from every stage of
the review run. Nothing here is legal advice.

The vendor draft contains seven planted traps. Each one is built to
defeat a different way that a fluent reader, human or model, fails. A
reviewer can be fluent, careful sentence by sentence, and still miss
all seven, because none of them lives inside a single bad sentence. A
correct review under the playbook and protocol catches all seven. A
naive single pass does not.

RUN NOTE (2026-08-28): in the production run, the protocol review
caught six of the seven outright. T3 was caught in part on the first
pass (the asymmetric exclusion list) and in full on the Stage 5
verification pass (the waiver that empties the enhanced cap), with
this key still closed to every stage. The verification report records
both the partial and the completion, with receipts.

## T1. The schedule that guts the indemnity

**Failure mode targeted: body-first reading. Legal terms hiding in a
technical document.**

Planted: Schedule A, Section A-9 ("Shared responsibility;
limitation"), the last section of the security schedule.

Section 23.2 of the body gives Customer a solid security incident
indemnity: defense, damages, regulatory fines, notification costs.
Schedule A reads as a technical security document for eight sections
(encryption, SOC 2, subprocessors, backups), and then Section A-9
opens with "Notwithstanding anything to the contrary in this
Agreement, including Sections 11 and 23" and removes the indemnity
for any incident "arising from or contributed to by" (a) any act or
omission of Customer or any User, including credential management,
(b) Customer's configuration choices, (c) Customer Systems, or (d)
"Customer Data as transmitted to the Platform by or on behalf of
Customer", with "arises from" defined as cause in fact "in any
degree."

Why a fluent reviewer misses it: reviewers read the body as law and
the schedules as engineering. Eight sections of genuinely standard
security content buy the ninth section a pass, and "shared
responsibility" pattern-matches to ordinary cloud practice. But every
incident involving Customer Data is, in some degree, contributed to
by data Customer transmitted, and credential compromise is the most
common attack path. Clause (d) plus the "in any degree" causation
definition reduces the Section 23.2 indemnity to nearly zero without
touching Section 23.2.

Playbook family violated: PB-2 (Indemnification), ESCALATE trigger
("any carve-back, condition, allocation matrix, or shared
responsibility language, in any document of the stack, that reduces
or hollows the security indemnity"). Reading rule RR-1.

The correct catch: quote A-9 next to 23.2, state that clause (d)
swallows the indemnity because all Customer Data is transmitted by or
on behalf of Customer, grade CRITICAL, route to the gate, and redline
A-9 to a true allocation clause (indemnity reduced only to the extent
an incident results solely from Customer's breach of its own
obligations).

## T2. The escalator split across two documents

**Failure mode targeted: composition. No single sentence is wrong,
and the defect only exists when three passages are read as one
machine.**

Planted: body Sections 16.1, 16.2, and 18.2, with Order Form
Sections 5 and 6.

The body says Subscription Fees are "fixed for the Initial Term" and
that adjustments happen "as set forth in the applicable Order Form."
The Order Form then runs two escalators on two clocks: a Renewal
Adjustment (the greater of 6% or CPI-W plus 2%, compounding at each
renewal) on Subscription Fees, and an Anniversary Adjustment that
raises the Overage Rate and the Professional Services rate every
single year, including the years inside the "fixed" Initial Term,
because the Section 1.17 definition of Subscription Fees excludes
those rates. Renewal terms are 24 months, the non-renewal notice
must arrive at least 180 days out, and a notice sent more than 270
days out is void, so the practical exit window is a 90 day slot that
opens once every two years.

Why a fluent reviewer misses it: each passage is individually
ordinary. "Fixed for the Initial Term" is reassuring, a renewal
escalator is expected, and an anniversary adjustment clause reads as
housekeeping. The trap only appears when the definition of
Subscription Fees, the two adjustment clauses, and the renewal window
are composed and the arithmetic is run: the overage rate is up 6%
by month 12 of the "fixed" term ($1,150 to $1,219.00), up again at
month 24 ($1,292.14), the floor is 6% with an uncapped CPI-plus-2
topside, and both curves compound indefinitely against a 90 day exit
slot every 24 months.

Playbook family violated: PB-6 (Price escalation), ESCALATE triggers
(uncapped formula, floor above 5%, adjustment during a fixed term,
escalator split across documents), and PB-5 (Term and auto-renewal),
ESCALATE triggers (renewal term over 12 months, provision voiding
early notice). Reading rules RR-2 and RR-4.

The correct catch: quote all five passages, run the numbers on the
page, grade HIGH or worse, route both gates, and redline to one
capped formula on one date with 12 month renewals and an open notice
window.

## T3. The exception that swallows the cap

**Failure mode targeted: checklist matching. The clause contains
every expected part, and the defect is in how the parts interact.**

Planted: body Sections 26.1, 26.3, and 26.4.

The limitation of liability section looks buyer-negotiated. There is
a mutual 12 month cap (26.2), an Enhanced Cap of two times that
amount for Security Incident claims (26.3), and an exclusions list
(26.4). Two mechanisms defeat it. First, 26.3's quiet second
sentence provides that "[t]he Enhanced Cap is subject to Section
26.1", and 26.1's waiver list expressly waives the actual damages a
data breach produces: notification costs, call centers, credit
monitoring, forensic investigation, regulatory fines, and amounts
paid to third parties. The Enhanced Cap therefore caps a category of recoverable
damages that the waiver has already emptied. Second, 26.4 is drafted
in mutual voice ("a party's indemnification obligations") but the
only indemnity it lifts out of the caps is Section 24, the Customer
side indemnity. The vendor's Section 23 indemnities stay inside the
capped and waived structure. Customer's exposure is uncapped where it
matters and vendor's is capped twice.

Why a fluent reviewer misses it: the checklist says cap, enhanced
cap, exclusions, and all three are present. The facially mutual
"a party's" phrasing reads as symmetry, and the asymmetry appears
only when the cross-reference is resolved and someone asks which
party ever owes anything under Section 24. The waiver interaction
appears only when someone lists what a breach actually costs and
walks the list against 26.1. Fluency affirms the structure. Only the
interaction analysis breaks it.

Playbook family violated: PB-1 (Limitation of liability), ESCALATE
triggers (incident response damages inside the consequential waiver,
asymmetric exclusion list). Reading rules RR-2 and RR-3.

The correct catch: quote 26.3's second sentence and the 26.1 list
together, state that the Enhanced Cap is nearly empty, expose the
26.4 asymmetry by resolving the cross-reference, grade CRITICAL,
route the gate, and redline a direct-damages sentence for incident
response costs plus a symmetric exclusions list covering both
parties' indemnities.

## T4. Change of control with the data in the moving van

**Failure mode targeted: omission detection. Everything present is
standard, and the harm is one added sentence plus two missing
rights.**

Planted: body Section 29, second sentence.

The assignment clause begins as boilerplate: no assignment without
consent, excepting affiliates and merger or asset sale successors.
Then one sentence provides that upon a Provider assignment, "all
rights and licenses granted to Provider under this Agreement,
including under Section 8, and all Customer Data then in Provider's
possession or control, transfer to and vest in the assignee without
further action or notice." Combined with the Section 8.2 perpetual
license (trap T7), an acquirer of the vendor, including Customer's
direct competitor or a data broker, inherits Customer's production
data and a perpetual right to exploit it in aggregated form. There is
no notice obligation, no competitor restriction, and no Customer
termination right on change of control anywhere in the stack.

Why a fluent reviewer misses it: the clause matches the standard
pattern a reviewer verifies for presence (consent requirement, merger
exception, void assignments). The added sentence is dressed as a
clarification of what assignment means, and the two protections that
would matter are absent rather than wrong. Reviewers audit what is on
the page far more reliably than what is not.

Playbook family violated: PB-8 (Assignment and change of control),
ESCALATE triggers (automatic transfer of company data or licenses,
change of control without customer termination right), with PB-7
(Termination rights) implicated by the missing exit. Reading rule
RR-3.

The correct catch: quote the transfer sentence, name the two
absences as findings with playbook receipts, grade CRITICAL, route to
the General Counsel gate, and redline for successor limitations,
closing notice, a change of control termination right with pro rata
refund, and a bar on data transfer beyond continued service delivery.

## T5. Two courthouses in one stack

**Failure mode targeted: precedence applied in the abstract. The
reviewer knows the precedence rule and still files the body's clause
as the answer.**

Planted: body Section 32 against Order Form Section 7, Additional
Term 3, armed by body Section 3.2.

Section 32 is a clean Delaware package: Delaware law, exclusive
jurisdiction in New Castle County, jury waiver. Order Form Additional
Term 3 requires all actions "arising out of or relating to this Order
Form or the Agreement" to be brought exclusively in Travis County,
Texas. Section 3.2 provides that a conflicting Order Form controls
over the body. Read together, the stack's own precedence rule moves
venue to the vendor's home county in Texas while leaving Delaware
governing law in place, and it does so in a paragraph most reviewers
treat as commercial housekeeping.

Why a fluent reviewer misses it: governing law gets checked in the
body, where lawyers expect it, and the answer there is fine under the
playbook fallback (Delaware law, defendant's home forum). Order form
"Additional Terms" read as administrative (purchase order handling,
invoicing), and the reviewer who read Section 3.2 hours earlier does
not connect it to a venue line in a fee document. The conflict is
real, the resolution is automatic, and it runs in the vendor's favor.

Playbook family violated: PB-12 (Governing law and venue), ESCALATE
trigger (conflicting governing law or venue provisions anywhere
within the stack). Reading rules RR-1 and RR-6.

The correct catch: quote Section 32, Additional Term 3, and Section
3.2 together, state the resolved outcome (Texas venue, Delaware law,
by the stack's own rule), grade HIGH, route the gate, and redline to
strike Additional Term 3 or conform it to the body.

## T6. The SLA that amends itself

**Failure mode targeted: register misclassification. A legal power
placed in an operational document, laundered by boilerplate.**

Planted: Schedule B, Section B-7, with body Section 33.2.

The amendment clause in the boilerplate says no amendment is
effective without a signed writing, "[e]xcept as expressly provided
in this Agreement". Schedule B, Section B-7 is the express provision:
Provider may revise the entire service level schedule by posting to
its support portal, effective in 30 days, with continued use deemed
acceptance. The tail of B-7 completes the trap: if a revision
materially degrades the availability commitment, Customer's exclusive
remedy is non-renewal under Section 18.2, which trap T2 has already
narrowed to a 90 day window every 24 months. The vendor can lower the
SLA in month 4 of a 36 month term, and the contract's answer is that
the customer may leave when the Initial Term ends, thirty two months
later.

Why a fluent reviewer misses it: the reviewer verifies the amendment
clause in the boilerplate, finds the signed-writing requirement, and
checks the box. The generic exception tail reads as drafting caution
rather than as a live pointer, and the SLA is skimmed as operations
material (uptime percentages, credit tables). A posting right in an
SLA does not look like an amendment clause. It is one.

Playbook family violated: PB-10 (SLA and remedies), ESCALATE trigger
(any mechanism anywhere in the stack by which the vendor can amend
unilaterally, including by posting), compounded by credits as sole
remedy with no chronic failure exit. Reading rules RR-1, RR-2, and
RR-5.

The correct catch: quote B-7 and 33.2 together, state that the
exception tail activates the posting right, trace the exclusive
remedy into the T2 renewal window and price the exit, grade
CRITICAL, route the gate, and redline B-7 to signed-amendment-only
with a chronic failure termination right.

## T7. The license that eats the confidential data

**Failure mode targeted: term-of-art pattern matching. Privacy
vocabulary doing trade secret damage.**

Planted: body Section 8.2, armed by the Section 1.2 definition,
Section 20.3(c), and Section 27.6.

Section 8.2 grants the vendor a perpetual, irrevocable license to use
Customer Data to improve its products and to "create, use, market,
and commercialize Aggregated Data," including in industry
benchmarking products. The Section 1.2 definition requires only that
Aggregated Data not identify Customer "as its source." It does not
require removal of the content: cycle times, scrap rates, supplier
pricing, cost structures, the operational facts that are the
company's confidential information. Section 20.3(c) lets the vendor
keep Aggregated Data after termination, and Section 27.6 provides
that nothing in the confidentiality section limits the Section 8
licenses. The confidentiality clause and the deletion clause both
yield, by their own terms, to the license.

Why a fluent reviewer misses it: aggregation and de-identification
are privacy vocabulary, and in a privacy context non-attribution is
most of the protection, because the harm runs through identifying a
person.
Here the data subjects are machines and processes, and the harm is
the content itself reaching competitors as a benchmark, with or
without the company's name on it. A reviewer who pattern-matches the
vocabulary instead of reading the definition approves a perpetual
trade secret outflow because it was labeled with the word that means
harmless somewhere else.

Playbook family violated: PB-3 (Data ownership and use), all three
ESCALATE triggers (perpetual or irrevocable license,
commercialization in renamed form, survival past termination).
Reading rules RR-3 and RR-5.

The correct catch: quote 8.2 with the 1.2 definition and state what
the definition does not require, connect 20.3(c) and 27.6 as the
survival and confidentiality overrides, grade CRITICAL, route to the
General Counsel gate, and redline to a service-only license, content
level de-identification standards, an opt-in for any benchmarking,
and deletion of derived stores at exit.

---

## Design note

The seven traps are one argument made seven ways: contract risk does
not live in sentences, it lives in structure. A trap in a schedule
(T1), a trap in arithmetic across documents (T2), a trap in clause
interaction (T3), a trap in what is missing (T4), a trap in
precedence (T5), a trap in document register (T6), and a trap in a
borrowed label (T7). Fluent reading, which grades sentences, misses
all seven for seven different reasons. The playbook's reading rules
RR-1 through RR-6 exist because judgment about how contracts actually
fail was frozen into rules a reviewer can execute. The protocol makes
the rules run in order, and the gates make a human rule on everything
the rules surface.

*Invented for demonstration. No real company, person, or agreement is
depicted.*
