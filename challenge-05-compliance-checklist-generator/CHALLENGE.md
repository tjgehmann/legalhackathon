# Challenge 5: Compliance Checklist Generator

## The Problem

When teams across the company launch new products, enter new markets, run marketing campaigns, or onboard vendors, they often need to comply with a patchwork of legal and regulatory requirements. But figuring out *which* requirements apply is half the battle.

Today, teams either:
- Ask legal for a compliance review (adding weeks to their timeline)
- Try to figure it out themselves and miss something important
- Skip the compliance step entirely and hope for the best

The legal team has documented compliance requirements in various places — regulatory guides, internal wikis, past project checklists — but there's no easy way for a non-lawyer to determine: *"For MY specific project, what do I need to do?"*

## Your Mission

Build a compliance checklist generator that:

1. **Asks targeted questions** about a project or initiative (type, scope, geographies, data involved, audience, etc.)
2. **Generates a tailored compliance checklist** based on the answers — not a generic list, but requirements specific to that project
3. **Explains each requirement in plain language** — why it matters and what the team needs to do
4. **Categorizes requirements by priority** (must-do before launch vs. should-do vs. nice-to-have)
5. **Identifies items that require legal sign-off** vs. items the team can self-certify

## What Success Looks Like

- A product manager planning a new feature that collects user data in the EU gets a specific checklist covering GDPR consent, privacy notice updates, DPIA requirements, and data retention
- A marketing team planning an email campaign gets a checklist covering CAN-SPAM/GDPR marketing consent, unsubscribe requirements, and data usage limitations
- Each checklist item includes a plain-English explanation and a clear action step
- The tool distinguishes between "you can handle this yourself" and "you need legal to review this"

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `compliance-requirements-database.json` | A structured database of compliance requirements organized by category, regulation, and trigger conditions |
| `project-scenarios.json` | 6 sample project scenarios to test the generator |
| `regulatory-summaries.md` | Plain-language summaries of key regulations (GDPR, CAN-SPAM, CCPA, SOX, AML/KYC) |

## Suggested Approach

1. Study the compliance requirements database to understand the structure
2. Design an intake questionnaire that captures the right information to filter requirements
3. Build a prompt that maps project characteristics to applicable requirements
4. Generate a clear, actionable checklist with priorities and explanations
5. Test with the provided scenarios to ensure the right requirements surface for each case

## Stretch Goals

- Add jurisdiction-specific guidance (different requirements for EU, US, UK, APAC)
- Build a progress tracker so teams can mark items as complete and share status with legal
- Generate a "compliance summary memo" that the team can attach to their project documentation
- Include links to relevant policy documents and templates for each checklist item
