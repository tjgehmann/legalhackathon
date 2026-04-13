# Contract Approval Gate Rules

## Overview

Every contract request flows through a three-tier approval gate before a contract is generated and sent. The tier determines who must approve the contract and how quickly. The gate is applied consistently — the same inputs always produce the same tier assignment.

---

## Tier 1: Auto-Approve (Generate Immediately)

No human approval required. The system generates the contract and the requester can send it directly.

**All of the following must be true:**

- Contract type is an NDA, standard service/consulting agreement, standard vendor agreement, or SaaS/tool agreement
- Counterparty is a private company (not a government entity, state-owned enterprise, or listed public company)
- Contract value is below EUR 50,000 (or not applicable, e.g. NDAs)
- Governing law is German law or the law of an EU member state
- Term or confidentiality period does not exceed 3 years
- No highly regulated data involved (no PHI, financial data subject to banking secrecy, biometric data, children's data, classified information)
- No non-standard terms requested (no custom indemnity, no IP ownership changes, no deviations from standard template)
- Counterparty jurisdiction is one of: EU member states, United Kingdom, Switzerland, United States, Canada, Australia, Japan, New Zealand, Norway, or Iceland

**Output:** Fully generated contract, ready to countersign and send.

---

## Tier 2: Manager Gate (Business Manager Must Approve)

The requester's direct manager must approve before the contract is generated and sent. Target turnaround: **24 hours**.

**Triggered by any one of the following:**

- Contract value is between EUR 50,000 and EUR 500,000
- Counterparty jurisdiction is outside the Tier 1 approved list but not in the Tier 3 restricted list (e.g. Brazil, India, UAE, South Korea, Mexico, South Africa)
- Term or confidentiality period is between 3 and 5 years
- Contract includes a non-solicitation clause, exclusivity clause, or right of first refusal
- Counterparty is a publicly listed company where disclosure obligations may apply
- Requester's department does not typically enter this contract type (e.g. HR requesting a vendor software agreement)
- Contract covers multi-vendor arrangements, subcontracting rights, or staff augmentation
- A soft-flag condition applies (see below) — soft flags alone do not change the tier but do appear in the manager packet
- Contract includes a limitation of liability waiver or cap above EUR 500,000

**Manager approval packet must include:**

1. Plain-language summary of the contract purpose and key commercial terms
2. Counterparty details (name, type, jurisdiction)
3. Reason(s) the contract landed at Tier 2 (specific trigger(s))
4. Any soft-flag warnings with recommended actions
5. Draft contract for the manager's reference
6. Confirmation checkbox: manager is explicitly approving the stated scope and terms

---

## Tier 3: Legal Gate (Legal Team Must Approve)

The legal team must review and approve before the contract is sent. Target turnaround: **48 hours**.

**Triggered by any one of the following:**

- Contract value exceeds EUR 500,000
- M&A, investment, joint venture, or co-development context
- Counterparty is a government agency, state-owned enterprise, or quasi-governmental body
- Counterparty jurisdiction is: People's Republic of China, Russia, North Korea, Iran, Syria, Cuba, Belarus, or any territory subject to comprehensive EU/UN/US sanctions
- Highly regulated data is in scope: protected health information (PHI/HIPAA), data subject to banking secrecy or securities regulation, classified/government-restricted information, biometric data, or children's data (COPPA)
- Non-standard terms requested: counterparty insists on their own template, custom indemnity structure, IP ownership changes, warranty carve-outs, or arbitration clauses not in the standard template
- Confidentiality or contract term exceeds 5 years
- Revenue-sharing, royalty, or profit-participation arrangement
- Contract requires a "clean room" or data room arrangement
- Potential deal value exceeds EUR 5,000,000 (even if initial contract value is lower)
- Counterparty has proposed or rejected material terms during prior negotiations

**Legal brief must include:**

1. Executive summary (2–3 sentences: what is being contracted, with whom, and why it needs legal review)
2. Counterparty profile (name, entity type, jurisdiction, ownership, any known flags)
3. Contract type and key commercial terms (value, duration, obligations, IP treatment)
4. Specific Tier 3 trigger(s) with risk explanation
5. Open issues and questions legal must resolve before approval
6. Draft contract with trigger-relevant clauses clearly flagged
7. Requester contact details, internal sponsor, and urgency/deadline

---

## Soft Flags (Do Not Change Tier — Add Warning)

These conditions appear in the approval packet for any tier but do not change the tier assignment on their own. They must be surfaced to the requester and any approver.

| Flag | Condition | Guidance |
|------|-----------|----------|
| Personal data sharing | Scope involves sharing employee, customer, or other personal data | A separate Data Processing Agreement (DPA) may be required. Consult the Data Protection Officer before proceeding. |
| Technical IP disclosure | Scope involves source code, algorithms, patentable inventions, or core technology | Confirm with the IP team that disclosure is appropriate and that the contract scope adequately protects the IP. |
| Competitor counterparty | Counterparty is a direct or indirect competitor | Review antitrust/competition law implications. Consult legal if there is any doubt about the appropriateness of disclosure. |
| GDPR transfer risk | Counterparty is in a country without an EU adequacy decision | Standard Contractual Clauses (SCCs) or another approved transfer mechanism may be required. Consult the DPO. |
| Regulated sector | Counterparty operates in a regulated sector (financial services, healthcare, critical infrastructure) | Additional regulatory obligations may attach to the contract. Flag for awareness. |

---

## Escalation Overrides

**Upward escalation** (any tier can be moved to a higher tier):

- The requester may self-escalate to request additional scrutiny
- The Tier 2 manager may escalate to Tier 3 if they are uncomfortable approving
- Any legal team member may upgrade a Tier 1 or Tier 2 contract to Tier 3 based on judgment

**Downward de-escalation** (moving to a lower tier):

- Requires explicit written authorization from the legal team
- Must be documented with the rationale for why the Tier 3 trigger no longer applies

---

## Gate Decision Record

For every contract, the system must produce and retain a gate decision record containing:

- Tier assigned and the complete list of triggers that applied
- Approver(s), their role, and their decision (approved / rejected / escalated)
- Timestamp of each approval step
- Any conditions or modifications attached to approval
- Final contract version that was sent

This record is retained for audit and regulatory purposes.

---

## SLA and Escalation on Overdue Approvals

| Gate | Target Response | Overdue Escalation |
|------|----------------|-------------------|
| Tier 2 – Manager | 24 hours | Notify manager's manager and cc legal team |
| Tier 3 – Legal | 48 hours | Notify General Counsel; requester is notified of delay |

If a Tier 2 or Tier 3 approval is not acted on within the target window, the system must surface the overdue item to the next level and notify the requester of the delay.
