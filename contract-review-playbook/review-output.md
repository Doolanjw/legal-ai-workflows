# Contract Review Memo: Corvantic Vendor Draft v. Meridian Playbook

> **DEMONSTRATION MATERIAL.** This memo is an invented artifact of a
> legal AI workflow demonstration. The parties, the contract, the
> playbook, and every finding are fictional. Nothing here is legal
> advice.

**Matter:** Proposed Master Subscription and Services Agreement,
Corvantic Analytics, LLC (vendor form draft transmitted August 21,
2026) with Order Form No. 1, Schedule A, and Schedule B
**Reviewed for:** Office of the General Counsel, Meridian Fabrication
Group, Inc. (Customer)
**Standard applied:** Vendor Contract Negotiation Playbook v4.1
**Protocol:** CR-1 (Contract Review Under Playbook), Stages 1 through 4
**Run date:** 2026-08-28
**Produced by:** the model, under Protocol CR-1

Status line per protocol: nothing in this memo is ruled. Ten gate
items are routed to the decision makers the playbook names, in the
Human Decision Queue below. Proposed dispositions are marked
PROPOSED. The trap or issue count of the source draft, if any exists,
was not available to this run. This memo relies only on the stack,
the playbook, and Protocol CR-1.

## Run summary

- Stack census: 4 documents, 56 numbered provisions (body Sections 1
  through 33, Order Form Sections 1 through 7, Schedule A Sections
  A-1 through A-9, Schedule B Sections B-1 through B-7). Coverage:
  56 of 56 mapped (Coverage Appendix).
- Family verdicts: 0 of 12 families conform in full. 4 CRITICAL, 6
  HIGH, 2 MEDIUM.
- Gate items routed: 10.
- Every finding carries two receipts: the contract language with
  location, and the playbook line it is measured against, per the
  protocol's receipts requirement.

## Summary deviation table

| Family | Verdict | Severity | Contract says (fragment) | Gate |
|---|---|---|---|---|
| PB-1 Limitation of liability | DEVIATES | HIGH | "do not apply to ... a party's indemnification obligations under Section 24" | G1 |
| PB-2 Indemnification | DEVIATES | CRITICAL | "no obligation to indemnify ... any Security Incident to the extent arising from or contributed to by" | G2 |
| PB-3 Data ownership and use | DEVIATES | CRITICAL | "perpetual, irrevocable license ... to create, use, market, and commercialize Aggregated Data" | G3 |
| PB-4 Security and breach notice | DEVIATES | HIGH | "within seventy-two (72) hours, after Provider confirms" | G4 |
| PB-5 Term and auto-renewal | DEVIATES | HIGH | "renewal terms of twenty-four (24) months ... more than two hundred seventy (270) days ... no force or effect" | G5 |
| PB-6 Price escalation | DEVIATES | HIGH | "the greater of (a) six percent (6%) and (b) ... CPI-W ... plus two percent (2%)" | G6 |
| PB-7 Termination rights | DEVIATES | HIGH | no convenience, chronic failure, or change of control exit exists in the stack | G7 |
| PB-8 Assignment and change of control | DEVIATES | CRITICAL | "all Customer Data then in Provider's possession or control, transfer to and vest in the assignee" | G8 |
| PB-9 IP license scope | DEVIATES | MEDIUM | "conditioned on Customer's timely payment of all Fees" | none |
| PB-10 SLA and remedies | DEVIATES | CRITICAL | "may update this Schedule B ... by posting a revised version" | G9 |
| PB-11 Insurance | DEVIATES | MEDIUM | "cyber liability insurance with combined limits of at least two million dollars" | none |
| PB-12 Governing law and venue | DEVIATES | HIGH | "brought exclusively in the state or federal courts sitting in Travis County, Texas" | G10 |

## Stage 3 interaction results

The single-clause comparisons above understate this draft. Five
structural results from the interaction pass are used by the findings
and are reported here once.

### 3.1 Precedence walk (RR-6)

Section 3.2 sets the stack's hierarchy:

```
Contract, Section 3.2: "If an Order Form conflicts with the body of
this Agreement or with a Schedule, the Order Form controls with
respect to the subscriptions and services it covers. If a Schedule
conflicts with the body of this Agreement, the Schedule controls
with respect to its subject matter."
```

Resolved conflicts:

| Conflict | Documents | Resolved outcome under Section 3.2 |
|---|---|---|
| Venue | Section 32 (New Castle County, Delaware) v. Order Form Additional Term 3 (Travis County, Texas) | Order Form controls: Texas venue, Delaware law. See PB-12. |
| Fee fixity | Section 16.1 ("fixed for the Initial Term") v. Order Form Section 6 (annual Anniversary Adjustment) | Order Form controls: overage and services rates move annually, including during the Initial Term. See PB-6. |
| Security indemnity | Section 23.2 v. Schedule A Section A-9 ("[n]otwithstanding anything to the contrary ... including Sections 11 and 23") | Schedule controls its subject matter, and A-9 says so expressly: the carve-back overrides the body indemnity. See PB-2. |
| Amendment | Section 33.2 (signed writing) v. Schedule B Section B-7 (amendment by posting) | Section 33.2's own exception ("[e]xcept as expressly provided in this Agreement") activates B-7: the posting right is effective. See PB-10. |

### 3.2 Recomputation (RR-4)

All arithmetic assumes the 6% floor binds. The formula's topside
(CPI-W change plus 2%) is uncapped, so every figure below is a
minimum.

| Item | Now | Month 12 | Month 24 | Month 36 | Year 10 |
|---|---|---|---|---|---|
| Overage Rate (per TB) | $1,150.00 | $1,219.00 | $1,292.14 | $1,369.67 | $1,942.90 |
| Professional Services rate (per hour) | $210.00 | $222.60 | $235.96 | $250.11 | $354.79 |
| Subscription Fee (per Facility per year) | $62,400.00 | fixed | fixed | $66,144.00 | $78,778.56 |

Subscription Fees adjust at each 24 month renewal (months 36, 60, 84,
108: four adjustments inside a ten year horizon, compounding to a
26.2% minimum increase). The Overage and Professional Services rates
adjust every anniversary (nine adjustments in ten years, compounding
to a 68.9% minimum increase), including at months 12 and 24, inside
the Initial Term that Section 16.1 describes as fixed.

Notice window arithmetic: the Initial Term ends August 31, 2029.
Under Section 18.2, a non-renewal notice is effective only if
delivered no less than 180 days before term end (on or before March
4, 2029) and no more than 270 days before term end (on or after
December 4, 2028). The only valid notice window for the Initial Term
is December 4, 2028 through March 4, 2029, a 90 day slot, recurring
once per 24 month Renewal Term thereafter.

### 3.3 Cap and remedy walk

Tracing the vendor's two indemnities and the SLA remedy through every
limitation that touches them:

1. Section 23.1 (IP indemnity) runs through Section 26.4, which does
   not except it from the caps: recovery capped at 12 months of Fees
   (Section 26.2).
2. Section 23.2 (Security Incident indemnity) first runs through
   Schedule A Section A-9, which removes it "to the extent arising
   from or contributed to by" four categories including all
   Customer-transmitted data (see PB-2: this is the operative
   defeat). If any claim survives A-9, Section 26.4 does not except
   Section 23 from the caps, so recovery is capped by Section 26.3's
   Enhanced Cap:

```
Contract, Section 26.3: "Notwithstanding Section 26.2, Provider's
aggregate liability for all claims arising from a Security Incident
will not exceed two (2) times the amount stated in Section 26.2 (the
'Enhanced Cap')."
```

   At current fees the Enhanced Cap is approximately $374,400 plus
   two times any overage and services fees paid in the trailing 12
   months.
3. By contrast, Section 26.4(b) lifts "a party's indemnification
   obligations under Section 24" out of both caps. Section 24 is the
   Customer indemnity. No section number in 26.4 reaches the
   vendor's Section 23 obligations. The customer side is uncapped,
   the vendor side is capped. See PB-1.
4. Schedule B credits are the sole remedy for availability failures
   (Section 13; Schedule B Section B-6), and the maximum monthly
   credit is 20% of one month's prorated Subscription Fees: $1,040
   per Facility, $3,120 across the three subscribed Facilities.

### 3.4 Exit walk

Every path out of the contract, as drafted:

| Exit | Where | Earliest availability | Cost or condition |
|---|---|---|---|
| Non-renewal | Section 18.2 | Effective August 31, 2029, notice only December 4, 2028 through March 4, 2029 | Miss the 90 day slot and the term extends 24 months |
| Termination for cause | Section 19.1 | On vendor material breach plus 30 day cure | Requires proof of material breach; prepaid fees refunded (Section 19.4) |
| Insolvency | Section 19.2 | On a listed insolvency event | Rare in practice |
| Convenience | absent | never | none exists |
| Chronic SLA failure | absent | never | credits are sole remedy (B-6) |
| Vendor change of control | absent | never | data and licenses transfer automatically (Section 29) |

The only unilateral exit is the 90 day notice slot once every two
years. Schedule B Section B-7 routes even a materially degraded SLA
into that same slot. This result feeds PB-5, PB-7, and PB-10.

### 3.5 Survival walk

Section 20.4 survives, among others, Section 8.2 (the perpetual
Aggregated Data license) and Section 20.3(c) (vendor retention of
Aggregated Data after termination). The data license outlives the
contract, the deletion obligation, and the confidentiality clause
(Section 27.6). This result feeds PB-3.

---

## Findings by family

### PB-1. Limitation of liability: DEVIATES, HIGH. GATE G1.

Playbook line:

```
Playbook, PB-1 ESCALATE: "Any exclusion list that operates
asymmetrically, including by excluding only the customer-side
indemnity from the caps."
```

Contract:

```
Contract, Section 26.4: "Sections 26.2 and 26.3 do not apply to (a)
Customer's obligation to pay Fees; (b) a party's indemnification
obligations under Section 24; (c) a party's breach of Section 5.3;
or (d) a party's gross negligence or willful misconduct."
```

```
Contract, Section 26.1: "IN NO EVENT WILL EITHER PARTY BE LIABLE FOR
ANY INDIRECT, INCIDENTAL, SPECIAL, CONSEQUENTIAL, EXEMPLARY, OR
PUNITIVE DAMAGES ... HOWEVER CAUSED AND UNDER ANY THEORY OF
LIABILITY, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGES."
```

Analysis. The caps read mutual and the exclusion list is drafted in
mutual voice, but the only indemnity excluded from the caps is
Section 24, the Customer indemnity, and the only conduct excluded is
Customer conduct (payment, Section 5.3 use restrictions). Resolving
the cross-references, every exclusion runs against Customer and none
runs against the vendor. The playbook's asymmetry trigger is met and
the item is gated. Section 26.1 is a mutual waiver of consequential
damages in customary form. Partial mitigation noted: Section 26.3
provides an Enhanced Cap of two times twelve months of fees for
Security Incident claims (quoted in Section 3.3 above), which
preserves a doubled recovery for the incident scenario, so the family
grades HIGH rather than CRITICAL pending the gate ruling.

Proposed redline. Rewrite 26.4(b) to except "a party's
indemnification obligations under Sections 23 and 24," delete
26.4(c) or pair it with a vendor-side conduct exclusion, and add the
playbook's direct-damages sentence to Section 26.1: "Damages arising
from a Security Incident, including costs of legally required
notification, call center support, credit monitoring, forensic
investigation, and regulatory fines or penalties passed through to
Customer, are direct damages recoverable subject to Section 26.3."

**GATE G1** to Associate General Counsel, Commercial, with the Chief
Financial Officer. Question: is the company prepared to sign any cap
structure in which its own indemnity is uncapped while the vendor's
is capped, and if not, what symmetric structure is the floor?
PROPOSED: hold for full symmetry per the redline.

### PB-2. Indemnification: DEVIATES, CRITICAL. GATE G2.

Playbook line:

```
Playbook, PB-2 ESCALATE: "[A]ny carve-back, condition, allocation
matrix, or 'shared responsibility' language, in any document of the
stack, that reduces or hollows the security indemnity."
```

Contract. The body indemnity is close to standard:

```
Contract, Section 23.2: "Provider will defend Customer Indemnitees
against third party claims, and indemnify them against damages,
regulatory fines and penalties, and reasonable costs of legally
required notifications, arising from a Security Incident caused by
Provider's breach of Section 10 or Schedule A, and will reimburse
Customer's reasonable out-of-pocket costs of responding to such an
incident."
```

The security schedule then removes it:

```
Contract, Schedule A, Section A-9: "The security of the Services is
a shared responsibility. Notwithstanding anything to the contrary in
this Agreement, including Sections 11 and 23 of the
Agreement, Provider has no responsibility or liability for, and no
obligation to indemnify, defend, or hold harmless any Customer
Indemnitee against, any Security Incident to the extent arising from
or contributed to by (a) any act or omission of Customer, a Customer
Affiliate, or any User, including management of User credentials;
(b) Customer's configuration of the Platform or of any integration,
report, or export; (c) Customer Systems or any network, device, or
software not managed by Provider; or (d) Customer Data as
transmitted to the Platform by or on behalf of Customer. For
purposes of this Section A-9, a Security Incident 'arises from' an
item if the item is a cause in fact of the incident in any degree."
```

Analysis. Clause (d) covers all Customer Data, because all Customer
Data is transmitted to the Platform by or on behalf of Customer.
Clause (a) covers credential compromise, the most common intrusion
path, regardless of fault. The final sentence sets the causation
standard at cause in fact "in any degree," so any contribution,
however small, defeats the indemnity "to the extent" of it, and in
the categories listed the extent will be argued as total. Section
23.2 survives on paper and covers almost nothing in practice. This
is the exact structure the playbook's escalation line names, located
in the ninth section of an otherwise standard technical schedule.
Sections A-1 through A-8 conform to PB-4's program content at
standard or fallback. Section 24 (Customer indemnity) also exceeds
the playbook's scope line ("our data, our misuse, and our systems")
by reaching any claim "arising from ... Customer Data as provided",
without a knowledge or breach qualifier. Graded HIGH within this
family. Section 25 procedures conform, including the settlement
consent and prejudice qualifiers.

Proposed redline. Delete A-9 and replace with: "Provider's
indemnification obligation under Section 23.2 is reduced only to the
extent a Security Incident results solely from Customer's breach of
its obligations under Sections 2.2, 5, or 6 of the Agreement."
Qualify Section 24(a) to Customer Data "as provided in breach of
Section 5.1(c) or in violation of third party rights known to
Customer."

**GATE G2** to Associate General Counsel, Commercial. Question: with
A-9 hollowing the breach indemnity, is the deal signable on any terms
while any version of A-9 survives? PROPOSED: no. A-9 deletion is a
walk-away condition.

### PB-3. Data ownership and use: DEVIATES, CRITICAL. GATE G3.

Playbook line:

```
Playbook, PB-3 ESCALATE: "[A]ny perpetual or irrevocable license to
company data. Any right to commercialize company data in
'aggregated,' 'de-identified,' 'anonymized,' or any other renamed
form. Any survival of data rights past termination."
```

Contract:

```
Contract, Section 8.2: "Customer further grants Provider a
non-exclusive, worldwide, royalty-free, perpetual, irrevocable
license to use, reproduce, modify, and create derivative works of
Customer Data to develop, test, train, benchmark, and improve
Provider's products and services, and to create, use, market, and
commercialize Aggregated Data, including by combining Aggregated
Data with the data of other customers in industry benchmarking
products."
```

```
Contract, Section 1.2: "'Aggregated Data' means Customer Data that
has been combined with other data or modified so that the result
does not identify Customer or any User as its source."
```

```
Contract, Section 20.3: "After the export window, Provider will
delete Customer Data within sixty (60) days, except ... (c)
Aggregated Data, which Provider may retain and continue to use under
Section 8.2."
```

```
Contract, Section 27.6: "Nothing in this Section 27 limits
Provider's exercise of the licenses granted in Section 8."
```

Analysis. All three escalation triggers are met by the same
mechanism. The definition of Aggregated Data requires non-attribution
only: it does not require removal of content. Cycle times, scrap
rates, first pass yield, supplier pricing, and cost structures are
Customer's confidential information whether or not Customer is named
as the source, and Section 8.2 licenses the vendor to sell them to
the market, expressly including in benchmarking products sold to
other manufacturers. Section 20.3(c) carries the right past
termination and past the deletion obligation, and Section 27.6
subordinates the entire confidentiality section to it. Ownership
language in Section 7.1 is correct and is beside the point: the
license, not the title, moves the value. Sections 7.2 (outputs are
Customer Data) and 6.2 (free export) conform to PB-3 and PB-9 and
are noted as conforming elements.

Proposed redline. Delete the perpetual and irrevocable grant in 8.2;
limit any aggregation to a separate written opt-in per PB-3 FALLBACK
that lists fields, requires content-level de-identification
("removal of content that reveals Customer's processes or costs, not
merely removal of Customer's name"), and is revocable. Delete
20.3(c) and 27.6.

**GATE G3** to the General Counsel, personally. Question: whether any
participation in vendor benchmarking is ever on the table for
production data, and if so on what opt-in terms. PROPOSED: no
benchmarking participation, service-only license.

### PB-4. Security and breach notice: DEVIATES, HIGH. GATE G4.

Playbook line:

```
Playbook, PB-4 ESCALATE: "[T]he notice clock runs from confirmation,
validation, or completed investigation rather than awareness, or
notice is conditioned or qualified."
```

Contract:

```
Contract, Section 11.1: "Provider will notify Customer without undue
delay, and in any event within seventy-two (72) hours, after
Provider confirms that a Security Incident has occurred."
```

Analysis. The 72 hour figure sits at the playbook fallback, but the
clock does not start at awareness. It starts when the vendor
"confirms," a word the contract does not define and the vendor
controls. The Section 1.15 definition of Security Incident includes
"reasonably suspected" events, but the notice clause never reaches
suspected events, because an incident that is suspected is by
definition not yet confirmed. Customer's own notification duties run
from its awareness, which cannot begin before the vendor's notice
arrives. The playbook escalates exactly this structure. Sections A-1
through A-8 of Schedule A otherwise meet the program content at
standard (encryption, access control, SOC 2 Type II, penetration
testing) and are conforming elements. Section 10's
non-diminishment sentence conforms, but see PB-10 for the posting
mechanism that can rewrite Schedule B, and note that no equivalent
posting right reaches Schedule A.

Proposed redline. Replace the quoted clause with: "Provider will
notify Customer without undue delay, and in any event within
seventy-two (72) hours, after Provider becomes aware of an actual or
reasonably suspected Security Incident." Add: "Provider's
investigation, confirmation, or characterization of an incident does
not delay notice."

**GATE G4** to Associate General Counsel, Commercial, with the Chief
Information Security Officer. Question: is 72 hours from awareness
acceptable under the company's own downstream notification
obligations, or must this deal carry 48? PROPOSED: 72 from awareness
per fallback, given the data categories.

### PB-5. Term and auto-renewal: DEVIATES, HIGH. GATE G5.

Playbook line:

```
Playbook, PB-5 ESCALATE: "[A]ny renewal term longer than twelve (12)
months. Notice requirement longer than one hundred twenty (120)
days. Any provision that voids or penalizes early notice of
non-renewal."
```

Contract:

```
Contract, Section 18.2: "This Agreement renews automatically for
successive renewal terms of twenty-four (24) months each (each a
'Renewal Term') unless either party delivers written notice of
non-renewal not less than one hundred eighty (180) days before the
end of the then current term. A notice of non-renewal delivered more
than two hundred seventy (270) days before the end of the then
current term is of no force or effect."
```

Analysis. Three escalation triggers in one clause: a 24 month
renewal term, a 180 day notice requirement, and a sentence that
voids notice given early. The second sentence deserves the attention
the first will get: a customer that decides in year one to leave at
the end of year three cannot yet give effective notice, and a notice
sent with the annual renewal calendar in mind is void if sent one
day before December 4, 2028. Combined with the recomputation in
Section 3.2, the practical effect is a 90 day exit slot once every
two years against a compounding price curve. The 36 month Initial
Term itself is within the playbook standard and is a conforming
element.

Proposed redline. "Renewal terms of twelve (12) months. Either party
may decline renewal by written notice at least sixty (60) days
before the end of the then current term. Notice of non-renewal may
be given at any time." Delete the void-notice sentence.

**GATE G5** to the business owner (VP Operations) with Associate
General Counsel, Commercial. Question: does operations want this
platform on a term that renews in two year blocks with a 90 day exit
slot, and if not, what renewal length is the ceiling? PROPOSED: 12
month renewals, 60 day notice, no window.

### PB-6. Price escalation: DEVIATES, HIGH. GATE G6.

Playbook line:

```
Playbook, PB-6 ESCALATE: "[A]ny uncapped formula. Any floor above
five percent (5%). Any adjustment that operates during a term the
contract describes as fixed. Any escalator split across documents so
that different rate classes move on different clocks."
```

Contract, the split machine, three passages:

```
Contract, Section 16.1 and 16.2: "Subscription Fees are fixed for
the Initial Term." "Upon each renewal, Subscription Fees adjust as
set forth in the applicable Order Form. Rates for quantities or
services not included in the Subscription Fees are as set forth in
the applicable Order Form and adjust as set forth therein."
```

```
Contract, Order Form Section 5: "At the commencement of each Renewal
Term, each Subscription Fee then in effect increases by the greater
of (a) six percent (6%) and (b) the percentage change in the
Consumer Price Index for Urban Wage Earners and Clerical Workers
(CPI-W, U.S. city average, all items) over the most recently
published twelve (12) months, plus two percent (2%)."
```

```
Contract, Order Form Section 6: "On each anniversary of the
Effective Date, the Overage Rate and the Professional Services rate
then in effect increase by the percentage determined under the
Renewal Adjustment methodology in Section 5 of this Order Form,
applied as of that anniversary."
```

Analysis. All four escalation triggers are met. The formula has a 6%
floor and no ceiling (CPI-W plus 2% is uncapped). The body's "fixed
for the Initial Term" sentence is true only of the defined term
Subscription Fees, which Section 1.17 defines to exclude overage and
services rates, and the Order Form moves those rates every
anniversary, including months 12 and 24 of the "fixed" Initial Term
(Section 3.2 of this memo: $1,150 to $1,219.00 to $1,292.14). Two
rate classes move on two different clocks, in two different
documents, under one methodology whose floor compounds. At the 6%
floor the overage rate is up 68.9% by year ten while the
subscription is up 26.2%, and the topside is unbounded.

Proposed redline. Conform to PB-6 STANDARD: all rates fixed for the
Initial Term (amend the Order Form, not just the body); renewal
increases capped at the lower of 3% or CPI-W change; one formula,
one adjustment date, all rates together; delete Order Form Section 6.

**GATE G6** to the Chief Financial Officer. Question: what escalator
cap and structure is the company's ceiling for this platform, and is
any intra-term adjustment ever acceptable? PROPOSED: 3% or CPI cap
at renewal only, per standard.

### PB-7. Termination rights: DEVIATES, HIGH. GATE G7.

Playbook line:

```
Playbook, PB-7 ESCALATE: "[T]he deal as drafted leaves no exit
before end of term other than vendor breach."
```

Contract. Section 19 grants termination for cause (19.1) and
insolvency (19.2), and refund on Customer termination for cause
(19.4), each conforming. The deviation is what is absent, per RR-3:

- No termination for convenience anywhere in the stack (playbook
  expects it after year one, 60 days' notice, pro rata refund).
- No chronic SLA failure termination (see PB-10; credits are sole
  remedy under Schedule B Section B-6).
- No change of control termination (see PB-8).
- No transition assistance provision.

Analysis. With every listed absence confirmed against the stack, the
exit walk (Section 3.4) shows the only unilateral exit is the 90 day
non-renewal slot every 24 months. The playbook's fallback would
accept no convenience termination during the Initial Term only if
chronic failure and change of control exits existed. Neither exists.
The escalation trigger is met as drafted. Suspension (19.3) conforms
(notice and cure before suspension, security exception).

Proposed redline. Add convenience termination after month 12 on 60
days' notice with pro rata refund; add chronic failure termination
(three consecutive months, or four in any twelve, below the
Availability Commitment) with pro rata refund; add change of control
termination per PB-8; add 90 day transition assistance at
then-current rates.

**GATE G7** to Associate General Counsel, Commercial. Question:
which of the three missing exits are non-negotiable for a deal of
this size? PROPOSED: chronic failure and change of control exits
non-negotiable, convenience exit tradeable against price.

### PB-8. Assignment and change of control: DEVIATES, CRITICAL. GATE G8.

Playbook line:

```
Playbook, PB-8 ESCALATE: "[A]ny automatic transfer of company data,
or of any license to company data, to an assignee or successor. Any
vendor change of control without a customer termination right."
```

Contract:

```
Contract, Section 29: "... except that either party may assign this
Agreement in its entirety, without consent, to (a) an Affiliate or
(b) a successor in interest in connection with a merger,
consolidation, reorganization, or sale of all or substantially all
of the assets or equity to which this Agreement relates, provided
the successor agrees in writing to be bound by this Agreement. Upon
an assignment by Provider under this Section, all rights and
licenses granted to Provider under this Agreement, including under
Section 8, and all Customer Data then in Provider's possession or
control, transfer to and vest in the assignee without further action
or notice."
```

Analysis. Both escalation triggers are met. The second sentence
transfers Customer Data and the Section 8 licenses, including the
Section 8.2 perpetual commercialization license, to any successor,
automatically and without notice. The successor exclusions the
playbook expects are absent: no competitor restriction, no notice of
closing, no Customer termination right on vendor change of control
(confirmed absent across the stack, per RR-3). Read with PB-3, an
acquirer of the vendor, including a Customer competitor or a data
broker, would take a perpetual license to exploit Customer's
production data in aggregated form. The first sentence's consent
requirement and void-assignment tail are standard and conforming.

Proposed redline. Delete the transfer sentence. Add: "Provider will
give Customer written notice within ten (10) days after a change of
control. Customer may terminate this Agreement on written notice
within sixty (60) days after such notice, with a pro rata refund of
prepaid fees. Customer Data and licenses to Customer Data transfer
to a successor only as necessary to continue providing the Services
to Customer under this Agreement."

**GATE G8** to the General Counsel, personally. Question: whether
any successor may ever take the data licenses automatically, and
whether a competitor restriction is required or the termination
right suffices. PROPOSED: termination right required, competitor
restriction pursued but tradeable per fallback.

### PB-9. IP license scope: DEVIATES, MEDIUM. No gate.

Playbook line:

```
Playbook, PB-9 STANDARD: "License rights not conditioned on payment
status; nonpayment is addressed by the suspension and termination
clauses, not by converting use into infringement."
```

Contract:

```
Contract, Section 2.4: "The rights granted in this Section 2 are
conditioned on Customer's timely payment of all Fees."
```

Analysis. Conforming elements first: Users include Affiliate
personnel (Section 1.22), outputs belong to Customer (Section 7.2),
export is free in standard formats during the term (Section 6.2) and
at exit (Section 20.2), and the grant covers the subscribed
Facilities for internal business purposes (Section 2.1). The
deviation is Section 2.4: a condition, not a covenant, so a payment
failure arguably terminates the license itself and converts use into
infringement, sidestepping the Section 19.3 suspension regime
(second notice plus ten days) and the Section 15.4 good faith
dispute right. The escalation trigger (automatic lapse on a payment
dispute) is not clearly met because Section 15.4 makes a disputed
withholding not a failure of "timely payment" on the better reading,
but the ambiguity is the vendor's drafting and should not be left to
a court. Not gated. Graded MEDIUM per the scale.

Proposed redline. Delete Section 2.4. Nonpayment remedies remain
Sections 15.3, 19.1, and 19.3.

### PB-10. SLA and remedies: DEVIATES, CRITICAL. GATE G9.

Playbook line:

```
Playbook, PB-10 ESCALATE: "[A]ny mechanism, anywhere in the stack,
by which the vendor can amend the service level schedule or any
other contract term unilaterally, including by posting revised
terms. Credits as sole remedy with no chronic failure exit."
```

Contract:

```
Contract, Schedule B, Section B-7: "Provider may update this
Schedule B from time to time to reflect changes in the Services by
posting a revised version to the Support Portal. A revised version
becomes effective thirty (30) days after posting. Customer's
continued use of the Platform after the effective date of a revised
version constitutes acceptance of the revision. If a revised version
materially degrades the Availability Commitment, Customer's
exclusive remedy is to deliver notice of non-renewal in accordance
with Section 18.2 of the Agreement."
```

```
Contract, Section 33.2: "Except as expressly provided in this
Agreement, no amendment of this Agreement is effective unless in a
writing that identifies itself as an amendment and is signed by an
authorized representative of each party."
```

Analysis. Both escalation triggers are met. The signed-writing
requirement in the boilerplate is real but self-defeating: its
opening clause is an exception for anything "expressly provided in
this Agreement," and B-7 expressly provides a posting mechanism for
the entire service level schedule, deemed accepted by continued use.
The tail of B-7 then prices the customer's recourse: if the vendor
degrades the SLA materially, the remedy is non-renewal under Section
18.2, which the exit walk (Section 3.4) shows is a 90 day slot once
every 24 months. A revision posted in month 4 of the Initial Term
could not even be answered with effective notice until December 4,
2028. Separately, credits are the sole remedy (Section 13; Schedule
B Section B-6) with no chronic failure termination anywhere in the
stack, the second escalation trigger. The 99.5% Availability
Commitment itself sits at the playbook fallback and would be
acceptable if the remedy structure were repaired. Credit tiers
(B-3) and the cash-out at exit (B-4) are conforming elements.

Proposed redline. Replace B-7 with: "This Schedule B may be amended
only by a written amendment signed by both parties." Delete the
exclusive-remedy tail. Amend B-6: "Credits are Customer's exclusive
remedy for Unavailability in any single month, except that Customer
may terminate for chronic failure (three consecutive months, or any
four months in a rolling twelve, below the Availability Commitment)
with a pro rata refund of prepaid fees."

**GATE G9** to Associate General Counsel, Commercial, with the
business owner. Question: is any unilateral update right acceptable
for operational content of Schedule B (maintenance windows, claim
mechanics) if the Availability Commitment and remedies are carved
out and frozen? PROPOSED: no posting right at all. Operational
changes ride the ordinary amendment process.

### PB-11. Insurance: DEVIATES, MEDIUM. No gate.

Playbook line:

```
Playbook, PB-11 STANDARD: "technology errors and omissions and cyber
liability of five million dollars ($5,000,000) per claim and
aggregate"
```

Contract:

```
Contract, Section 28: "(c) technology errors and omissions and cyber
liability insurance with combined limits of at least two million
dollars ($2,000,000) per claim and in the aggregate"
```

Analysis. CGL (1/2), umbrella (5), workers' compensation,
certificates on request, and 30 days' cancellation notice all
conform. The cyber tower is $2,000,000 against a $5,000,000 standard
and a $3,000,000 fallback, and the escalation floor ($2,000,000 or
any self-insurance representation) is not crossed. For a platform
holding production data from three facilities, and measured against
the Enhanced Cap arithmetic in Section 3.3 (a cap of roughly
$374,400 backed by a $2,000,000 tower), the limit is thin but the
exposure allocation problem lives in PB-1 and PB-2, not here. Graded
MEDIUM: negotiate to fallback or better.

Proposed redline. Raise (c) to $5,000,000, or $3,000,000 with the
umbrella endorsed to sit over the cyber and E&O tower. Add
"certificates furnished annually" in place of "on request."

### PB-12. Governing law and venue: DEVIATES, HIGH. GATE G10.

Playbook line:

```
Playbook, PB-12 ESCALATE: "Conflicting governing law or venue
provisions anywhere within the stack, whatever the order of
precedence resolves them to."
```

Contract, the body:

```
Contract, Section 32: "This Agreement is governed by the laws of the
State of Delaware without regard to its conflict of laws rules ...
Each party irrevocably submits to the exclusive jurisdiction of the
state and federal courts sitting in New Castle County, Delaware for
any action arising out of or relating to this Agreement, and waives
objection to venue in those courts."
```

Contract, the order form:

```
Contract, Order Form Section 7, Additional Term 2: "Any action or
proceeding arising out of or relating to this Order Form or the
Agreement shall be brought exclusively in the state or federal
courts sitting in Travis County, Texas, and each party consents to
the jurisdiction of those courts."
```

Analysis. Standing alone, Section 32 would grade CONFORMS at
fallback: Delaware law is on the playbook's accepted list, a
Delaware forum is the defendant vendor's chartered home, and the
jury waiver is acceptable. The order form breaks it. The Additional
Term claims exclusive Texas venue for actions relating to "this
Order Form or the Agreement," and under Section 3.2 (precedence
walk, Section 3.1 of this memo) the Order Form controls. The
resolved outcome is Delaware law administered by a Travis County,
Texas court, the vendor's home county, reached through a paragraph
formatted as commercial housekeeping. The playbook escalates any
conflicting dispute provisions in the stack regardless of how
precedence resolves them, because the conflict itself invites a
motion fight. The trigger is met.

Proposed redline. Strike the Additional Term. If the vendor wants
its home forum, it says so in Section 32 where the choice is visible,
and the playbook answer is Ohio at standard or a neutral or
defendant's forum at fallback, decided at the gate.

**GATE G10** to the General Counsel, personally. Question: which
forum package does the company accept for this deal (Ohio standard,
Delaware fallback, or vendor's home forum), with the requirement
that exactly one dispute clause survive in the stack? PROPOSED:
Delaware law, Delaware venue, single clause in Section 32, Additional
Term struck.

---

## Additional findings (outside the twelve families)

- **AF-1, Publicity (Section 30), LOW.** Vendor may use Customer's
  name and logo unless Customer opts out. Flip to prior written
  consent. Not gated.
- **AF-2, Data processing addendum (Section 12), LOW.** If personal
  data categories expand, the clause commits Customer to "Provider's
  standard data processing addendum" sight unseen. Replace with "a
  mutually agreed data processing addendum." Not gated.
- **AF-3, Analytics disclaimer (Sections 21.4 and 22), note.** The
  informational-outputs warranty and accuracy disclaimer are
  customary for analytics platforms and are not graded as
  deviations. Recorded so the absence of a finding is visible as a
  decision, not a gap.

## Human decision queue

| Gate | Family | Decision maker (per playbook) | Decision question |
|---|---|---|---|
| G1 | PB-1 | AGC Commercial + CFO | Floor structure for cap symmetry |
| G2 | PB-2 | AGC Commercial | Is any survival of A-9 signable |
| G3 | PB-3 | General Counsel | Any benchmarking participation, ever, on what opt-in |
| G4 | PB-4 | AGC Commercial + CISO | 48 or 72 hours from awareness |
| G5 | PB-5 | VP Operations + AGC Commercial | Renewal length ceiling |
| G6 | PB-6 | CFO | Escalator cap and structure ceiling |
| G7 | PB-7 | AGC Commercial | Which missing exits are non-negotiable |
| G8 | PB-8 | General Counsel | Successor data rights and competitor restriction |
| G9 | PB-10 | AGC Commercial + business owner | Any unilateral update right for operational SLA content |
| G10 | PB-12 | General Counsel | Forum package, single dispute clause |

Per Protocol CR-1, this review is not complete until each gate item
is ruled by the named decision maker. Every PROPOSED line above is a
proposal and nothing more.

## Coverage appendix (Stage 1 census)

56 of 56 provisions mapped. NO FAMILY entries carry a one line
reason.

| Provision | Family | Note |
|---|---|---|
| Body 1 (Definitions) | feeds all | definitions read per RR-5; 1.2, 1.17, 1.15 load-bearing in findings |
| Body 2 | PB-9 | grant, users, condition (2.4) |
| Body 3 | PB-12, PB-6 | precedence machinery (RR-6), applied in Section 3.1 |
| Body 4 | NO FAMILY | implementation scope; no playbook position implicated |
| Body 5 | PB-2, PB-1, PB-9 | customer duties feed Section 24 and 26.4(c) |
| Body 6 | PB-3, PB-9 | connectors, export |
| Body 7 | PB-3 | ownership, outputs |
| Body 8 | PB-3 | service license (8.1), aggregation license (8.2) |
| Body 9 | PB-3 | usage data, content excluded |
| Body 10 | PB-4 | program, non-diminishment |
| Body 11 | PB-4 | notice clock (11.1), cooperation, notification control |
| Body 12 | PB-4 | DPA condition (AF-2) |
| Body 13 | PB-10 | SLA incorporation, sole remedy pointer |
| Body 14 | NO FAMILY | support response times; conforms to no stated position, no deviation |
| Body 15 | PB-6 | invoicing, late interest, dispute rights (15.4) |
| Body 16 | PB-6 | fee fixity and adjustment pointers |
| Body 17 | NO FAMILY | taxes, standard allocation |
| Body 18 | PB-5 | initial term, renewal, notice window |
| Body 19 | PB-7 | cause, insolvency, suspension, refund |
| Body 20 | PB-3, PB-7 | export window, deletion, survival (20.3(c), 20.4) |
| Body 21 | NO FAMILY | warranties; 21.4 noted in AF-3 |
| Body 22 | NO FAMILY | disclaimers; AF-3 |
| Body 23 | PB-2 | IP and security indemnities |
| Body 24 | PB-2 | customer indemnity |
| Body 25 | PB-2 | procedures, conform |
| Body 26 | PB-1 | waiver, caps, exclusions |
| Body 27 | PB-3 | confidentiality; 27.6 subordination; otherwise standard |
| Body 28 | PB-11 | insurance |
| Body 29 | PB-8 | assignment, transfer sentence |
| Body 30 | NO FAMILY | publicity; AF-1 |
| Body 31 | NO FAMILY | notices, standard |
| Body 32 | PB-12 | law and venue |
| Body 33 | PB-10 | 33.2 amendment machinery; 33.1, 33.3 through 33.8 standard boilerplate |
| OF 1 | NO FAMILY | module list |
| OF 2 | NO FAMILY | facility list |
| OF 3 | PB-6 | rate table |
| OF 4 | PB-5 | initial term restate |
| OF 5 | PB-6 | renewal adjustment |
| OF 6 | PB-6 | anniversary adjustment |
| OF 7 | PB-12, PB-6 | additional terms: precedence restate, PO terms, venue |
| Sched A-1 | PB-4 | program |
| Sched A-2 | PB-4 | access control |
| Sched A-3 | PB-4 | encryption |
| Sched A-4 | PB-4 | SOC 2, pen testing |
| Sched A-5 | PB-4 | subprocessors, US data centers |
| Sched A-6 | PB-4 | incident response |
| Sched A-7 | PB-4 | continuity |
| Sched A-8 | PB-4 | personnel |
| Sched A-9 | PB-2 | carve-back; also feeds PB-1 cap walk |
| Sched B-1 | PB-10 | definitions |
| Sched B-2 | PB-10 | 99.5% commitment |
| Sched B-3 | PB-10 | credit tiers |
| Sched B-4 | PB-10 | claims, cash-out |
| Sched B-5 | PB-10 | exclusions |
| Sched B-6 | PB-10 | sole remedy |
| Sched B-7 | PB-10 | posting amendment |

*End of memo. Produced by the model under Protocol CR-1. Invented for
demonstration. No real company, person, or agreement is depicted.*
