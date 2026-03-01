# Challenge 6: Legal Document Summarizer & Risk Flagger

## The Problem

Legal professionals and business leaders regularly need to digest lengthy legal documents — new regulations, court decisions, legislative changes, lengthy terms of service from partners, or multi-page internal policy drafts. A single regulatory update can be 80+ pages. A commercial lease might be 50 pages. An M&A due diligence report can run into hundreds of pages.

Reading every page carefully is ideal but often impractical given time constraints. Lawyers need to quickly understand:
- What does this document actually say? (the summary)
- What should I be worried about? (the risks)
- What do I need to do about it? (the action items)

Currently, junior associates or paralegals prepare manual summaries — a process that takes hours and still depends on the summarizer's experience to catch what matters.

## Your Mission

Build a legal document summarizer and risk flagger that:

1. **Produces a structured executive summary** of any legal document (regulation, contract, policy, court decision)
2. **Identifies and flags key risks** with severity ratings and explanations
3. **Extracts action items** — what needs to happen and by when
4. **Adapts the summary to the audience** — a summary for the CEO should look different from one for the compliance team
5. **Handles different document types** — regulations, contracts, court decisions, and internal policies

## What Success Looks Like

- A lawyer pastes a 30-page regulation and gets a 1-page executive summary, a risk table, and a prioritized action item list within minutes
- The summary captures the key points that an experienced lawyer would highlight
- Risks are categorized by severity and include specific references to the relevant sections
- Different audience modes produce appropriately tailored output (executive brief vs. detailed legal analysis)

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `regulation-eu-ai-act-excerpt.md` | An excerpt from EU AI Act provisions covering high-risk AI systems |
| `commercial-lease-agreement.md` | A 30-clause commercial office lease with embedded risks |
| `court-decision-data-privacy.md` | A fictional court decision on cross-border data transfers |
| `summary-templates.md` | Template structures for different summary types and audiences |

## Suggested Approach

1. Start with one document type (e.g., the regulation excerpt) and build a strong summary prompt
2. Add risk flagging with severity levels and section references
3. Add action item extraction
4. Test whether the same approach works for a different document type (e.g., the lease)
5. Add audience adaptation — let the user choose who the summary is for
6. Iterate on quality until the summaries are genuinely useful

## Stretch Goals

- Add a "compare documents" mode — summarize what changed between two versions of a policy or regulation
- Build a Q&A mode where the user can ask follow-up questions about the document
- Create a "regulatory impact assessment" template that maps regulation requirements to company functions
- Generate presentation slides from the summary for board or leadership meetings
