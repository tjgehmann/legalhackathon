# EU AI Act Risk Classification Rubric
## A Practical Decision Tool for Internal AI Agent Assessment

*Based on Regulation (EU) 2024/1689 (the EU AI Act). This rubric is a working tool, not legal advice. Consult qualified counsel before making final compliance determinations.*

---

## Step 1: Is This System Covered?

The EU AI Act applies to:
- AI systems **placed on the EU market or put into service in the EU**
- AI systems whose **outputs are used in the EU**
- Applies to both external-facing and **internal-use systems** — an agent used only by employees in Germany is still covered

**Exclusions** (narrow): AI for military/national security purposes; AI for pure scientific research (not deployed); AI for personal non-professional use.

> For any agent your company runs internally or deploys to customers/partners in the EU: **the Act applies.**

---

## Step 2: Is This a Prohibited Practice?

*Article 5 — applies from 2 February 2025. These are hard stops — no business justification overrides them.*

Ask the following questions. If **any** answer is YES → **the system must be shut down or fundamentally redesigned.**

| # | Question | If YES |
|---|----------|--------|
| 2.1 | Does the system use subliminal techniques (below conscious perception) to influence behavior, causing harm? | PROHIBITED |
| 2.2 | Does the system exploit psychological vulnerabilities, age, disability, or social/economic situation to influence behavior against the user's interests? | PROHIBITED |
| 2.3 | Does the system assign social scores to individuals based on behavior, personality, or personal characteristics, used to deny/restrict rights or services? | PROHIBITED |
| 2.4 | Does the system perform **real-time** remote biometric identification of individuals in publicly accessible spaces (with narrow LE exceptions)? | PROHIBITED |
| 2.5 | Does the system infer the **emotional states** of individuals in the **workplace or educational settings**? | PROHIBITED |
| 2.6 | Does the system build or expand facial recognition databases by scraping images from the internet or CCTV? | PROHIBITED |
| 2.7 | Does the system perform **predictive policing** — assessing individuals' likelihood of offending based on profiling or personality traits alone? | PROHIBITED |
| 2.8 | Does the system perform biometric categorization that infers **race, political opinion, trade union membership, religious belief, sexual orientation, or health data** from biometric data? | PROHIBITED |

**Decision:**
- Any YES → **PROHIBITED. Stop deployment immediately. Escalate to Legal.**
- All NO → proceed to Step 3.

---

## Step 3: Is This a High-Risk System?

*Annex III — obligations phasing in 2025–2026.*

An AI system is **HIGH-RISK** if it falls into any of the following categories **AND** makes, or materially influences, decisions about individuals.

### Category A — Employment, Workers, Self-Employment (Annex III §4)

| Question | If YES |
|----------|--------|
| Does the system screen, rank, or filter job applicants? | HIGH-RISK |
| Does it make or recommend hiring, promotion, demotion, or dismissal decisions? | HIGH-RISK |
| Does it monitor, evaluate, or score employee performance? | HIGH-RISK |
| Does it allocate tasks, set working conditions, or determine pay? | HIGH-RISK |

### Category B — Access to Essential Private Services and Public Benefits (Annex III §5)

| Question | If YES |
|----------|--------|
| Does the system assess creditworthiness or establish credit scores? | HIGH-RISK |
| Does it determine access to insurance, pricing, or coverage? | HIGH-RISK |
| Does it determine access to housing, utilities, or essential services? | HIGH-RISK |

### Category C — Education and Vocational Training (Annex III §3)

| Question | If YES |
|----------|--------|
| Does the system determine access to educational institutions? | HIGH-RISK |
| Does it assess, grade, or evaluate students? | HIGH-RISK |
| Does it monitor students during examinations? | HIGH-RISK |

### Category D — Law Enforcement (Annex III §6)
| Question | If YES |
|----------|--------|
| Does the system assist in assessing individuals' risk of offending or re-offending? | HIGH-RISK |
| Does it assess reliability of evidence or witness credibility? | HIGH-RISK |

### Category E — Critical Infrastructure Safety Components (Annex III §2)

| Question | If YES |
|----------|--------|
| Is the system a safety component of infrastructure in energy, water, transport, or finance? | HIGH-RISK |

### Category F — Administration of Justice / Democratic Processes (Annex III §8)

| Question | If YES |
|----------|--------|
| Does the system assist judges, arbitrators, or prosecutors in legal proceedings? | HIGH-RISK |
| Does it influence elections, referenda, or voting behavior at scale? | HIGH-RISK |

---

**If classified HIGH-RISK, mandatory requirements include:**

- [ ] **Risk management system** — documented, ongoing (Art. 9)
- [ ] **Data governance** — training data quality, bias testing, data minimization (Art. 10)
- [ ] **Technical documentation** — full system documentation before deployment (Art. 11)
- [ ] **Automatic logging** — event logs maintained throughout lifecycle (Art. 12)
- [ ] **Transparency to deployer** — user must receive sufficient info to use correctly (Art. 13)
- [ ] **Human oversight** — meaningful human ability to monitor, intervene, override (Art. 14)
- [ ] **Accuracy, robustness, cybersecurity** — tested and documented (Art. 15)
- [ ] **Conformity assessment** — self-assessment or third-party depending on category (Art. 43)
- [ ] **EU Database registration** — before deployment (Art. 49)
- [ ] **Fundamental rights impact assessment** — for certain deployers (Art. 27)

---

## Step 4: Does This System Have Transparency Obligations?

*Article 50 — applies to all systems, regardless of risk tier.*

| Question | Obligation |
|----------|-----------|
| Does a human interact with the system without necessarily knowing it's AI? | Must disclose clearly that the user is interacting with an AI system, at the start of each interaction |
| Does the system generate synthetic audio, video, images, or text intended for publication? | Must label the content as AI-generated |
| Does the system perform emotion recognition or biometric categorization? | Must notify the subjects being analyzed |
| Does the system operate as an AI model with a persona (e.g., "Hi, I'm Aria from TechCorp")? | May maintain persona but must disclose it's AI when sincerely asked |

---

## Step 5: Final Classification

| Classification | What it means | Action required |
|----------------|--------------|-----------------|
| **PROHIBITED** | Violates Art. 5 | Shut down immediately. Do not redeploy without fundamental redesign and legal review. |
| **HIGH-RISK** | Annex III category | Cannot deploy until all Art. 9–15 requirements are met. Register in EU database. |
| **LIMITED RISK** | Has transparency obligations only | Add required disclosures. No conformity assessment needed. |
| **MINIMAL RISK** | No specific obligations | Best practice: document it anyway. Add to internal registry. |

---

## Quick Reference: Classification by Scenario

| Agent type | Typical classification | Key risk |
|-----------|----------------------|----------|
| CV screener / hiring assistant | HIGH-RISK | Annex III §4 — employment decisions |
| Automated leave approval/denial | HIGH-RISK | Annex III §4 — working conditions |
| Emotion analysis of employees | PROHIBITED | Art. 5(1)(f) — emotion in workplace |
| Creditworthiness / payment terms scorer | HIGH-RISK | Annex III §5 — access to financial services |
| Customer service chatbot (external) | LIMITED RISK | Art. 50 — must disclose AI identity |
| Internal IT helpdesk bot | LIMITED RISK | Art. 50 if not obvious it's AI |
| Email drafting assistant (human reviews) | MINIMAL RISK | No specific obligations |
| Document summarizer (human reviews) | MINIMAL RISK | Low risk if no autonomous action |
| Security system with auto account suspension | HIGH-RISK (likely) | Annex III §6 or fundamental rights impact |
| Social scoring system | PROHIBITED | Art. 5(1)(c) |
