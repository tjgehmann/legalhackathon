# Challenge 10: The Regulatory Horizon Map

## The Problem

Executives are drowning in "regulation soup." The EU AI Act, GDPR, ESG disclosure requirements, the Digital Services Act, ePrivacy — the list keeps growing. Every time TechForward wants to launch a new product, expand into a new market, or add a data-driven feature, the legal team produces 30–50 pages of regulatory analysis. The executive team's eyes glaze over.

What leadership actually needs to know is simple: **"Can we launch this product in June? What could stop us? What do we need to do first?"** But that answer is buried under layers of legal detail, regulatory cross-references, and caveats.

The result: business decisions are delayed because leadership can't quickly assess the regulatory landscape. Legal analysis is thorough but not actionable at the executive level. Opportunities are missed because "legal is still reviewing," and sometimes products launch without proper regulatory clearance because teams bypass the process entirely.

## Your Mission

Build a Regulatory Horizon Map — a visual, executive-friendly decision support tool that:

1. **Transforms complex regulatory analysis into a Go/No-Go matrix** for a specific business initiative (e.g., launching a data-driven analytics service across the EU)
2. **Categorizes regulatory requirements as Deal Breakers, Managed Risks, or Clear to Proceed** — based on the company's risk appetite and the actual state of compliance
3. **Produces a visual "heat map"** of regulatory readiness across different dimensions (data privacy, AI regulation, sector-specific rules, cross-border requirements)
4. **Generates specific business actions** — not legal citations, but concrete steps like "Appoint a DPO in France before launch" or "Complete DPIA by May 15 to stay on track for June launch"

## What Success Looks Like

- An executive pastes or describes a business initiative and receives a clear, visual Go/No-Go assessment within seconds — not a 50-page memo
- The output clearly separates **Deal Breakers** (cannot launch until resolved) from **Managed Risks** (can launch if mitigated) from **Non-Issues** (already compliant or not applicable)
- Each flagged item has a concrete action, an owner suggestion, and a timeline — not just "comply with GDPR"
- A non-lawyer can look at the output and make a business decision: launch, delay, modify scope, or escalate to the board
- The tool adapts to different risk appetites (conservative, moderate, aggressive) and shows how the assessment changes

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `business-initiative-scenarios.json` | 4 business initiative scenarios with different regulatory profiles — from a straightforward EU SaaS launch to a high-risk AI-powered financial analytics product |
| `regulatory-landscape.json` | A structured database of regulatory requirements across GDPR, EU AI Act, DSA, ePrivacy, ESG, and sector-specific rules, with applicability triggers and compliance effort estimates |
| `company-compliance-status.md` | TechForward's current compliance posture — what's already in place, what's in progress, and what's missing |
| `risk-appetite-profiles.md` | Three risk appetite profiles (Conservative, Moderate, Aggressive) with decision thresholds and escalation criteria |

## Suggested Approach

1. Study the regulatory landscape database and understand how requirements are triggered by business characteristics
2. Pick one business initiative scenario and map applicable regulations
3. Build a prompt that categorizes each requirement into Deal Breaker / Managed Risk / Clear
4. Design a visual output — a heat map, traffic-light matrix, or dashboard — that an executive could read in under 2 minutes
5. Add action items with owners and deadlines for each flagged requirement
6. Test across multiple scenarios and risk appetite profiles to verify the tool adapts correctly

## Stretch Goals

- Build a timeline view showing what must happen by when to hit a target launch date
- Add a cost/effort estimator for achieving compliance (e.g., "DPIA completion: ~2 weeks, EUR 15K external cost")
- Create a comparison mode showing regulatory requirements across different launch geographies side-by-side
- Implement a "what-if" mode: "What changes if we exclude AI-based profiling from the product?"
