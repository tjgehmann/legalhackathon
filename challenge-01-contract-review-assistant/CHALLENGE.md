# Challenge 1: Contract Review Assistant

## The Problem

A legal team at a mid-size technology company reviews 40–60 vendor contracts per month. Each review takes 45–90 minutes. Many contracts contain similar issues — unfavorable liability caps, missing data protection clauses, auto-renewal traps, or non-standard termination terms.

Junior lawyers and paralegals spend hours on initial reviews that surface the same types of problems. Senior lawyers then re-review the flagged issues. The process is slow, inconsistent (different reviewers catch different things), and doesn't scale.

## Your Mission

Build an AI-powered contract review assistant that:

1. **Analyzes a vendor contract** and produces a structured review highlighting key risks, deviations from standard terms, and missing clauses
2. **Categorizes findings by severity** (high / medium / low risk)
3. **References specific clause numbers** so the reviewer can quickly navigate to the relevant section
4. **Suggests alternative language** where the contract deviates from the company's preferred position

## What Success Looks Like

- A legal professional uploads or pastes a contract and receives a structured, actionable review within seconds
- The review is consistent — running the same contract twice produces substantially the same output
- The output is useful enough that a junior lawyer can use it to prepare a first-pass review, saving 30–50% of review time
- The tool clearly distinguishes between critical issues (deal-breakers) and minor deviations

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `vendor-contract-saas-platform.md` | A SaaS platform agreement with several embedded risks |
| `vendor-contract-consulting-services.md` | A consulting services agreement with non-standard terms |
| `company-standard-positions.md` | The company's preferred contractual positions (your "benchmark") |

## Suggested Approach

1. Start by defining a system prompt that establishes the reviewer's role and the company's standard positions
2. Feed in a contract and ask for a structured review
3. Iterate on the output format until it's genuinely useful
4. Test with the second contract to see if the tool generalizes well
5. Consider building a reusable template or artifact that any team member could use

## Stretch Goals

- Add a "negotiation playbook" that suggests email language for pushing back on risky clauses
- Build a comparison mode that shows differences between two contract versions
- Create a dashboard view that summarizes the risk profile of a contract at a glance
