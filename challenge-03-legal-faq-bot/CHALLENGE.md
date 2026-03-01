# Challenge 3: Legal FAQ Bot for Non-Legal Teams

## The Problem

The legal team receives dozens of Slack messages and emails every week with questions like:

- *"Can we use this stock photo on our website?"*
- *"Do we need a DPA with this vendor?"*
- *"Can I share this customer data with our partner?"*
- *"What's our policy on employee referral bonuses?"*
- *"Is it okay to use open-source software in our product?"*

Most of these questions have straightforward answers based on existing company policies. But finding those answers requires digging through a 200-page policy handbook, scattered wiki pages, and tribal knowledge. So people default to asking legal directly — and legal spends hours per week answering the same questions repeatedly.

## Your Mission

Build an AI-powered legal FAQ bot that:

1. **Answers common legal questions** based on the company's existing policies and guidelines
2. **Cites the specific policy or guideline** it's referencing in each answer
3. **Knows its limits** — clearly indicates when a question falls outside its knowledge and should be escalated to a human lawyer
4. **Uses plain language** — the audience is non-lawyers, so answers should be clear, practical, and jargon-free

## What Success Looks Like

- A marketing manager asks *"Can we use a customer's logo on our website?"* and gets a clear, policy-backed answer in seconds
- The bot points to the exact section of the relevant policy
- When asked something ambiguous or high-stakes (*"Can we terminate this employee?"*), the bot declines to answer and recommends contacting legal
- Answers are consistent — the same question always gets substantially the same answer

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `company-legal-policies.md` | Consolidated company policies covering IP, data privacy, contracts, employment, and compliance |
| `frequently-asked-questions.json` | 20 real-world questions that employees have asked the legal team, with expected answers |
| `escalation-topics.md` | Topics and question patterns that should always be escalated to human lawyers |

## Suggested Approach

1. Upload the company policies as your knowledge base
2. Write a system prompt that defines the bot's role, tone, and escalation rules
3. Test with the provided FAQ list — does the bot give correct, policy-backed answers?
4. Refine the prompt to handle edge cases and ambiguous questions
5. Consider building this as a conversational interface (follow-up questions, clarifications)

## Stretch Goals

- Add a confidence score to each answer (*"I'm 90% confident based on Section 4.2 of the Data Privacy Policy"*)
- Build a feedback mechanism where users can flag incorrect answers for legal review
- Create a "question log" that helps legal identify which policies need to be clarified or updated
- Support multiple languages for international teams
