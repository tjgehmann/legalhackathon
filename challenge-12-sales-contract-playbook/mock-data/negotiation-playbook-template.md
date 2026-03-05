# Sales Contract Negotiation Playbook — Output Template

> This template shows what a **completed playbook output** should look like when the AI tool processes a set of customer redlines. Use this as your target format when building the solution.

---

## DEAL OVERVIEW

| Field | Value |
|-------|-------|
| Customer | [Customer Name] |
| Deal Value | EUR [X] / year · EUR [Y] total |
| Contract Term | [X] months |
| Account Executive | [Name] |
| Playbook Generated | [Date] |
| **Overall Risk Rating** | 🟡 MEDIUM — 3 issues require VP approval, 1 requires Legal review |

---

## EXECUTIVE SUMMARY

> *(2–3 sentence summary of the deal's negotiation status — what can be closed today, what needs escalation, and the most critical issues)*

**Example:**
> GlobalManufacturing has submitted 14 redlines. Most commercial changes (payment terms, SLA credits) are within pre-approved ranges for a deal of this size and can be accepted today. Two issues — the Most Favored Customer clause and the 36-month liability cap — require Legal review and CFO approval before TechForward can respond. The remaining items can be resolved in one negotiation session using the counter-proposals below.

---

## CLAUSE-BY-CLAUSE ANALYSIS

### 🔴 ESCALATE TO LEGAL — Do not accept or counter without Legal sign-off

---

#### Issue 1: Most Favored Customer Clause (Section 11.7 — New Clause)

| | |
|--|--|
| **Customer Ask** | Guarantee that pricing is no worse than any comparable customer; offer equivalent terms if a better deal is given to anyone else |
| **Risk Level** | 🔴 Critical — Deal-Breaker |
| **Why This Is a Problem** | MFC clauses create an open-ended commercial obligation that is impossible to monitor and enforce. TechForward's pricing is confidential and varies by deal size, bundling, and negotiation. Accepting this clause would either (a) require disclosing other customers' pricing or (b) expose TechForward to breach claims every time a discount is offered to any customer. **TechForward's policy prohibits MFC commitments.** |
| **Recommendation** | Reject entirely — this is a company-wide policy. Do not negotiate or offer alternatives that achieve the same economic outcome. |
| **What to Say to the Customer** | *"TechForward doesn't offer MFC commitments as a policy, as our pricing reflects deal-specific commercial terms including volume, term, and services mix. We're happy to confirm that the pricing in your proposal reflects our best enterprise rate for a deal of this size and commitment."* |
| **Escalation Path** | Inform customer this requires VP Sales sign-off. VP Sales to confirm rejection. Do not counter without VP sign-off. |

---

#### Issue 2: Liability Cap — 36-Month Cap on TechForward (Section 7.2)

| | |
|--|--|
| **Customer Ask** | TechForward's liability capped at 36 months of fees (EUR 1.44M); Customer's liability remains at 12 months (EUR 480K) |
| **Risk Level** | 🔴 High — Requires Legal + CFO Approval |
| **Why This Is a Problem** | A 36-month cap on TechForward equals the full contract value. This is asymmetric and significantly increases TechForward's financial exposure. The standard 12-month cap (EUR 480K) is already meaningful; 36 months (EUR 1.44M) could exceed TechForward's insurance coverage for a single event. |
| **Acceptable Counter-Position** | TechForward will offer a mutual 24-month cap (EUR 960K per party). This is the maximum pre-approved for enterprise deals. |
| **Counter-Proposal Language** | *"Each party's total aggregate liability arising under or in connection with this Agreement shall not exceed the total fees paid or payable by Customer in the **24 months** immediately preceding the event giving rise to the claim. This cap applies equally to both parties."* |
| **Escalation Path** | Legal to review; CFO approval required for any cap above EUR 720K (24 months of fees). |

---

### 🟡 NEGOTIATE — Counter with the language below; VP approval may be needed

---

#### Issue 3: Payment Terms — Net 60 (Section 3.3)

| | |
|--|--|
| **Customer Ask** | Net 60 instead of TechForward standard Net 30 |
| **Risk Level** | 🟡 Medium |
| **Why This Is a Problem** | Net 60 delays cash collection by 30 days on EUR 480K invoices (annual), creating a EUR 40K monthly cash flow impact. Acceptable for a strategic deal of this size, but worth a counter. |
| **Recommendation** | Accept Net 45. Offer this as a concession in exchange for annual upfront payment (preferred) or to close the deal. Do not go to Net 60 without VP Sales approval. |
| **Counter-Proposal Language** | *"Invoices are due and payable within **45 days** of the invoice date."* |
| **Fallback (with VP approval)** | Accept Net 60 if customer agrees to annual upfront payment and 0.5% early payment discount is removed from the discussion. |

---

#### Issue 4: Price Increase Cap — 3% / HICP (Section 3.6)

| | |
|--|--|
| **Customer Ask** | Reduce price increase cap from 8% to 3% or HICP (whichever is lower); extend notice from 90 to 180 days |
| **Risk Level** | 🟡 Medium |
| **Why This Is a Problem** | Limiting increases to HICP (~2–3% currently) removes pricing flexibility over a 3-year term. TechForward's cost base (infrastructure, engineering) grows faster than CPI. However, this is a 3-year deal and some pricing certainty is reasonable. |
| **Recommendation** | Counter with 5% cap or HICP + 2%, whichever is higher. Accept 180-day notice for this deal size — this is reasonable. |
| **Counter-Proposal Language** | *"TechForward may adjust subscription fees once per year with **180 days' prior written notice**. Annual fee increases are capped at **5% per year** or the HICP for Germany published by Eurostat + 2 percentage points, whichever is lower."* |

---

#### Issue 5: Uptime SLA — 99.9% (Section 5.1)

| | |
|--|--|
| **Customer Ask** | Increase SLA from 99.5% to 99.9% |
| **Risk Level** | 🟡 Medium |
| **Why This Is a Problem** | 99.9% SLA is technically achievable but requires a different infrastructure tier. This is available as a paid add-on at EUR 38,000/year (EUR 3,167/month). Accepting 99.9% without pricing it in transfers infrastructure cost to TechForward. |
| **Recommendation** | Offer 99.9% SLA as a commercial upgrade at EUR 38,000/year, already incorporated into the deal pricing if customer accepts. If customer insists it must be included at current price, escalate to VP Sales. |
| **Counter-Proposal Language** | *"TechForward will use commercially reasonable efforts to ensure the Software is available **99.9%** of the time per calendar month, excluding scheduled maintenance windows communicated 48 hours in advance. This SLA commitment is contingent on Customer's selection of the Enterprise High-Availability Infrastructure Tier, included in the Order Form at the agreed pricing."* |

---

#### Issue 6: SLA Remedy — Termination Right for Persistent Outages (Section 5.2)

| | |
|--|--|
| **Customer Ask** | Right to terminate for cause (with prepaid fee refund) if SLA falls below 99.0% in any rolling 3-month period |
| **Risk Level** | 🟡 Medium |
| **Why This Is a Problem** | Termination rights tied to SLA performance are unusual but not unprecedented. The 99.0% threshold over 3 months is meaningful — that's ~2.2 hours of downtime/month for 3 consecutive months. If TechForward is delivering 99.9%, this trigger should never activate. The fee refund exposure is capped at the pro-rata amount. |
| **Recommendation** | Accept the termination right but modify: (a) threshold should be 98.5% (not 99.0%), (b) must persist for 3 consecutive months (not a rolling window), (c) refund is pro-rata of prepaid fees for remaining unused term only. |
| **Counter-Proposal Language** | *"If the Software fails to achieve 98.5% uptime for three consecutive calendar months, Customer may, upon 30 days' written notice, terminate this Agreement for cause and receive a pro-rata refund of any prepaid, unused subscription fees for the remaining Subscription Term."* |

---

#### Issue 7: Termination for Convenience — 30-Day Notice + Refund (Section 4.4)

| | |
|--|--|
| **Customer Ask** | Reduce notice from 90 to 30 days; receive pro-rata refund of all prepaid fees |
| **Risk Level** | 🟡 High (Revenue Risk) |
| **Why This Is a Problem** | Accepting a full pro-rata refund on a EUR 1.44M contract means TechForward receives no benefit from annual upfront payment and loses infrastructure and staffing cost already committed for the year. Especially high risk given customer is paying annually in advance. |
| **Recommendation** | Counter with 60-day notice (acceptable at this deal size) but do not concede on prepaid fee refunds for convenience termination. Offer a partial refund (25% of unused fees) as a goodwill concession maximum, only with VP approval. |
| **Counter-Proposal Language** | *"Customer may terminate this Agreement without cause upon **60 days'** written notice. In such case, TechForward shall refund to Customer **25% of prepaid, unused subscription fees** for the remaining Subscription Term within 45 days of the effective termination date. This partial refund represents Customer's sole financial remedy for a convenience termination."* |
| **Fallback (deal-breaker check)** | Do NOT accept a full pro-rata refund on convenience termination without CFO approval. |

---

### ✅ ACCEPT — These changes are within pre-approved ranges for this deal

---

#### Issue 8: Invoice Dispute Window — 45 Days (Section 3.5)

| | |
|--|--|
| **Customer Ask** | Extend dispute window from 21 to 45 days |
| **Decision** | ✅ Accept |
| **Rationale** | 45 days is within the pre-approved range for enterprise deals. No material risk to TechForward — invoices with no dispute notified within 45 days are deemed accepted. |
| **Updated Language** | *"Customer may dispute an invoice in good faith within **45 days** of the invoice date by providing written notice specifying the disputed amounts."* |

---

#### Issue 9: Late Payment Interest — 0.5% per Month (Section 3.4)

| | |
|--|--|
| **Customer Ask** | Reduce late interest from 1.5% to 0.5% per month |
| **Decision** | ✅ Accept with counter |
| **Rationale** | 0.5%/month (6%/year) is below market. Counter with 1.0%/month (12%/year), which is the pre-approved minimum for deals above EUR 200K. |
| **Updated Language** | *"Amounts not paid by the due date will accrue interest at **1.0% per month**..."* |

---

#### Issue 10: Data Export Period — 180 Days (Section 4.5)

| | |
|--|--|
| **Customer Ask** | Extend data export window from 45 to 180 days |
| **Decision** | ✅ Accept |
| **Rationale** | For a company processing 2TB of data, 180-day export window is reasonable. No operational cost to TechForward beyond standard hosting. |
| **Updated Language** | *"Customer may export Customer Data for **180 days** post-termination using TechForward's standard export tool."* |

---

#### Issue 11: Auto-Renewal Removal (Section 4.2)

| | |
|--|--|
| **Customer Ask** | Remove auto-renewal; TechForward to notify 90 days before expiry for renewal negotiation |
| **Decision** | ✅ Accept |
| **Rationale** | Removing auto-renewal in exchange for a 3-year commitment is a standard trade. The 90-day advance notice from TechForward is operationally fine. |
| **Updated Language** | *"This Agreement will not automatically renew. TechForward shall provide Customer with written notice of the upcoming expiry at least **90 days** before the end of the then-current Subscription Term. The parties may negotiate renewal terms upon receipt of such notice."* |

---

#### Issue 12: Data Breach Notification — 24 Hours (Section 8.4)

| | |
|--|--|
| **Customer Ask** | Reduce notification time from 48 to 24 hours |
| **Decision** | ✅ Accept (with qualification) |
| **Rationale** | TechForward's ops team has confirmed 24-hour notification of suspected breaches is operationally feasible. This is consistent with regulatory best practice. |
| **Updated Language** | *"TechForward will notify Customer of a **suspected or confirmed** personal data breach within **24 hours** of becoming aware, with a preliminary incident report within 24 hours and a full written report within 72 hours."* |

---

#### Issue 13: Subprocessor Notice — 60 Days (Section 8.3)

| | |
|--|--|
| **Customer Ask** | Extend notice period from 30 to 60 days; extend objection window from 15 to 30 days |
| **Decision** | ✅ Accept notice + objection extension; push back on approval requirement |
| **Rationale** | 60-day notice and 30-day objection window are reasonable for a large enterprise. However, changing "objection right" to "approval requirement" would give customer a veto over TechForward's infrastructure decisions — unacceptable. |
| **Counter-Proposal Language** | *"TechForward will provide Customer with **60 days' prior written notice** before adding new subprocessors. Customer may object within **30 days** on documented data protection grounds. If TechForward cannot accommodate Customer's objection, Customer may terminate this DPA, and TechForward will continue to use the then-current subprocessor list until the end of the notice period."* |

---

#### Issue 14: Publicity / Reference Customer (Section 9.4)

| | |
|--|--|
| **Customer Ask** | Absolute prohibition on use of customer name in any materials, for any reason |
| **Decision** | ✅ Accept |
| **Rationale** | Customer is a publicly listed company with legitimate brand protection concerns. TechForward should not rely on referenceable customers without explicit consent. This is consistent with standard policy. |
| **No changes needed beyond confirming existing language applies.** | |

---

## SOURCE CODE ESCROW REQUEST (New Clause — Section 6.5)

| | |
|--|--|
| **Customer Ask** | Escrow agreement with release upon insolvency, cessation of business, or software discontinuation with less than 12 months' notice |
| **Risk Level** | 🟡 Medium — Non-standard, requires Legal review |
| **Why This Is a Problem** | Source code escrow is legitimate for mission-critical software. However, it has cost implications (escrow agent fees: ~EUR 5,000–15,000/year) and legal complexity around what constitutes releasable "source code." TechForward has a standard escrow template. |
| **Recommendation** | Accept in principle using TechForward's standard escrow addendum. Propose splitting the escrow agent cost 50/50 (TechForward: EUR 5,000/year, Customer: EUR 5,000/year). Legal to review and attach the standard escrow addendum. |
| **Counter-Proposal** | *"The parties will enter into TechForward's standard Source Code Escrow Addendum within 90 days of the Effective Date. Escrow agent fees will be shared equally between the parties."* |

---

## PRE-SIGNATURE CHECKLIST

Before sending for signature, confirm all items below are complete:

- [ ] All redlined clauses have a documented resolution (Accept / Counter / Escalate)
- [ ] VP Sales has approved: Price freeze / 60-day termination notice / 99.9% SLA pricing
- [ ] Legal has reviewed: MFC clause rejection, liability cap counter, source code escrow addendum
- [ ] CFO has approved: Asymmetric liability cap if above EUR 720K
- [ ] Data Processing Agreement (DPA) is attached and signed
- [ ] Source Code Escrow Addendum is attached (if accepted)
- [ ] Order Form reflects correct pricing including 99.9% SLA add-on
- [ ] Auto-renewal language has been removed from the final draft
- [ ] Updated payment terms (Net 45 or Net 60) are reflected in the Order Form
- [ ] Governing law: Berlin courts confirmed (arbitration counter not applicable for this deal)
- [ ] Customer has signed the DPA before or simultaneous with the main Agreement
- [ ] TechForward countersignature authority confirmed: VP Sales or above for this deal value

---

## NEGOTIATION CALL BRIEFING

**Suggested opening position for the next call with GlobalManufacturing:**

> "We've reviewed your redlines carefully and want to have a productive conversation. We can resolve about 10 of the 14 points today — mostly commercial terms, data protection, and operational details where we can meet your needs. We have two items that need internal approvals: the liability cap and the MFC clause. We'd like to propose the following package..."

**Key trades to propose:**
1. Accept 99.9% SLA + 180-day data export → in exchange for annual upfront payment (TechForward preference)
2. Offer Net 45 + 60-day termination notice → instead of Net 60 + 30-day + full refund
3. Accept escrow + 60-day subprocessor notice → as goodwill on data protection
4. Hold firm on MFC rejection → non-negotiable policy item

---

*Template generated by TechForward Sales Contract Review Playbook v1.0*
*This playbook is for internal use only. All language suggestions should be confirmed by Legal before inclusion in a binding contract.*
