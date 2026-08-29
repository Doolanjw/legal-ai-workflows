# Vendor Contract Negotiation Playbook: SaaS and Data Services

> **DEMONSTRATION MATERIAL.** This playbook is invented for a legal AI
> workflow demonstration. The company it speaks for, Meridian
> Fabrication Group, Inc., is fictional, and so is every position,
> threshold, and role in it. It is not legal advice and not a template
> for actual use.

**Issued by:** Office of the General Counsel, Meridian Fabrication
Group, Inc. (buyer side)
**Applies to:** subscriptions to hosted software and data services
that will receive company operational data
**Version:** 4.1, August 2026

## Purpose

The positions below are market-standard buyer-side stances for SaaS
and data services procurement. What this exhibit demonstrates is
encoding them into an executable review, with planted traps, human
gates, and a verification pass, so a model can run the comparison and
a person still rules the calls that matter.

This playbook records the company's settled negotiating positions so
that contract review is comparison against a decided standard, not
improvisation. Each clause family below carries three lines. STANDARD
is what we ask for and expect to get. FALLBACK is the worst position
the reviewer may accept without asking anyone. ESCALATE names the
conditions that take the decision away from the reviewer entirely and
send it to the person listed. The escalation lines are the point of
the document. They mark where a decision is expensive enough, or
strategic enough, that it must be made fresh by someone accountable
for it, no matter how fluent the analysis in front of them looks.

A reviewer, human or machine, applies this playbook. It does not
argue with it. If a position here is wrong for a particular deal, the
fix is a ruling from the General Counsel recorded in the deal file,
not a quiet exception.

## Reading rules

These rules govern how the paper is read before any position is
compared. Most bad deals are signed by people who read well but read
in the wrong order.

- **RR-1. The contract is the entire stack.** Body, order forms,
  schedules, exhibits, policies incorporated by reference, and
  anything a URL pulls in. A term is binding wherever it sits. A
  schedule is not an attachment to the contract. It is the contract.
- **RR-2. Chase every cross-reference to its target and read the
  target.** "As set forth in the Order Form," "subject to Section X,"
  and "notwithstanding anything to the contrary" are not summaries.
  Each one changes the meaning of the sentence it lives in, and the
  change is only visible at the target.
- **RR-3. Check for absence.** Each family below includes terms whose
  absence is a deviation. Silence in a vendor draft is a drafting
  choice made by the vendor.
- **RR-4. Recompute every formula and every date across the stack.**
  Escalators, caps, notice windows, and cure periods get arithmetic,
  not adjectives. Where two documents each contribute half of a
  formula, the formula is the combination.
- **RR-5. Read defined terms by their definitions, not their
  labels.** A label borrowed from another discipline ("de-identified,"
  "aggregated," "shared responsibility") imports nothing but the
  words. What the definition actually does is all it does.
- **RR-6. Apply the stack's own precedence rules to every conflict
  found.** Do not assume the body controls. If the paper says an
  order form controls over the body, then a line item in the order
  form can quietly rewrite a section of the body, and the review must
  treat it that way.

## Severity scale

- **CRITICAL:** signing as written exposes the company to unbounded
  or uncapped loss, loss of rights in company data, or loss of any
  practical exit. Never accepted at reviewer level.
- **HIGH:** material economic or legal exposure. Negotiate before
  signature.
- **MEDIUM:** negotiate, or accept knowingly at fallback with the
  deviation recorded.
- **LOW:** cleanup. Fix if the redline is otherwise open.
- **CONFORMS:** meets standard or fallback. Say so and cite it.

A finding at any severity requires two receipts: the contract
language quoted with its location, and the playbook line it is
measured against. A finding without both is not a finding.

---

## PB-1. Limitation of liability

Why we hold this line: the cap is the price of the vendor's failure,
set in advance. A cap that looks mutual but excludes only the things
a customer does is not mutual, and an enhanced cap that sits beneath
a damages waiver is not enhanced.

- **STANDARD:** mutual aggregate cap at twelve (12) months of fees.
  A separate enhanced cap of three (3) times twelve months of fees
  for claims arising from security incidents or breach of
  confidentiality or data protection obligations. Excluded from both
  caps, for both parties: indemnification obligations, gross
  negligence, willful misconduct. The mutual waiver of consequential
  damages must state expressly that the costs of responding to a
  security incident (notification, call centers, credit monitoring,
  forensic investigation, and regulatory fines or penalties passed
  through to the company) are direct damages and are recoverable.
- **FALLBACK:** enhanced cap of two (2) times twelve months of fees,
  with the direct-damages sentence for incident response costs
  preserved intact. The direct-damages sentence is not tradeable at
  reviewer level.
- **ESCALATE WHEN:** any cap below twelve months of fees. Any
  structure in which incident response damages fall inside the
  consequential damages waiver. Any exclusion list that operates
  asymmetrically, including by excluding only the customer-side
  indemnity from the caps. Decision: Associate General Counsel,
  Commercial, with the Chief Financial Officer.

## PB-2. Indemnification

Why we hold this line: indemnities allocate the claims we cannot
price. The two we always buy are infringement (the vendor's product
is the vendor's problem) and data breach (their custody, their
failure, their check).

- **STANDARD:** vendor defends and indemnifies against (a) third
  party IP infringement claims arising from the platform, with the
  standard remedy trilogy (procure the right, modify or replace, or
  terminate and refund prepaid fees), and (b) third party claims,
  regulatory fines, and legally required notification costs arising
  from a security incident caused by the vendor's breach of its
  security obligations. Procedures: prompt notice (with prejudice
  qualifier), indemnitor control, no settlement imposing non-monetary
  obligations without consent. Both parties' indemnification
  obligations sit outside the liability caps.
- **FALLBACK:** infringement indemnity limited to United States
  claims. Breach indemnity keyed to the vendor's failure to meet its
  written security schedule rather than strict liability.
- **ESCALATE WHEN:** any carve-back, condition, allocation matrix, or
  "shared responsibility" language, in any document of the stack,
  that reduces or hollows the security indemnity. Any customer-side
  indemnity that reaches beyond our data, our misuse, and our
  systems. Decision: Associate General Counsel, Commercial.

## PB-3. Data ownership and use

Why we hold this line: our process data is the company. Cycle times,
scrap rates, supplier pricing, and cost structures describe how we
make money. A vendor right to reuse that data in any form the vendor
sells is a transfer of competitive information, whatever the clause
calls itself.

- **STANDARD:** the company owns its data and everything derived from
  it, except platform telemetry that contains no data content. Vendor
  license limited to hosting and processing as necessary to serve us,
  during the term. No commercialization of company data in any form.
  On exit, deletion of company data and derived stores, certified in
  writing.
- **FALLBACK:** participation in vendor benchmarking permitted only
  through a separate written opt-in that lists the specific fields
  shared, requires removal of content that reveals our processes or
  costs (not merely removal of our name), and is revocable.
- **ESCALATE WHEN:** any perpetual or irrevocable license to company
  data. Any right to commercialize company data in "aggregated,"
  "de-identified," "anonymized," or any other renamed form. Any
  survival of data rights past termination. Decision: General
  Counsel, personally.

## PB-4. Security and breach notice

Why we hold this line: in an incident the clock is the whole game.
Our regulatory and customer notification duties run from awareness,
so the vendor's clock must too. A vendor that gets to decide when it
has "confirmed" an incident holds our clock in its pocket.

- **STANDARD:** written security program aligned to a recognized
  framework, annual SOC 2 Type II (or equivalent) with the report
  available on request, encryption in transit and at rest, annual
  penetration testing, breach notice within forty-eight (48) hours of
  becoming aware of an actual or reasonably suspected incident,
  cooperation with our investigation, and vendor bears its own
  response and remediation costs.
- **FALLBACK:** notice within seventy-two (72) hours of awareness.
- **ESCALATE WHEN:** the notice clock runs from confirmation,
  validation, or completed investigation rather than awareness, or
  notice is conditioned or qualified. Any right to weaken the
  security schedule during the term. Decision: Associate General
  Counsel, Commercial, with the Chief Information Security Officer.

## PB-5. Term and auto-renewal

Why we hold this line: auto-renewal is a defect that compounds. Every
month of renewal term beyond what we would choose fresh, and every
day of notice window beyond what a calendar reminder can catch, is
leverage we handed the vendor for free.

- **STANDARD:** initial term up to thirty-six (36) months is
  acceptable if priced for it. Renewal terms of twelve (12) months or
  less. Non-renewal on sixty (60) days' notice. No restriction on how
  early notice may be given.
- **FALLBACK:** non-renewal notice up to ninety (90) days.
- **ESCALATE WHEN:** any renewal term longer than twelve (12) months.
  Notice requirement longer than one hundred twenty (120) days. Any
  provision that voids or penalizes early notice of non-renewal.
  Decision: business owner (VP Operations) with Associate General
  Counsel, Commercial.

## PB-6. Price escalation

Why we hold this line: renewal is where the real price of year one is
collected. An uncapped index formula with a floor is not an inflation
adjustment. It is a one-way ratchet, and a ratchet split across two
documents is still one ratchet.

- **STANDARD:** all rates (subscription, usage, overage, and services
  rates) fixed for the initial term. Renewal increases capped at
  three percent (3%) per year or the CPI change, whichever is lower.
  One formula, one adjustment date, applied to all rates together.
- **FALLBACK:** renewal increases capped at five percent (5%) per
  year. No compounding within any term.
- **ESCALATE WHEN:** any uncapped formula. Any floor above five
  percent (5%). Any adjustment that operates during a term the
  contract describes as fixed. Any escalator split across documents
  so that different rate classes move on different clocks. Decision:
  Chief Financial Officer.

## PB-7. Termination rights

Why we hold this line: a contract's real price includes the cost of
leaving it. We do not sign agreements whose only exit is the end of
the term, because every negotiation after signature is conducted
against that fact.

- **STANDARD:** termination for material breach with a thirty (30)
  day cure. Termination for insolvency events. Customer termination
  for convenience after the first contract year on sixty (60) days'
  notice with a pro rata refund of prepaid fees. Vendor suspension
  rights limited to nonpayment after notice and cure, or genuine
  security risk. Transition assistance for up to ninety (90) days at
  then-current rates. Refund of prepaid fees on any customer
  termination for cause.
- **FALLBACK:** no convenience termination during the initial term,
  if and only if chronic service level failure and vendor change of
  control each carry their own termination right.
- **ESCALATE WHEN:** the deal as drafted leaves no exit before end of
  term other than vendor breach. Any vendor right to suspend without
  notice for reasons other than security. Decision: Associate General
  Counsel, Commercial.

## PB-8. Assignment and change of control

Why we hold this line: we priced this vendor, not whoever buys it. If
the vendor is acquired, the acquirer gets the contract only on terms
that protect the data, and we get the choice to leave.

- **STANDARD:** no assignment without consent, except to affiliates
  and to a successor by merger or sale of substantially all assets,
  provided (a) the successor is not a competitor of the company, (b)
  notice within ten (10) days of closing, and (c) the company may
  terminate on notice within sixty (60) days after a vendor change of
  control, with a pro rata refund. Company data and any license to it
  never transfer beyond what is necessary for the successor to
  continue serving us under this contract.
- **FALLBACK:** the competitor restriction may be dropped if the
  change of control termination right and the data limitation stand.
- **ESCALATE WHEN:** any automatic transfer of company data, or of
  any license to company data, to an assignee or successor. Any
  vendor change of control without a customer termination right.
  Decision: General Counsel, personally.

## PB-9. IP license scope (license to the company)

Why we hold this line: the license is the product. We buy access for
the whole company we actually are, we keep what the platform makes
from our data, and a billing dispute is a billing dispute, not an
infringement case.

- **STANDARD:** subscription license for all users of the company and
  its affiliates, coextensive with the term. Outputs, reports, and
  dashboards built from our data are our data. Export in standard
  formats at no charge, during the term and at exit. License rights
  not conditioned on payment status; nonpayment is addressed by the
  suspension and termination clauses, not by converting use into
  infringement.
- **FALLBACK:** licensing by named facility with an annual true-up.
- **ESCALATE WHEN:** the vendor claims ownership of outputs derived
  from our data. Any condition that makes license rights lapse
  automatically on a payment dispute. Decision: Associate General
  Counsel, Commercial.

## PB-10. SLA and remedies

Why we hold this line: an SLA is only as real as its worst month and
its amendment clause. Credits are a pricing adjustment, not a remedy,
and an SLA the vendor can rewrite by posting is not an SLA. It is a
press release.

- **STANDARD:** availability commitment of 99.9% measured monthly.
  Credits applied automatically, without a claim. Termination for
  chronic failure (three consecutive months, or any four months in a
  rolling twelve, below commitment) with a pro rata refund. The
  service level schedule amendable only by signed amendment. Credits
  are not the exclusive remedy for chronic failure.
- **FALLBACK:** 99.5% commitment with claimed credits, if the chronic
  failure termination right stands and the schedule cannot be changed
  unilaterally.
- **ESCALATE WHEN:** any mechanism, anywhere in the stack, by which
  the vendor can amend the service level schedule or any other
  contract term unilaterally, including by posting revised terms.
  Credits as sole remedy with no chronic failure exit. Decision:
  Associate General Counsel, Commercial, with the business owner.

## PB-11. Insurance

Why we hold this line: the indemnity is only as good as the balance
sheet behind it, and vendor balance sheets are opinions. Insurance is
the part of the indemnity we can verify.

- **STANDARD:** commercial general liability at one million dollars
  ($1,000,000) per occurrence and two million dollars ($2,000,000)
  aggregate, umbrella of five million dollars ($5,000,000),
  technology errors and omissions and cyber liability of five million
  dollars ($5,000,000) per claim and aggregate, workers'
  compensation as required by law, certificates furnished annually,
  and thirty (30) days' notice of cancellation or material reduction.
- **FALLBACK:** cyber limits of three million dollars ($3,000,000) if
  the umbrella sits over the cyber tower.
- **ESCALATE WHEN:** cyber limits below two million dollars
  ($2,000,000), or any self-insurance representation in place of
  policies. Decision: Associate General Counsel, Commercial, with the
  risk manager.

## PB-12. Governing law and venue

Why we hold this line: we litigate where we said we would, under law
we chose on purpose. One dispute clause per contract. A stack that
points to two courthouses has not chosen either one. It has chosen a
motion fight before the merits.

- **STANDARD:** Ohio law. Exclusive venue in the state or federal
  courts sitting in Montgomery County, Ohio.
- **FALLBACK:** Delaware or New York law. A neutral venue or the
  defendant's home forum. Jury waiver acceptable. No arbitration
  without General Counsel approval.
- **ESCALATE WHEN:** any non-United States law or venue. Arbitration.
  Conflicting governing law or venue provisions anywhere within the
  stack, whatever the order of precedence resolves them to. Decision:
  General Counsel, personally.

---

## Applying this playbook

The reviewer produces a finding for every family, including the
families where the paper conforms. Every ESCALATE condition met is
routed to the named decision maker as a gate item with the decision
question stated. The reviewer may draft a proposed disposition for a
gate item, marked as a proposal. The reviewer does not rule on gate
items, and a review is not complete while a gate item is unrouted.

*Invented for demonstration. No real company, policy, or person is
depicted.*
