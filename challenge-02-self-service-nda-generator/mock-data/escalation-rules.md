# NDA Escalation Rules

## When to Escalate to Legal

The self-service NDA generator should handle standard NDA requests without legal involvement. However, certain situations require human legal review. The tool should **flag the request for legal review** if any of the following conditions are met.

---

## Mandatory Escalation Triggers

### 1. Government Entities
- **Trigger:** Counterparty is a government agency, state-owned enterprise, or quasi-governmental body
- **Reason:** Government entities often have their own required contract forms, sovereign immunity considerations, and specific regulatory requirements (e.g., FAR clauses for US federal agencies)
- **Action:** Escalate to legal. Inform the requester that government NDAs typically require specialized handling.

### 2. M&A / Investment Context
- **Trigger:** The purpose involves a potential acquisition, merger, investment, or similar corporate transaction
- **Reason:** M&A NDAs require additional provisions (standstill, non-solicitation of employees, exclusivity, etc.) and are typically handled by specialized counsel
- **Action:** Escalate to legal. Recommend the requester contact the General Counsel's office directly.

### 3. Highly Regulated Data
- **Trigger:** The confidential information involves any of the following:
  - Protected health information (PHI) or HIPAA-regulated data
  - Financial data subject to banking secrecy or securities regulations
  - Classified or government-restricted information
  - Children's data (COPPA)
  - Biometric data
- **Reason:** These data categories may require additional agreements (BAA, DPA) or specialized terms beyond a standard NDA
- **Action:** Escalate to legal. Flag the specific data type for legal's attention.

### 4. Certain Jurisdictions
- **Trigger:** Counterparty is located in or governed by laws of:
  - People's Republic of China
  - Russia
  - Countries subject to comprehensive sanctions (North Korea, Iran, Syria, Cuba, etc.)
  - Any jurisdiction where TechForward does not currently operate
- **Reason:** These jurisdictions may have unique enforceability concerns, data localization requirements, export control implications, or sanctions risks
- **Action:** Escalate to legal. Flag the jurisdiction-specific concerns.

### 5. Deal Value Thresholds
- **Trigger:** The potential business relationship has an estimated value exceeding EUR 5,000,000
- **Reason:** High-value transactions warrant customized terms and senior legal oversight
- **Action:** Escalate to legal with deal context.

### 6. Non-Standard Requests
- **Trigger:** The requester indicates any of the following:
  - The counterparty insists on using their own NDA template
  - The counterparty has requested modifications to our standard terms
  - The confidentiality period needs to be longer than 5 years
  - There is a need for a "clean room" or "data room" arrangement
  - The NDA needs to cover a joint venture or co-development arrangement
- **Reason:** These situations require legal judgment about acceptable deviations from standard terms
- **Action:** Escalate to legal with details of the non-standard request.

---

## Soft Flags (Proceed with Caution)

These situations don't require mandatory escalation but should be flagged to the requester with guidance:

### A. Personal Data Sharing
- **Flag:** The purpose involves sharing employee data, customer data, or other personal data
- **Guidance:** Inform the requester that an NDA alone may not be sufficient — a Data Processing Agreement (DPA) may also be required. Suggest they consult with the Data Protection Officer.

### B. Technical IP Sharing
- **Flag:** The purpose involves sharing source code, algorithms, patentable inventions, or core technology
- **Guidance:** Recommend the requester confirm with their manager and the IP team that sharing this information is appropriate and that the NDA scope adequately protects the disclosed IP.

### C. Competitor Counterparties
- **Flag:** The counterparty appears to be a direct competitor
- **Guidance:** Warn the requester about antitrust/competition law implications of information sharing with competitors. Recommend they consult legal if there is any doubt about the appropriateness of the disclosure.

---

## Escalation Process

When an escalation is triggered:

1. **Do not generate the NDA** — inform the requester that this request requires legal review
2. **Provide a clear explanation** of why escalation is needed (reference the specific trigger)
3. **Capture all intake information** so that legal has context when they pick up the request
4. **Route the request** to the legal team with:
   - Requester name and department
   - Counterparty details
   - Purpose of the NDA
   - Specific escalation trigger(s)
   - Any additional context provided by the requester
5. **Set expectations** — inform the requester that legal will respond within 2 business days
