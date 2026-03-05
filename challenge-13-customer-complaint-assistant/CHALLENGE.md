# Challenge 13: Customer Complaint Resolution Assistant

## The Problem

TechForward's customer care team handles 200–300 inbound complaints per month across email, support tickets, and live chat. The same issues come up again and again — billing disputes, SLA breach claims, cancellation requests, data access requests, and onboarding failures.

Right now, each agent handles these situations differently. One agent offers a refund; another doesn't. One correctly spots that a complaint contains a GDPR data access request buried in an angry email; another treats it as a generic complaint and responds in 5 business days instead of the legally required 1 month. One agent escalates everything to a senior; another resolves things that should have been escalated.

The result: inconsistent customer experience, compliance risk, unnecessary escalations, and senior team members spending their time supervising situations that a good playbook could resolve autonomously.

The team needs a tool that equips every agent — including new starters — to handle standard complaints correctly, consistently, and confidently, on the first try.

## Your Mission

Build an AI-powered Customer Complaint Resolution Assistant that:

1. **Classifies incoming complaints** by type (billing, SLA, cancellation, data rights, product defect, etc.), urgency, and whether they contain a legally significant request (GDPR DSARs, formal contract claims, legal threats)
2. **Suggests the correct response routine** for each complaint type — a step-by-step guide telling the agent exactly what to do, in what order, with what approvals
3. **Generates a draft response** using pre-approved templates, personalized with the customer's name and specific complaint details
4. **Flags compliance-critical situations** such as GDPR Subject Access Requests, formal contract termination notices, or implied legal threats — and routes them immediately to the correct team
5. **Tracks resolution SLAs** by complaint type so the agent knows when a response is due and whether it is at risk

## What Success Looks Like

- A new customer care agent can handle 90% of standard complaints correctly without supervisor intervention, by following the assistant's routine
- Legally significant requests (DSARs, formal complaints, legal notices) are never misclassified as routine tickets — they are always flagged and routed correctly
- Every customer receives a response that matches TechForward's tone guidelines: professional, empathetic, clear, and solution-oriented
- Agents spend less time drafting from scratch and more time resolving — average handle time drops by 30%
- The tool produces a consistent paper trail that can be reviewed if a complaint escalates to a formal dispute

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `complaint-categories.json` | 12 complaint categories with severity levels, SLA targets, required actions, and escalation triggers |
| `response-templates.md` | Pre-approved response templates for each complaint category, with placeholder fields for personalization |
| `sample-complaints.json` | 10 realistic customer complaints spanning all major categories — including some that contain hidden legal significance |
| `escalation-and-sla-rules.md` | Escalation decision tree, SLA targets by complaint type, and compliance obligations (GDPR, contract law) |

## Suggested Approach

1. Start by reading the complaint categories and SLA rules to understand the landscape of issues agents face
2. Build a classifier prompt that reads a raw complaint and outputs: category, urgency, SLA deadline, and whether it contains a legally significant request
3. For each category, build a response routine — a numbered checklist of what the agent should do
4. Connect the routine to a template: the agent fills in the blanks, the tool generates the response
5. Test with the 10 sample complaints — check whether the legally significant ones are correctly flagged
6. Iterate on tone and empathy: the tool should never sound robotic or dismissive

## Key Complaint Categories to Cover

| Category | Why It Matters |
|----------|---------------|
| **Billing dispute** | Risk of chargebacks; customer retention; may contain contract termination intent |
| **SLA breach claim** | Contract liability; customer may be entitled to service credits or termination rights |
| **Cancellation request** | Must distinguish: within cooling-off period, for-cause termination, or for-convenience |
| **GDPR / Data Subject Request** | Legal deadline (1 month); non-compliance = regulatory fine up to 4% of global turnover |
| **Data breach notification** | Customer notifying TechForward of a suspected breach — incident response must activate |
| **Onboarding / delivery failure** | Contract warranty implications; may trigger remedy or refund obligations |
| **Product bug / feature complaint** | SLA and warranty assessment; distinguish critical vs. cosmetic bugs |
| **Refund request** | Apply correct refund policy based on contract type and termination clause |
| **Account access / locked out** | Urgency depends on customer tier; may have SLA implication |
| **Legal threat / formal notice** | Immediate Legal team routing; no response without approval |

## Stretch Goals

- Build a **complaint triage dashboard** showing open tickets by category, SLA status (on track / at risk / breached), and agent assignment
- Add a **sentiment analysis layer** that adjusts response tone based on how angry or distressed the customer sounds — more empathetic language for high-distress complaints
- Create a **"what went wrong" summary** that the agent fills in after resolution, feeding back into a monthly complaint trend report
- Build a **GDPR DSAR workflow** as a dedicated sub-tool: intake → identity verification checklist → data collection guide → response template → deadline tracker
- Add a **multi-language support mode** that detects complaint language and drafts the response in German, French, or English accordingly
