# Challenge 2: Self-Service Contract Generator with Approval Gate

## The Problem

Building on the success of the self-service NDA tool, the company now needs to extend self-service contracting to a broader set of standard commercial agreements. Business teams across Sales, Procurement, Marketing, and HR regularly need service agreements, vendor contracts, and tool/SaaS agreements — each flowing through the same slow legal queue.

Current state:

1. Business team submits a contract request to legal
2. Legal triages — often 2+ days just to prioritize
3. Legal drafts or adapts a template
4. Business team reviews and requests changes
5. Back-and-forth until final sign-off
6. Average time to a signed contract: **10–15 business days**

Legal has categorized their inbound work: **65% of contracts are routine and could be generated from pre-approved templates with minimal customization**. The remaining 35% genuinely require legal judgment. The challenge is building a system that can reliably tell the difference — and route each contract to the right approver automatically.

## Your Mission

Build a self-service contract generator with a tiered approval gate that:

1. **Accepts intake** for multiple contract types: NDAs, service/consulting agreements, vendor agreements, and SaaS/tool agreements
2. **Classifies the risk tier** based on contract type, value, counterparty, jurisdiction, and terms requested
3. **Routes through the appropriate gate:**
   - **Tier 1 – Auto-approve:** Standard low-risk contracts → generated and ready to send immediately, no human approval needed
   - **Tier 2 – Manager gate:** Medium-risk or higher-value contracts → requester's manager must approve before the contract is sent (target: 24-hour turnaround)
   - **Tier 3 – Legal gate:** High-risk, high-value, or non-standard → legal team reviews and approves before the contract is valid (target: 48-hour turnaround)
4. **Generates the contract** once all required approvals are obtained — and for Tier 2/3, generates an approval packet for the gatekeeper so they have everything they need in one place
5. **Explains routing decisions** transparently so requesters understand which tier their contract landed in and why

## The Approval Gate — Core Innovation

The approval gate is what separates this from a simple template filler. It must:

- Apply rules **consistently** — the same inputs always produce the same tier
- Give the requester a **clear explanation** of which gate triggered and what happens next
- Capture all required information **upfront** so approvers never have to chase the requester for basics
- For Tier 2: generate a **manager approval packet** — a concise brief with the key commercial terms, risk flags, and a draft contract attached
- For Tier 3: generate a **legal brief** — a structured summary including risk analysis, counterparty profile, open issues, and the draft contract with flagged clauses

## What Success Looks Like

- A procurement manager can generate and send a Tier 1 vendor agreement in under 5 minutes
- A Tier 2 contract reaches the manager as a self-contained approval packet — no follow-up needed
- A Tier 3 contract arrives at legal with a complete intake brief — legal never has to chase for basic information
- The gating logic is transparent and consistent — business teams learn to predict which tier their contracts fall into
- Legal's queue shrinks because the 65% of routine contracts no longer reach them

## Mock Data Provided

| File | Description |
|------|-------------|
| `contract-template-nda-mutual.md` | Standard mutual NDA template |
| `contract-template-nda-one-way.md` | Standard one-way NDA template |
| `contract-template-service-agreement.md` | Standard professional services agreement template |
| `intake-scenarios.json` | 10 intake scenarios spanning all three tiers |
| `approval-gate-rules.md` | Complete rules for tier classification and routing |

## Suggested Approach

1. Design the intake questionnaire — what questions determine contract type, risk tier, and required terms?
2. Implement the approval gate classification as a dedicated step before generation
3. For Tier 1: populate the appropriate template and return the final contract
4. For Tier 2: generate the manager approval packet (brief + draft contract)
5. For Tier 3: generate the legal brief (risk summary + flagged draft)
6. Test with the provided scenarios — verify each scenario lands in the correct tier with an accurate explanation
7. Think about how to represent gate state: pending approval, approved, rejected, escalated

## Stretch Goals

- **Approval workflow simulation:** Build an interactive multi-turn flow where the approver can approve, reject, or request changes — and the system responds accordingly, including re-generating the contract after approved modifications
- **Counterparty redline handling:** When the other side proposes changes to the generated contract, evaluate each redline as: acceptable (within playbook, apply automatically), negotiable (triggers a Tier 2 re-gate for manager sign-off), or non-acceptable (triggers Tier 3 escalation to legal)
- **Contract status dashboard:** Track all in-flight contracts by tier, status, requester, and time-in-queue — surface SLA breaches (e.g., Tier 2 approval has been pending for >24 hours)
- **Structured legal brief generator:** For Tier 3 contracts, auto-generate a legal brief that includes a risk rating, key terms analysis, counterparty background, comparable past deals, and a recommended action with rationale
- **Gate refinement feedback loop:** After legal reviews a Tier 3 contract, capture whether it could have been handled at Tier 1 or 2 — log this feedback and identify patterns where the gate rules should be tightened or relaxed
