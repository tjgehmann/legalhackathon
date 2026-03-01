# Challenge 2: Self-Service NDA Generator

## The Problem

The sales and business development teams at a growing company need NDAs signed before nearly every new business conversation. Currently, the process looks like this:

1. Sales rep emails the legal team: *"Need an NDA for a meeting next Tuesday with Acme Corp"*
2. Legal asks clarifying questions: *"Mutual or one-way? What's the scope? Any special requirements?"*
3. Back-and-forth over 2–3 days
4. Legal sends a draft
5. The counterparty requests changes
6. More back-and-forth

Average turnaround: **5 business days** for a document that is 90% boilerplate. Legal spends an estimated 15% of their time on NDA-related tasks that could be standardized.

## Your Mission

Build a self-service NDA generator that allows non-legal team members to:

1. **Answer a simple set of questions** (who's the counterparty, what's the purpose, mutual or one-way, duration, etc.)
2. **Generate a ready-to-send NDA** based on pre-approved templates and the company's standard terms
3. **Handle common variations** (mutual vs. one-way, different jurisdictions, different confidentiality periods)
4. **Flag edge cases** that should be escalated to legal (e.g., counterparty is a government entity, involves highly regulated data, or the deal value exceeds a threshold)

## What Success Looks Like

- A sales rep can generate a compliant NDA in under 5 minutes without contacting legal
- The generated NDA uses approved language — legal is comfortable with every version it produces
- Edge cases are properly identified and routed to legal instead of being handled by the tool
- The output is a clean, professional document ready to send to the counterparty

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `nda-template-mutual.md` | Company's standard mutual NDA template |
| `nda-template-one-way.md` | Company's standard one-way (disclosing party) NDA template |
| `intake-scenarios.json` | 8 sample intake scenarios with different parameters |
| `escalation-rules.md` | Rules for when an NDA request should be escalated to legal |

## Suggested Approach

1. Design the intake questionnaire — what questions does the tool need to ask?
2. Map answers to template variations
3. Build a prompt that assembles the right NDA based on the inputs
4. Test with the provided scenarios to make sure edge cases get flagged
5. Consider building an interactive form (Claude artifact, Google Form, etc.)

## Stretch Goals

- Add counterparty markup handling — when the other side proposes changes, the tool evaluates whether they're acceptable
- Generate a cover email to send along with the NDA
- Track NDA status (sent, signed, expired) in a simple spreadsheet or dashboard
