# Challenge 11: Contract Bottleneck & Deal Velocity Dashboard

## The Problem

At TechForward, the average sales contract takes 23 days from "terms sent" to "signature received." Every day a contract sits in the legal review queue is a day of lost revenue. The sales team calls Legal the "Department of No." The CFO sees a black hole between "deal agreed" and "revenue recognized."

The frustrating part: 80% of the delays come from the same 5–6 negotiation points. Customers push back on liability caps, want different data processing terms, reject auto-renewal clauses, or insist on their own governing law. Legal spends hours negotiating the same issues on every deal, often reaching the same compromises. Meanwhile, executives sign contracts without reading them because the stack is too thick and they trust that "legal reviewed it."

The company needs two things: (1) a way to identify and eliminate recurring bottlenecks, and (2) an executive-friendly contract summary that lets leadership sign with confidence in seconds instead of wading through 40 pages.

## Your Mission

Build a Contract Bottleneck & Deal Velocity Dashboard that:

1. **Analyzes contract negotiation data** to identify the top negotiation points that cause the most delays and proposes a "Standardized Acceptable Risk" (SAR) policy for each
2. **Calculates the revenue impact** of contract delays — translating days-in-queue into lost cash flow and delayed revenue recognition
3. **Generates an executive contract summary** that highlights *only* the deviations from company standard positions, enabling an executive to review and approve in under 60 seconds
4. **Recommends process improvements** — which terms should be pre-approved, which require legal review, and which are deal-breakers requiring escalation

## What Success Looks Like

- A sales leader can see at a glance which negotiation issues are slowing deals and by how much
- The tool produces a clear SAR policy: "For deals under EUR 500K, accept the customer's liability cap if it's at least 2x annual contract value" — eliminating back-and-forth on routine issues
- An executive receives a one-page contract summary showing: deal value, term, key deviations from standard, risk rating, and recommended action (sign / escalate / reject)
- The dashboard quantifies the ROI of standardization: "Reducing average negotiation time by 4 days would accelerate EUR 2.3M in quarterly revenue"
- Legal can use the analysis to proactively update standard templates based on what customers actually negotiate

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `contract-negotiation-log.json` | Negotiation history for 20 recent deals showing which clauses were negotiated, time spent, outcomes, and deal values |
| `company-standard-terms.md` | TechForward's standard contract positions across key clause categories |
| `sample-contracts-for-summary.json` | 4 fully negotiated contracts ready for executive summary generation — each with different risk profiles |
| `revenue-impact-data.json` | Financial data linking contract cycle times to revenue recognition, pipeline velocity, and quarterly targets |

## Suggested Approach

1. Analyze the negotiation log to identify patterns — which clauses get negotiated most, which cause the longest delays, and what the typical compromise looks like
2. Build a bottleneck analysis that ranks issues by frequency and delay impact
3. For each top bottleneck, draft a SAR policy defining pre-approved acceptable ranges
4. Design an executive contract summary format that shows only what matters: deviations, risks, and a sign/escalate/reject recommendation
5. Calculate the revenue impact of current delays and model the improvement from SAR policies
6. Test the executive summary generator with the sample contracts

## Stretch Goals

- Build a "deal velocity predictor" that estimates how long a specific contract will take based on the counterparty's initial redlines
- Add a negotiation playbook recommending specific counter-proposals for common pushback
- Create a quarterly trend report showing whether contract cycle times are improving or worsening
- Implement a "fast-track" classifier that identifies deals that can skip legal review entirely based on SAR policies
