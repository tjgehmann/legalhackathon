# Challenge 12: Sales Contract Review Playbook

## The Problem

TechForward's sales team closes 30–50 deals per month. For every deal, customers push back on the standard contract — asking for better payment terms, lower liability caps, different IP ownership clauses, or custom data processing agreements. Sales reps don't know which redlines they can accept on the spot, which need a quick legal check, and which are deal-breakers.

The result: reps either slow down deals by routing every question to Legal (who is already overloaded), or they accept risky terms to close faster without understanding the exposure. Junior AEs copy what they've seen senior reps do — and senior reps aren't always right. There is no consistent, accessible playbook.

Legal wants a tool that empowers the sales team to handle routine contract negotiations autonomously — without Legal needing to be in the room for every deal.

## Your Mission

Build an AI-powered Sales Contract Review Playbook that:

1. **Analyzes customer-proposed redlines** to TechForward's standard sales contract and classifies each change as: ✅ Accept / 🔶 Negotiate / 🚫 Escalate to Legal
2. **Explains the risk** behind each redline in plain language that a non-lawyer sales rep can understand (e.g., "This clause removes your right to collect interest on late payments — only accept if the deal is above EUR 500K")
3. **Suggests counter-proposals** for each contested clause — exact alternative language the sales rep can paste into the redlined document
4. **Generates a negotiation briefing** summarizing the deal's risk profile, what to push back on, and what can be conceded, before the rep enters a negotiation call
5. **Produces a pre-signature checklist** ensuring all required fields, approvals, and compliance items are present before a contract goes to signature

## What Success Looks Like

- A sales rep pastes in a customer's redlined contract (or a list of requested changes) and receives a clear, actionable playbook within seconds
- The playbook gives reps enough context to negotiate confidently — without needing to understand contract law
- Escalation recommendations are precise: the rep knows *why* an issue needs Legal, not just *that* it does
- Counter-proposal language is ready to copy-paste, dramatically reducing back-and-forth
- Legal can rely on the playbook's guidance being consistent with company policy — reducing post-signature cleanup and contract-driven disputes

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `techforward-standard-sales-contract.md` | TechForward's standard outbound sales contract (the baseline document) |
| `customer-redlines-enterprise-deal.md` | A real set of customer redlines from an enterprise deal — covering payment, liability, IP, and DPA terms |
| `sales-negotiation-scenarios.json` | Six deal scenarios (SMB, mid-market, enterprise, public sector) with different risk tolerances and approval thresholds |
| `negotiation-playbook-template.md` | A structured template showing what a completed playbook output should look like |

## Suggested Approach

1. Start by understanding TechForward's standard positions as the seller (not the buyer — this is the reverse of Challenge 1)
2. Build a system prompt that defines acceptable ranges, escalation triggers, and counter-proposal logic for each key clause category
3. Feed in the customer redlines and generate a clause-by-clause playbook
4. Test with the negotiation scenarios — different deal sizes and customer types should produce different recommendations
5. Refine the counter-proposal language so it's copy-paste ready (not just a description of what to say)
6. Build the pre-signature checklist as a final output

## Key Clause Categories to Cover

The playbook should address at minimum:

| Category | What to Check |
|----------|---------------|
| **Payment Terms** | Net days, late interest, invoice dispute windows, upfront vs. milestone payments |
| **Liability Cap** | Cap amount relative to contract value, carve-outs, mutual vs. one-sided |
| **Warranty & SLA** | Uptime commitments, remedy caps, exclusions |
| **IP Ownership** | Custom work, feedback clauses, license scope |
| **Data Processing** | Sub-processor approval, breach notification timelines, data deletion |
| **Termination** | For-cause triggers, for-convenience notice, wind-down obligations |
| **Governing Law** | Acceptable jurisdictions, arbitration vs. litigation |
| **Confidentiality** | Duration, permitted disclosures, return/destruction obligations |

## Stretch Goals

- Build an **escalation routing workflow** that generates a pre-filled email to Legal with all relevant context, so the handoff takes seconds instead of a phone call
- Create a **"deal health score"** that rates the overall contract risk from 1–10 based on the combination of accepted redlines
- Add a **customer profiling mode** that adjusts recommendations based on the customer's industry, size, and jurisdiction (e.g., stricter guidance for public sector or regulated industries)
- Build a **version comparison tool** that compares the customer's latest draft against the previous version and highlights only new changes
- Generate a **one-page deal brief** for the sales manager and CFO showing contract value, term, and deviations from standard that affect revenue or liability exposure
