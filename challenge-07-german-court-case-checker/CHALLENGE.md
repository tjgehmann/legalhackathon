# Challenge 7: German Court Case Checker

## The Problem

A corporate legal team at a mid-size technology company operating in Germany regularly needs to stay on top of court decisions that could affect their business. Relevant rulings come from multiple levels of the German court system — the Bundesgerichtshof (BGH), Oberlandesgerichte (OLG), Landgerichte (LG), and specialized courts like the Bundesarbeitsgericht (BAG) or Bundesfinanzhof (BFH).

Today, tracking relevant case law is a manual, time-consuming process. Lawyers browse legal databases, read newsletters, and scan dozens of decisions each month, most of which turn out to be irrelevant. When they *do* find a relevant decision, there's no structured way to assess its business impact, link it to existing contracts or policies, or alert the right internal stakeholders.

The result: important rulings get missed, legal advice is sometimes based on outdated precedent, and the team spends hours on research that could be dramatically accelerated.

## Your Mission

Build an AI-powered German court case checker that:

1. **Analyzes court decisions** and extracts the key holdings, legal principles, and practical implications in plain language
2. **Matches decisions to business-relevant topics** — given a company profile (industry, contract types, key legal areas), identifies which recent decisions are relevant and why
3. **Rates the business impact** of each relevant decision (high / medium / low) and explains what the company should do in response
4. **Generates actionable alerts** summarizing relevant decisions for different internal audiences (legal team, management, contract managers)

## What Success Looks Like

- A legal professional pastes or uploads a court decision and receives a structured analysis within seconds — no need to read the full 20-page ruling
- The tool correctly identifies whether a decision is relevant to the company's business areas and explains why (or why not)
- The output distinguishes between decisions that require immediate action (e.g., a clause in standard contracts is now unenforceable) and those that are good to know
- Non-lawyers in the business can understand the alert summaries and know whether they need to take action

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `company-legal-profile.md` | The company's industry, key legal areas, contract types, and business activities — the "lens" for relevance matching |
| `court-decisions.json` | 8 fictional German court decisions from various courts (BGH, OLG, LG, BAG) with full metadata and summaries |
| `relevance-assessment-template.md` | A template for structuring the relevance assessment and business impact analysis |

## Suggested Approach

1. Start by studying the company legal profile to understand what topics matter
2. Feed in a court decision and ask the AI to extract key holdings and legal principles
3. Build a prompt that assesses relevance against the company profile
4. Iterate on the output format until it's useful for both lawyers and business stakeholders
5. Test across all 8 sample decisions to verify the tool correctly distinguishes relevant from irrelevant cases

## Stretch Goals

- Build a "case law radar" dashboard that visualizes relevant decisions by topic, court level, and impact
- Add a feature that links relevant decisions to specific clauses in the company's standard contracts
- Create a weekly digest generator that summarizes the most important new decisions
- Implement trend detection — flag when multiple courts are ruling similarly on an issue, signaling a legal trend
