# TechForward Customer Care — Escalation Rules & SLA Guidelines

## Purpose

This document defines:
1. **SLA targets** — how quickly agents must respond and resolve each type of complaint
2. **Escalation rules** — who to contact, when, and how
3. **Compliance obligations** — legally binding deadlines that override all other priorities
4. **Agent authority limits** — what agents can decide independently vs. what requires approval

---

## 1. SLA REFERENCE TABLE

| Category | First Response | Resolution | Priority Level |
|----------|---------------|------------|----------------|
| CAT-05 Suspected Data Breach | **1 hour** | 3 business days | CRITICAL |
| CAT-10 Legal Threat / Formal Notice | **2 hours** | 2 business days | CRITICAL |
| CAT-04 GDPR Data Subject Request | **4 hours** | **30 calendar days** (legally binding) | CRITICAL |
| CAT-02 SLA Breach Claim | **8 hours** | 3 business days | HIGH |
| CAT-06 Onboarding / Delivery Failure | **8 hours** | 5 business days | HIGH |
| CAT-07 Product Bug (P1) | **2 hours** | Same business day | HIGH |
| CAT-07 Product Bug (P2) | **4 hours** | 2 business days | HIGH |
| CAT-11 Employee Conduct Complaint | **4 hours** (route to HR) | 3 business days | HIGH |
| CAT-09 Account Access / Locked Out | **4 hours** | **1 business day** | MEDIUM |
| CAT-03 Cancellation / Termination | **24 hours** | 5 business days | HIGH |
| CAT-01 Billing Dispute | **24 hours** | 5 business days | MEDIUM |
| CAT-08 Refund Request | **24 hours** | 5 business days | MEDIUM |
| CAT-07 Product Bug (P3/P4) | **24 hours** | 10 business days | MEDIUM |
| CAT-12 General Dissatisfaction | **24 hours** | 5 business days | LOW |

> **Enterprise / Premium SLA customers:** Reduce all first response SLAs by 50% (e.g., 24h → 12h, 8h → 4h). Check the customer's tier before setting internal deadlines.

> **Business days** = Monday–Friday, 09:00–18:00 CET, excluding German public holidays.

---

## 2. ESCALATION DECISION TREE

### Step 1 — Read the complaint and classify it

Before doing anything else, read the full complaint carefully. Ask:

1. **Does this contain a legal keyword?**
   - Keywords: *"Rechtsanwalt", "lawyer", "solicitor", "legal action", "court", "litigation", "sue", "damages", "formal notice", "breach", "terminate for cause", "Datenschutzbehörde", "supervisory authority", "regulator"*
   - If YES → **Route to Legal immediately (CAT-10 or relevant escalation trigger)**

2. **Does this mention data, privacy, GDPR, or personal information?**
   - Keywords: *"delete my data", "what data do you have", "right to be forgotten", "data access", "GDPR", "personal data", "data breach", "hack", "unauthorized access", "phishing"*
   - If YES → **Route to DPO/SIRT immediately (CAT-04 or CAT-05)**

3. **Does this involve an employee's conduct?**
   - If YES → **Route to HR and Customer Care Manager (CAT-11)**

4. **Can I classify this into one of the 12 categories?**
   - If YES → Follow the category routine and SLA
   - If NO → Start with CAT-12, ask one clarifying question, re-classify when the picture is clearer

---

### Step 2 — Can I resolve this myself?

| Situation | Agent Can Handle | Needs Approval |
|-----------|-----------------|----------------|
| Explaining a correct invoice | ✅ Yes | — |
| Issuing a credit note ≤ EUR 500 | ✅ Yes | — |
| Issuing a credit note > EUR 500 | ❌ No | Finance approval required |
| Confirming SLA service credits ≤ EUR 2,000 | ✅ Yes | — |
| Confirming SLA service credits > EUR 2,000 | ❌ No | Finance + Account Manager |
| Processing a for-convenience termination | ✅ Yes | Notify Account Manager |
| Accepting a for-cause termination | ❌ No | Legal required |
| Issuing a refund ≤ EUR 200 | ✅ Yes | — |
| Issuing a refund > EUR 200 | ❌ No | Finance approval required |
| Restoring account access (technical) | ✅ Yes | After identity verification |
| Restoring access suspended for non-payment | ❌ No | Finance must confirm payment first |
| Offering a 10% retention discount | ✅ Yes | — |
| Offering a retention discount > 10% | ❌ No | VP Sales approval |
| Extending a project timeline | ❌ No | Delivery Manager required |
| Responding to a lawyer's letter | ❌ No | Legal must draft all responses |
| Processing a GDPR DSR | ❌ No | DPO must handle |
| Investigating a potential data breach | ❌ No | SIRT must investigate |

---

### Step 3 — Who do I escalate to?

| Escalation Target | When to Use | Contact Method | SLA for Escalation |
|-------------------|-------------|----------------|-------------------|
| **Legal Team** | Legal threats, for-cause terminations, DSR complexity, formal notices | Email legal@techforward.de with subject: "URGENT LEGAL — [Ticket#] — [Customer]" | Within 2 hours |
| **DPO (Data Protection Officer)** | All GDPR DSRs, data breach reports, subprocessor objections | Email dpo@techforward.de with subject: "DSR/BREACH — [Ticket#] — [Date Received]" | Within 4 hours |
| **SIRT (Security Incident Response Team)** | Any suspected data breach or unauthorized access | Email sirt@techforward.de AND call +49 30 [SIRT hotline] | Within 15 minutes |
| **Finance / Billing** | Credits > EUR 500, refunds > EUR 200, suspended accounts | Create Finance request in CRM: category "Billing Approval" | Within 1 business day |
| **Account Manager** | Enterprise cancellations, SLA breaches on large accounts, retention saves | CRM notification + direct message | Within 4 hours |
| **Customer Care Manager** | Employee conduct complaints, P1 bugs, repeat escalations | Direct message + email | Within 2 hours |
| **Engineering On-Call** | P1 bugs (data loss, core platform unavailable) | PagerDuty alert via support system | Immediate |
| **Delivery Manager** | Onboarding / delivery failures, SOW disputes | CRM escalation flag + email | Within 8 hours |
| **VP Sales** | Retention discounts > 10%, terminations on deals > EUR 200K | Email + CRM flag | Within 1 business day |

---

## 3. COMPLIANCE OBLIGATIONS — LEGALLY BINDING DEADLINES

These deadlines are set by law and cannot be extended without following a formal process. Missing them may result in regulatory fines or legal liability.

### GDPR Data Subject Requests

| Request Type | Legal Basis | Deadline | Extension Option |
|-------------|-------------|----------|-----------------|
| Access Request (Art. 15) | GDPR | 1 calendar month from receipt | Yes — extendable to 3 months for complex/multiple requests; must notify customer within first month |
| Erasure ("Right to be Forgotten") (Art. 17) | GDPR | 1 calendar month | Yes — same extension rules |
| Portability (Art. 20) | GDPR | 1 calendar month | Yes |
| Rectification (Art. 16) | GDPR | 1 calendar month | Yes |
| Objection (Art. 21) | GDPR | Must respond without undue delay | Limited |

**Failure consequence:** Fine up to EUR 20 million or 4% of global annual turnover (whichever is higher).

**Agent action:** Log the exact date of receipt in the DSR register within 4 hours. The clock starts the day the request is received, not the day you open it.

---

### Data Breach Notification (GDPR Art. 33/34)

| Notification | Recipient | Deadline from Awareness |
|-------------|-----------|------------------------|
| Supervisory Authority (Datenschutzbehörde) | TechForward's lead DPA (Berlin, Germany) | **72 hours** |
| Affected individuals (Art. 34) | Individuals at high risk | "Without undue delay" after authority notification |
| Customer notification (contractual) | Customer (per DPA) | **48 hours** (TechForward standard contract) or **24 hours** (negotiated contracts) |

**Agent action:** Any report of suspected or actual unauthorized access to personal data must reach the SIRT within 15 minutes. Do not investigate, do not delay, do not wait for confirmation.

---

### Termination Notices — Contractual Deadlines

| Termination Type | Cure Period | Response Required |
|-----------------|-------------|-------------------|
| For-cause (customer alleging TechForward breach) | 30 days to cure (Section 4.3) | Legal must respond before cure period expires |
| For-convenience (customer) | 90-day notice (Section 4.4) | Acknowledge in writing immediately to start the clock |
| Cooling-off (B2C or contractually agreed) | No cure — immediate right | Confirm and process refund within 10 business days |

---

## 4. COMPLAINT SEVERITY & IMPACT MATRIX

Use this matrix when a complaint doesn't clearly fit one category, or when you need to decide how urgently to act:

| Dimension | Low | Medium | High | Critical |
|-----------|-----|--------|------|---------|
| **Financial Impact** | < EUR 500 | EUR 500 – EUR 5,000 | EUR 5,000 – EUR 50,000 | > EUR 50,000 |
| **Legal / Compliance Risk** | None | Possible contract claim | Breach claim or DSR | Legal action, GDPR violation |
| **Customer Tier** | Basic | Professional | Enterprise | Strategic / Public Sector |
| **Customer Tenure** | New (< 6 months) | Growing (6–24 months) | Established (> 2 years) | Key account |
| **Operational Impact** | Inconvenience | Minor disruption | Operations affected | Production stopped |
| **Recurrence** | First occurrence | Second occurrence | Third+ occurrence | Ongoing / systemic |

> **Rule:** If any single dimension reaches "Critical," treat the entire complaint as critical regardless of other scores. A small customer with a GDPR complaint is just as legally significant as a large one.

---

## 5. DOCUMENTATION REQUIREMENTS

Every complaint must be documented in the CRM system before closing. Minimum required fields:

| Field | Required For |
|-------|-------------|
| Complaint category (CAT-XX) | All complaints |
| Date and time received | All complaints |
| Date and time first response sent | All complaints |
| Date and time resolved | All complaints |
| Resolution summary (2–3 sentences) | All complaints |
| Financial impact (credits, refunds issued) | CAT-01, 02, 08 |
| Escalation log (who, when, why) | All escalated complaints |
| DSR registration date | CAT-04 |
| SIRT notification timestamp | CAT-05 |
| Legal team notification timestamp | CAT-10 |
| Customer satisfaction (if follow-up received) | All complaints |

> **Retention:** Complaint records must be retained for a minimum of **3 years** per TechForward's record retention policy. GDPR-related records must be retained for **5 years**.

---

## 6. PROHIBITED ACTIONS

Agents must **never** do the following, regardless of circumstances:

1. **Make any admission of liability** in writing without Legal approval
2. **Promise a specific remedy** (refund, credit, service level) without confirming internal approval first
3. **Disclose information about other customers**, incidents, or internal systems to the complainant
4. **Delete any records** related to an open complaint or a complaint that may lead to legal proceedings
5. **Respond substantively to a lawyer's letter** — acknowledgment only, then route to Legal
6. **Confirm or deny a data breach** — this determination belongs to SIRT and the DPO
7. **Tell a customer their GDPR rights do not apply** — all DSR claims must be assessed by the DPO
8. **Close a complaint as resolved without following up** to confirm the customer's issue is actually fixed
