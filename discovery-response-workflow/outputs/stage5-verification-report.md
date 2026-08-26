# Stage 5 Verification Report

**Whitfield v. Cumberland Ridge Logistics, LLC**
Circuit Court for Knox County, Tennessee, Docket No. 2-317-26
Plaintiff's First Set of Interrogatories and Requests for Production (served July 20, 2026; responses due August 31, 2026)

Date prepared: 2026-08-25
Stage 5 output per Protocol 05

Role note per protocol: this pass grades the drafts cold, as their adversary. Findings are ordered by severity: privilege leaks, record conflicts, citation FAILs, scope excesses, completeness gaps, style. Every finding carries a receipt. A separate section grades the naive baseline answer to Interrogatory No. 7. The closing section states what was checked, not only what was found.

Drafts verified:

- Protocol drafts: [stage4-response-shells.md](/Users/Jonathan/Desktop/Job_Search_2026/Demo_Discovery_Triage/outputs/stage4-response-shells.md)
- Naive baseline: [stage4-rog7-NAIVE-baseline.md](/Users/Jonathan/Desktop/Job_Search_2026/Demo_Discovery_Triage/outputs/stage4-rog7-NAIVE-baseline.md)

Record verified against: CRL-0001 through CRL-0023 in [materials/](/Users/Jonathan/Desktop/Job_Search_2026/Demo_Discovery_Triage/materials/), the [Stage 1 checklist](/Users/Jonathan/Desktop/Job_Search_2026/Demo_Discovery_Triage/outputs/stage1-intake-checklist.md), the [Stage 2 triage table](/Users/Jonathan/Desktop/Job_Search_2026/Demo_Discovery_Triage/outputs/stage2-triage-table.md), and the [Stage 3 privilege gate](/Users/Jonathan/Desktop/Job_Search_2026/Demo_Discovery_Triage/outputs/stage3-privilege-gate.md). TRAP-KEY.md was not opened.

---

# PART ONE: THE PROTOCOL DRAFTS (stage4-response-shells.md)

## 1. Privilege leak check (reported first per protocol)

Search targets: any content derived from (a) the withheld CRL-0008 thread, (b) the redacted final sentence of CRL-0010 entry 2026-05-27, (c) the four human review queue items (CRL-0010 entries 2026-03-18 and 2026-05-08; CRL-0011 in full; the CRL-0013 internal routing note).

**Finding P1 (qualified hit, ruled posture, counsel must confirm): the ROG No. 3 answer draws on routed queue item 1.** The answer's item 4 states that General Counsel Aldana "was consulted" and cites the routed entry:

```
Draft, ROG No. 3 answer, item 4: "Gregory Aldana, General Counsel
[CRL-0015, roster line]: was consulted [CRL-0010, entry 2026-03-18,
cited for the fact and date of consultation only]."

CRL-0010, entry 2026-03-18: "Consulted GA re restructuring proposal
and related personnel risk. See separate privileged correspondence,
not filed here."
```

The entry is human review queue item 1; its production form is undecided. Protocol 05 makes any use of routed material a hit reported at the top. Mitigation, stated for completeness: the draft uses only the fact and date of the consultation, not the subject phrase the gate flagged; it discloses its own dependence in a bracketed note ("the entry's production form remains pending counsel's determination"); and the Stage 3 gate itself observed that the bare fact of consultation "is ordinarily discoverable and belong[s] on a privilege log." The answer cannot be verified until counsel's queue item 1 determination lands and confirms the fact and date are answerable. Note also that placing the consultation inside the ROG No. 3 answer necessarily discloses that the consultation concerned the termination decision; counsel should confirm that framing is intended.

**Finding P2 (low): a citation range in ROG No. 12 sweeps routed and redacted entries.** The Paulk knowledge description cites "[CRL-0010, entries 2026-02-03 through 2026-05-27]", a range that includes routed entries 2026-03-18 and 2026-05-08 and the partially redacted 2026-05-27 entry. No content from the routed entries or the redacted sentence appears in the description (it says only "knowledge of the handling of HR complaint 26-004, the restructuring review, and the separation process"), so no substance leaked; the citation range should be trimmed or the current handling confirmed as intentional.

**No other hit.** Verified specifically: no draft sentence restates any part of the CRL-0008 advice; the shells' selection criteria language traces to CRL-0009 (Proposal section), CRL-0010 (entry 2026-03-30), and CRL-0012 (body paragraph 3), all independent of the privileged thread. The redacted "GA advised" sentence of entry 2026-05-27 appears nowhere. CRL-0011 (queue item 3) is not drawn on; ROG No. 3's note says so and the claim verifies (the April 20 coordinator date in ROG No. 2 has the independent source CRL-0016, change note). The CRL-0013 routing note ("reviewed by G. Aldana prior to transmittal") appears nowhere.

**Cross reference: the naive baseline contains an outright privilege FAIL (disclosure of the substance of the CRL-0008 advice). Detail in Part Two, finding B1.**

## 2. Record conflicts

**Finding R1 (HIGH, NOT flagged by the drafts): the record contradicts the sworn ROG No. 6 statement of when the restructuring was proposed.** The answer swears the proposal originated with the March 25, 2026 memorandum:

```
Draft, ROG No. 6 answer: "Who first proposed it and when: Lena
Ostrander, Chief Financial Officer, proposed the consolidation ...
by internal memorandum dated March 25, 2026 [CRL-0009, header and
opening paragraph]."
```

Two documents place the proposal, and the March 30 review meeting, in existence a week before that memo's date:

```
CRL-0008, Paulk to Aldana, sent Wednesday, March 18, 2026, 4:51 PM:
"You have seen Lena's restructuring memo proposing to consolidate
the two operations manager positions."

CRL-0010, entry 2026-03-18: "Consulted GA re restructuring proposal
and related personnel risk."

CRL-0009, header: "Date: March 25, 2026"; Next step section:
"I propose we meet on March 30 with HR to review this analysis."
```

Compounding it: the March 19, 2026 reply in CRL-0008 refers to "the March 30 review" by date, six days before CRL-0009 proposes that meeting date. (The reply's advice content is not restated here; the meeting date reference is cited by location only.) So either an earlier version of the restructuring memo circulated before March 18, or the March 25 date on CRL-0009 is wrong, or the CRL-0008 and CRL-0010 dates are wrong. Any of those is counsel's problem to resolve before a sworn answer says the proposal was made March 25; opposing counsel finding it first would argue the restructuring was in motion before the memo that supposedly initiated it, and the ROG No. 6 subpart "when it was proposed" is sworn on exactly this fact. Both conflicting citations stand regardless of which the draft used, per protocol. The drafts flag the March 26 decision conflict (R2 below) but not this one. Handling note: the receipts here live partly in a withheld privileged document; resolution must not quote privileged content into any served paper.

> **ADDENDUM, 2026-08-25 (demo author disposition): R1 RESOLVED BY SOURCE CORRECTION.** This finding was a genuine authoring defect in the invented corpus, not a planted trap: the case author dated the privileged thread March 18 to 19 while having it reference a memo dated March 25 and a meeting date that memo had not yet proposed. The materials QA pass had verified every date string against the master timeline but did not check narrative causality across documents; this verification pass caught it blind. Correction applied to CRL-0008 only: the March 18 message now references Lena's proposal as heard and "to be put in writing this week," and the March 19 reply now references "the restructuring review Lena intends to convene" without a date. The oral proposal preceding the written memo is coherent with CRL-0010's March 18 entry ("Consulted GA re restructuring proposal"). The two Stage 2 citations quoting the corrected passages were refreshed the same day and are so marked. The quotes preserved in this finding above are the PRE-correction text, kept as the verification record. After the correction, R2 is again the corpus's only record conflict, as designed.

**Finding R2 (flagged by the drafts; reported anyway per protocol): the record conflicts on when the decision to eliminate Plaintiff's position was made.**

```
CRL-0010, entry 2026-03-26: "DK confirmed today the Whitfield
position will be eliminated; begin severance paperwork."

CRL-0012, body paragraph 3: "The decision to eliminate the position
was reached following the restructuring review conducted on
March 30, 2026."

CRL-0010, entry 2026-03-30: "Consolidation of the two operations
manager roles approved."
```

March 26 precedes March 30 by four days. The draft handles this correctly: the ROG No. 6 note states the conflict with both citations, states no sworn date for the position elimination decision itself, and bars verification until counsel resolves it. Reported here because Protocol 05 requires every record conflict reported with both citations regardless of the draft's handling. Note R1 and R2 compound: the record now shows movement on eliminating Plaintiff's position both before the review meeting (March 26) and before the proposal memo's own date (March 18 references).

**No further conflict found.** Affirmatively cross checked and consistent: the January 8 email date across CRL-0002, CRL-0003, CRL-0004, CRL-0010, CRL-0019; the January 12 and 13 emails across CRL-0002, CRL-0003, CRL-0004, CRL-0010; the February 3 complaint and February 4 acknowledgment across CRL-0004, CRL-0005, CRL-0008, CRL-0010; hire date March 11, 2019 across CRL-0006, CRL-0014, CRL-0015 (and the February 25, 2019 offer letter accepted March 1, 2019 in CRL-0014 item 1 is consistent with it); the review dates and ratings across CRL-0006, CRL-0007, CRL-0014, CRL-0016; the April 6 meeting (2:00 pm, conference room B) across CRL-0010, CRL-0011, CRL-0012, CRL-0017; the April 17 effective date across CRL-0010, CRL-0012, CRL-0013, CRL-0014, CRL-0016, CRL-0017; the April 20 coordinator date across CRL-0011 and CRL-0016; the May 8 severance transmittal across CRL-0010, CRL-0013, CRL-0014; the May 29 lapse date (May 8 plus 21 days, recomputed); the severance amount (8 weeks of the 108,000 dollar salary in CRL-0014 item 4 equals 16,615.38 dollars as stated in CRL-0013, recomputed); the headcount step from 84 (CRL-0015) to 83 (CRL-0016); "seven years of service" in CRL-0012 against the 2019 hire date; and all eleven day of week statements in the record (recomputed against the 2026 calendar, all correct).

## 3. Citation audit

All 111 bracketed citations in the shells were reopened and graded against the cited passages. Result: **109 MATCH, 2 STRETCH, 0 FAIL.** The two STRETCH grades, with receipts, then the MATCH log in compressed form.

**Finding C1 (STRETCH, two citations, ROG No. 2): a January 2026 snapshot chart is cited for personnel claims covering January 1, 2025 forward.** Both sentences assert who held positions "during that period," meaning January 1, 2025 through April 16, 2026:

```
Draft: "During that period the VP of Operations was Dale Kestner;
the Operations Manager, East was Marlene Whitfield; and the
Operations Manager, West was Marcus Teal [CRL-0015, chart lines]."

Draft: "The Dispatch Supervisor (Cody Brantley) and the Safety and
Compliance Manager (Dana Hollis) also reported within the operations
department under the VP of Operations [CRL-0015, chart lines]."

CRL-0015, title block: "ORGANIZATION CHART, JANUARY 2026 /
Prepared by HR, January 5, 2026"
```

The chart evidences one date, January 5, 2026. The full period claim is a reasonable inference (CRL-0009 Background says the two manager structure ran "[s]ince the 2023 reorganization"; CRL-0006 shows Kestner as VP in November 2025 and Whitfield hired into the East role in 2019), but nothing cited establishes that these specific individuals held these positions for all of 2025. Grade STRETCH; fix by having the client confirm no operations personnel changes between January 1, 2025 and January 5, 2026, or by adding the supporting citations to the sentence.

**MATCH log.** Each remaining citation was reopened and the cited passage compared to the assertion; all support the assertion as written. Compressed by answer, with the load bearing passage quoted where the assertion is factual rather than enumerative:

- ROG No. 1 (8 citations, all MATCH): signature blocks of CRL-0005, CRL-0003, CRL-0009 carry the stated names and titles; custodian fields of CRL-0004 ("Renee Paulk (HR complaint file)"), CRL-0010, CRL-0014 header ("Index last updated: May 8, 2026 by R. Paulk"), CRL-0002, CRL-0006 header block, CRL-0009 custodian field, CRL-0015 chart line ("Safety and Compliance Manager: Dana Hollis"), CRL-0010 entry 2026-02-19 ("D. Hollis (Safety) reports") all say what they are cited for.
- ROG No. 2 (4 of 6 citations MATCH; 2 STRETCH per C1): CRL-0009 Background ("Since the 2023 reorganization we have run operations under two regional managers, East and West, each reporting to the VP of Operations"); CRL-0016 chart line and change note ("Effective April 17, 2026 the Operations Manager, East position (M. Whitfield) was eliminated ... Lead coordinators absorbed routine regional scheduling effective April 20, 2026"); the two holder list citations (CRL-0015 chart line with CRL-0016 change note; CRL-0015 chart line with CRL-0016 chart line).
- ROG No. 3 (8 citations, all MATCH): CRL-0009 opening paragraph ("This memo summarizes the financial case for consolidating our two regional operations manager positions") and Financial case section; CRL-0010 entry 2026-03-30 ("Attended restructuring review meeting with LO and DK. Consolidation of the two operations manager roles approved.") cited three times; CRL-0012 header and signature with CRL-0010 entry 2026-04-06 ("DK delivered memo"); CRL-0017 body paragraph 2 ("I will cover final pay, benefits, and COBRA and hand her the packet") with CRL-0010 entry 2026-04-06 ("I covered benefits, COBRA, final pay"); CRL-0015 roster line ("General Counsel: Gregory Aldana"); CRL-0010 entry 2026-03-18 (content supports the fact and date of consultation; see finding P1 for the privilege posture).
- ROG No. 4 (7 citations, all MATCH): CRL-0014 items 7, 8, 9, 10, 11 state the five review dates and ratings exactly as listed; CRL-0006 and CRL-0007 header blocks state "Reviewer: Dale Kestner, VP of Operations" and the two 2025 to 2026 ratings; CRL-0014 contents list shows no counseling or disciplinary item; CRL-0014 items 7 through 9 indeed list date and rating only, as the counsel note says.
- ROG No. 5 (8 citations, all MATCH): CRL-0002 body paragraph 1 ("dispatch has been leaning on drivers to hit delivery windows that do not work within their available hours"; "I saw the January 8 email"); CRL-0003 body paragraphs 2 and 4 ("I have looked at the January 8 exchange and I read it as Cody trying to keep a customer commitment on a tight day, not as an instruction to run over hours or touch a log"; "bring me the details and we will run it down through Safety the way the policy says"; "I do not think a sit down with Safety is necessary at this point"); CRL-0004 header and body with CRL-0010 entry 2026-02-03 ("Logged as complaint 26-004"); CRL-0005 body paragraphs 1 and 3 with CRL-0010 entry 2026-02-04; CRL-0010 entries 2026-02-09, 2026-02-13 ("Met with C. Brantley with his supervisor present ... Asked Safety to pull ELD records for the Mabry run"), 2026-02-19 ("delivery completed 22 minutes inside the 14 hour window, no edits to duty status after the fact ... exception report shows numbers consistent with prior quarters"), 2026-02-24 ("Memo to file closing initial review ... No confirmed HOS violation ... Recommended dispatch refresher training ... Called MW and summarized outcome").
- ROG No. 6 (6 citations, all MATCH as citations; see R1 for the record level conflict on the proposal date and R2 for the flagged decision date conflict): CRL-0009 header and opening paragraph; CRL-0009 Background and Financial case sections ("approximately 128,000 dollars annually"; "Q1 revenue is tracking 6 percent under plan"; "Combined tractor count is flat year over year"); CRL-0012 body paragraphs 2 and 3; CRL-0016 change note; CRL-0010 entries 2026-03-30 and 2026-03-26 (the note's quotations are verbatim).
- ROG No. 7 (1 citation, MATCH): CRL-0012 body paragraph 2 ("the company is consolidating its two regional operations manager positions into a single company wide operations manager role. As a result, your position, Operations Manager, East, is being eliminated.").
- ROG No. 8 (9 citations, all MATCH): CRL-0006 header block and CRL-0014 header ("Hire date: March 11, 2019"); CRL-0007 header block and CRL-0014 item 11; CRL-0015 chart line ("Marcus Teal (hired 2021)"); CRL-0016 chart line ("most recent review February 2026, rating 4 of 5"); CRL-0009 Proposal section ("That selection, if the consolidation is approved, should be made on documented, objective criteria at the review meeting."); CRL-0010 entry 2026-03-30; CRL-0012 body paragraph 3 ("based on objective factors including comparative regional consolidation requirements and recent performance assessments"); the two note citations including the verbatim "I hold the meeting record in the restructuring file."
- ROG No. 9 (8 citations, all MATCH): CRL-0002 and CRL-0004 bodies; CRL-0003 body paragraph 2; CRL-0019 header and body with CRL-0010 entry 2026-02-13; CRL-0019 header and body; CRL-0010 entry 2026-02-19 with CRL-0015 chart line; CRL-0010 entries 2026-02-03 through 2026-02-24; the note citations for "Trina" (CRL-0019 body paragraph 2: "when Trina is back at the desk") and the two unnamed drivers (CRL-0002 body paragraph 1: "Two other drivers have mentioned similar pressure to me since Thanksgiving").
- ROGs Nos. 10 and 11 (0 citations): placeholders only; nothing to audit, and correctly so, since the collected set contains no source (Stage 2 method note 4 confirmed).
- ROG No. 12 (8 citations, all MATCH): each knowledge description is supported by the cited bodies, header blocks, chart lines, and entries; CRL-0012 receipt acknowledgment line exists ("Receipt acknowledged: Marlene Whitfield (signed, April 6, 2026, acknowledgment of receipt only)"). The 2026-02-03 through 2026-05-27 range carries the privilege note at P2.
- RFP responses Nos. 1 through 10 (42 citations, all MATCH): the production lists were checked document by document (see completeness); the specific passage citations verify, including CRL-0018 title block ("EMPLOYEE HANDBOOK, SECTION 9 (EXCERPT)" / "Effective June 1, 2024"), CRL-0013 header and status line ("Transmitted by mail May 8, 2026. Not signed. Not returned."), CRL-0012 body paragraph 4 ("The company anticipates presenting you with a separation agreement, including a severance offer, under separate cover."), CRL-0014 item 15 and final note ("HR complaint file 26-004 is maintained separately in the HR complaint system per policy and is not part of the personnel file."), CRL-0009 Next step section ("My office will circulate the supporting financial detail before the meeting."), CRL-0007 linkage via CRL-0012 body paragraph 3, and the CRL-0010 entry ranges named in each production statement.

## 4. Scope audit

Each of the 22 responses was audited against the question scope restated from the Stage 1 checklist. Two excesses found, both graded FLAG FOR COUNSEL, none graded REMOVE.

**Finding S1 (FLAG FOR COUNSEL, ROG No. 2):** checklist scope is the operations department structure from January 1, 2025 to the present plus the operations manager holders; the checklist warns a careless answer "would describe company-wide structure or reach back before 2025." The draft's first sentence reaches back: "the operations department ran under a structure in place since the Company's 2023 reorganization." One clause, provenance context rather than substance, and arguably useful framing; counsel decides whether it stays.

**Finding S2 (FLAG FOR COUNSEL, ROG No. 3):** checklist scope is participants in, consultees on, and approvers of the termination decision, with roles in that decision; the checklist warns against narrating execution. Two role descriptions extend past the decision into execution: Kestner "communicated the decision to Plaintiff by memorandum and meeting on April 6, 2026" and Paulk "handled the separation logistics, including the separation packet and benefits items delivered at the April 6, 2026 meeting." Communication of a decision is arguably part of a role in it; separation logistics is execution. Trimming is counsel's call; disclosure risk is nil since the same facts are produced under RFPs Nos. 3 and 4.

All other answers stay inside their restated scope. Verified specifically: ROG No. 4 answers only the enumerated documented events after its stated objection; ROG No. 5 detail is inside the express "describe in detail every action" language; ROG No. 6 tracks its five subparts and nothing else; ROG No. 7 is one sentence stating the reason and nothing else; ROG No. 8 gives only the most recent rating for each manager, per the checklist's warning against producing more; ROG No. 9 lists six named persons with record based knowledge and routes the roster breadth problem through an objection; ROG No. 12 knowledge descriptions are brief, per the checklist's warning against witness statement detail; the RFP responses state production and objections without volunteering substance.

## 5. Completeness

**Every request has a response: 22 of 22.** Interrogatories Nos. 1 through 12 and Requests Nos. 1 through 10 each carry a response (three are placeholder responses with client supply notes: ROGs Nos. 10 and 11 and the derivative RFP No. 10, matching the Stage 2 collection gap note).

**Production accounting, checked document by document against the triage table.** Every responsive nonprivileged document is accounted for in at least one production statement: CRL-0002, CRL-0003, CRL-0004, CRL-0005 (RFPs Nos. 3 and 8); CRL-0006, CRL-0007 (RFPs Nos. 7 and 9); CRL-0009 (RFP No. 5); CRL-0010 (RFPs Nos. 3, 4, 5, 6, 8, with the redaction identified each time); CRL-0012 (RFPs Nos. 4, 5, 6, 9); CRL-0013 (RFPs Nos. 6 and 9); CRL-0014 (RFP No. 6 via item 15, and see F2); CRL-0016 (RFP No. 5); CRL-0017 (RFPs Nos. 3 and 4); CRL-0018 (RFPs Nos. 2 and 8); CRL-0019 (RFPs Nos. 3 and 8). CRL-0015 maps to interrogatories only, so no production statement is required. CRL-0011 is routed (queue item 3) and its contingent production is stated in the RFP Nos. 4 and 5 notes. CRL-0001 and the four noise documents (CRL-0020 through CRL-0023) map to nothing, correctly. The RFP No. 1 population was independently rebuilt from the interrogatory answers as drafted; the union of documents cited in the twelve answers is exactly the fourteen documents the response lists (CRL-0002 through CRL-0007, CRL-0009, CRL-0010, CRL-0012, CRL-0014 through CRL-0017, CRL-0019), no more and no fewer.

**Every withheld document has a log entry.** CRL-0008, withheld in full, is covered by privilege log entries 1 and 2 and is expressly identified as withheld in the responses to RFPs Nos. 4, 5, and 6. The single redaction (CRL-0010, entry 2026-05-27, final sentence) is covered by log entry 3 and is identified in every response producing CRL-0010. No other withholding exists to log.

**Finding F1 (completeness gap, FLAG FOR COUNSEL): the ROG No. 3 answer omits the March 26 Kestner confirmation that the triage table mapped to ROG No. 3.**

```
Triage table, CRL-0010, ROG No. 3 citation: entry 2026-03-26,
"DK confirmed today the Whitfield position will be eliminated;
begin severance paperwork."

Draft, ROG No. 3, item 2 (complete role description for Kestner):
"participated in the March 30, 2026 restructuring review [CRL-0010,
entry 2026-03-30] and communicated the decision to Plaintiff by
memorandum and meeting on April 6, 2026."
```

The record evidence that Kestner confirmed the elimination on March 26, four days before the review, appears only in the ROG No. 6 conflict note, not in the ROG No. 3 description of his role. If the conflict resolves toward the March 26 entry meaning what it says, Kestner's sworn role description is understated (he confirmed the elimination, not merely participated in the review). The omission should be an explicit counsel decision tied to the R2 resolution, not a silent drop. FLAG FOR COUNSEL.

**Finding F2 (completeness gap, minor): the production posture of CRL-0014 itself is not squarely stated.** The index is mapped responsive to RFP No. 6 and RFP No. 9. The RFP No. 6 response produces "the personnel file index entry recording the offer's transmittal and status [CRL-0014, item 15]," an entry rather than the document, and the RFP No. 9 response produces the file "as maintained, the contents of which are indexed at CRL-0014" without saying whether the index document itself produces. One clarifying clause fixes it.

**Open items restated by the drafts, verified as accurately stated (not new findings):** the four human review queue determinations; the client supplied content for ROGs Nos. 10 and 11 and RFP No. 10; the collection gaps (full handbook and policies for RFP No. 2; the March 30 meeting record and pre-meeting financial detail for RFP No. 5 and ROG No. 8; underlying ELD records, exception reports, and any audits for RFP No. 8; the 2022 through 2024 review documents and all comparator evaluations for RFP No. 7; personnel file items 1 through 9, 12, 14, and 16 for RFP No. 9; Teal's full hire date; administering persons for the 2022 through 2024 reviews; the Complaint and Answer for ROG No. 12; identification of "Trina" and the two unnamed drivers for ROG No. 9). Each is flagged in the draft where it bites, and each blocks final verification of its answer.

## 6. Style

**Finding ST1: internal boundary wobble in ROG No. 2.** The answer opens with the old structure running "[f]rom January 1, 2025 through April 16, 2026," then lists Whitfield as "Operations Manager, East, through April 17, 2026." Both are defensible readings of an April 17 effective date (CRL-0016 change note; CRL-0014 separation date April 17; CRL-0017 has her working through the effective date), but the same answer should pick one convention. One word fix.

**Dash scan of the drafts:** neither draft file contains an em dash or an en dash (character scan, receipt in the closing section).

Nothing else at style level. The shells' bracketed counsel notes are consistently labeled, the objection language is uniform, and the caption matches CRL-0001.

---

# PART TWO: THE NAIVE BASELINE (stage4-rog7-NAIVE-baseline.md)

Scope restated from the checklist for Interrogatory No. 7: "Single subject, narrow on its face. The boundary is the reason for the termination; a careless answer would argue the case, recite performance history covered by Interrogatory No. 4, or offer multiple shifting rationales without counsel's direction. The answer given here fixes the Company's stated position." Findings in severity order.

## B1. PRIVILEGE FAIL (top of section per protocol): the baseline discloses the substance of the withheld attorney client communication, with citation

Paragraph 5's closing sentence restates the privileged advice from CRL-0008, the document the gate withheld in full, and cites it into a discovery answer:

```
Baseline, paragraph 5: "Prior to the termination, the Company also
sought and obtained legal advice from its General Counsel, Gregory
Aldana, regarding the restructuring and the selection decision,
including advice that the selection be made at the March 30 review
on documented, objective criteria with the financial analysis before
the group (CRL-0008; CRL-0010)."
```

That is a near verbatim restatement of the March 19, 2026 advice in the withheld thread (compare CRL-0008, Aldana message; not requoted here). Served as written, this discloses privileged advice to the adverse party, invites a subject matter waiver argument reaching the whole thread and the related severance advice, and does it in the Company's own sworn answer. It also affirmatively ties counsel's advice to "the selection decision," the exact linkage the gate withheld. This is the disqualifying defect of the baseline.

## B2. Privilege FAILs, additional

**(a) The withheld document is listed as relied upon.** "Documents principally relied upon: CRL-0002 through CRL-0019" sweeps in CRL-0008 (withheld in full), CRL-0011 (routed, queue item 3), CRL-0013 including its routing note (queue item 4), and CRL-0010 unredacted. A reliance list naming a withheld privileged document in a served answer is itself a disclosure and a waiver hook.

**(b) Routed material is used directly.** Paragraph 4 draws its implementation timeline from CRL-0011, queue item 3, whose production posture is undecided: "the CFO circulated an implementation punch list on March 31, 2026 setting the notification meeting for April 6, 2026 and the separation effective date as April 17, 2026 (CRL-0011)."

**(c) Counsel is named as a knowledge source without any privilege objection.** "Persons with knowledge of this answer: ... Gregory Aldana, General Counsel." Combined with B1, this presents the General Counsel as a witness on the substance of his own advice. The baseline contains no privilege objection, no privilege log reference, and no redaction handling anywhere.

## B3. Record conflicts sworn into the answer, unflagged

**(a) The March 26 versus March 30 decision date conflict is sworn on both sides of itself.** Paragraph 2 swears the consolidation was approved at the March 30 review; paragraph 4 swears "HR working notes reflect that on March 26, 2026 Mr. Kestner confirmed the Whitfield position would be eliminated and that severance paperwork should begin (CRL-0010)." The baseline hands opposing counsel the predetermination timeline inside the Company's own sworn answer, with no flag and no reconciliation. Receipts as in Part One, finding R2.

**(b) The proposal date conflict (Part One, finding R1) infects the baseline the same way.** Paragraph 2 swears "The CFO's March 25, 2026 memorandum proposed consolidating the two operations manager positions," while the record it cites elsewhere (CRL-0008; CRL-0010 entry 2026-03-18) shows the proposal and the March 30 meeting date in circulation by March 18 and 19. Unflagged.

**(c) Internal contradiction on performance.** The answer swears both of these:

```
Baseline, opening paragraph: "Plaintiff's employment was not
terminated for cause, for performance reasons, or for any reason
personal to Plaintiff other than the elimination of her position."

Baseline, paragraph 3: "The selection between the two operations
manager positions was based on objective factors, including
comparative regional consolidation requirements and recent
performance assessments," followed by the 3 of 5 versus 4 of 5
rating comparison and the February 2026 review's "communication
friction" finding.
```

Not for performance reasons, then selected on performance. The two sentences coexist only with careful drafting the baseline does not do; as written they are a cross examination exhibit. And volunteering the February 20, 2026 review's friction finding, seventeen days after the February 3 complaint about dispatch, gift wraps the pretext narrative.

## B4. Citation audit

All 22 citation clusters (36 document citations) reopened. Result: **20 clusters MATCH, 2 clusters STRETCH, 0 accuracy FAILs.** The B1 citation of CRL-0008 is accurate as support, which is precisely the problem; it is graded under the privilege check, not as a citation miss. The STRETCH grades:

**(a) Paragraph 4, paid through claim:** "Plaintiff was paid through April 17, 2026, together with accrued and unused paid time off ... (CRL-0012; CRL-0013; CRL-0010)." CRL-0012 promises payment prospectively ("You will be paid through April 17, 2026, together with all accrued and unused paid time off"); CRL-0010 entry 2026-04-17 says only "Final pay processed," silent on PTO. Asserting completed PTO payment outruns the record. Also in the same sentence, the offer particulars (May 8 date, eight weeks) are supported by CRL-0013 alone; CRL-0012 states neither.

**(b) Paragraph 5, investigation cluster:** "(CRL-0005; CRL-0010; CRL-0018; CRL-0019)" is cited for the investigation narrative. CRL-0018 is the handbook policy excerpt; it supports no sentence of the narrative. CRL-0019 is the underlying dispatch email, not evidence of the investigation steps. The narrative facts trace to CRL-0005 and CRL-0010; half the cluster is decoration.

## B5. Scope audit

Sentence one states the reason and is within scope. Everything after it exceeds the question. Grades:

- Opening paragraph, sentence 2 ("not terminated for cause, for performance reasons ..."): argument and characterization beyond the stated reason, and the fuse for B3(c). REMOVE (counsel may separately choose a defensive phrasing, but not this one and not here).
- Opening paragraph, sentence 3 ("The full circumstances are as follows.") and paragraph 1 (business conditions narrative, 6 sentences): ROG No. 6 territory. REMOVE.
- Paragraph 2 (consolidation decision narrative, 3 sentences): ROG No. 6 territory. REMOVE.
- Paragraph 3 (selection detail and comparator ratings, 5 sentences): ROG No. 8 territory, volunteers performance detail the checklist expressly warns against, and feeds B3(c). REMOVE.
- Paragraph 4 (implementation and notification, 4 sentences): ROG No. 6 territory; swears the March 26 entry unflagged (B3(a)); uses routed CRL-0011 (B2(b)). REMOVE.
- Paragraph 5 (complaint investigation narrative and the no role argument, 7 sentences): ROG No. 5 territory, argues the case, and ends in the B1 privilege disclosure. REMOVE; the final sentence must be removed on privilege grounds independent of scope.
- "Persons with knowledge" and "Documents principally relied upon" blocks: not asked by ROG No. 7 (they answer ROG No. 1 and RFP No. 1 badly), and both carry privilege problems (B2). REMOVE.

Count: 27 of 28 sentences plus both closing blocks exceed the question's scope. The protocol drafts answer the same interrogatory in one sentence with one citation, graded MATCH, with zero scope excess.

## B6. Completeness and comparison

As a single answer, the baseline responds to the interrogatory, so no response gap exists. It contains no objection preserving anything, no privilege log reference, no verification gate, and no flag on either record conflict it swears through. Same record, same question: the protocol draft produced one clean sentence; the baseline produced five paragraphs containing two unflagged record conflicts, an internal contradiction, and a privilege disclosure with a waiver exposure. That contrast is the demonstration.

---

# WHAT WAS CHECKED (closing statement per protocol)

The protocol requires a statement of what was checked, not only what was found. Clean areas below were affirmatively verified, not assumed.

1. **Citation audit.** 111 bracketed citations in the protocol drafts, each reopened against the cited document and passage: 109 MATCH, 2 STRETCH, 0 FAIL. 22 citation clusters (36 document citations) in the baseline, each reopened: 20 MATCH, 2 STRETCH, 0 accuracy FAILs, with the CRL-0008 citation graded as the B1 privilege FAIL.
2. **Date cross check.** 31 distinct dated assertions in the protocol drafts and 19 in the baseline, each checked against every collected document speaking to the same event, across the full 23 document set. Eleven day of week statements in the record recomputed against the 2026 calendar (all correct). Arithmetic recomputed: the severance figure (108,000 dollars at 8 weeks equals 16,615.38 dollars) and the consideration window lapse (May 8 plus 21 days equals May 29). Two record conflicts found (R1 new, R2 previously flagged); every other cross checked date agreed across all sources that state it.
3. **Scope audit.** All 22 protocol draft responses audited against scope restated from the Stage 1 checklist: 2 excesses, both FLAG FOR COUNSEL, 0 REMOVE. The baseline answer audited against the ROG No. 7 scope: 27 sentences plus 2 closing blocks graded REMOVE.
4. **Privilege leak check.** Both drafts searched in full against the CRL-0008 thread content, the redacted final sentence of CRL-0010 entry 2026-05-27, and all four human review queue items. Protocol drafts: one qualified hit (P1, the routed 2026-03-18 entry cited for fact and date only, self disclosed, pending counsel) and one low citation range note (P2); no substance from any withheld or routed source appears. Baseline: one direct disclosure of withheld advice substance (B1), plus reliance listing of withheld and routed documents, direct use of routed CRL-0011, and counsel named as a knowledge source (B2).
5. **Completeness.** 22 of 22 requests have responses. All 18 responsive documents in the triage table reconciled against the production statements; the RFP No. 1 population independently rebuilt from the answers and matched exactly (14 documents). Both withheld units (CRL-0008 in full; the CRL-0010 redaction) have privilege log entries (1 and 2; 3). Two completeness findings (F1 flag, F2 minor); all draft stated open items verified as accurately stated.
6. **Dash rule.** This report and both graded drafts were scanned for em dash and en dash characters; none present in any of the three files.

Finding totals, protocol drafts: 1 qualified privilege hit plus 1 low privilege note; 2 record conflicts (1 new and unflagged, 1 flagged by the drafts); 0 citation FAILs (2 STRETCH); 2 scope excesses (both FLAG FOR COUNSEL); 2 completeness gaps (1 flag, 1 minor); 1 style item.

Finding totals, naive baseline: 4 privilege failures (1 substance disclosure, 3 associated); 3 conflict findings sworn unflagged (2 record conflicts, 1 internal contradiction); 0 citation accuracy FAILs (2 STRETCH); 27 sentences plus 2 blocks of scope excess graded REMOVE; no objection, log, or verification apparatus at all.

Verification posture: the protocol drafts may proceed to counsel revision with the R1 conflict added to the counsel queue alongside the items the drafts already hold open; no answer touching the restructuring timeline should be verified until R1 and R2 are resolved. The baseline is not servable in any part beyond its first sentence.
