# Challenge 4: Clause Library & Comparison Tool

## The Problem

Over the years, the legal team has negotiated hundreds of contracts. Buried in those contracts are battle-tested clause variations for every situation — strong indemnification language that a tough counterparty accepted, creative limitation-of-liability carve-outs, GDPR-compliant data processing terms that actually work.

But this knowledge lives in individual lawyers' heads and in contract files scattered across SharePoint, email, and the contract management system. When drafting a new contract, lawyers either:

- Start from the standard template (which may not fit the situation)
- Try to remember which past deal had the right language (unreliable)
- Spend 30+ minutes searching through old contracts (slow)

There's no organized, searchable library of approved clause alternatives.

## Your Mission

Build a clause library and comparison tool that:

1. **Organizes clauses by category** (indemnification, liability, termination, IP, data protection, etc.)
2. **Provides multiple variations** for each clause type, from most company-favorable to most counterparty-favorable
3. **Compares a proposed clause** against the library to assess where it falls on the spectrum
4. **Recommends alternatives** when a proposed clause is unfavorable, with context on when each alternative was successfully used

## What Success Looks Like

- A lawyer pastes a limitation-of-liability clause from a counterparty's paper and instantly sees how it compares to the company's standard positions
- The tool suggests 2–3 alternative formulations ranked from strongest to most concession-friendly
- Each alternative includes context: *"This version was accepted by [type of counterparty] in [type of deal]"*
- New clauses from completed negotiations can be added to the library over time

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `clause-library.json` | A structured library of 25+ clause variations across 6 categories |
| `sample-clauses-to-analyze.md` | 5 clauses from counterparty contracts to test the comparison feature |
| `clause-categories.md` | Definitions and explanations for each clause category |

## Suggested Approach

1. Start by organizing the clause library data into a format the AI can reference effectively
2. Build a comparison prompt that takes a new clause and evaluates it against the library
3. Add context-aware recommendations — not just "this is bad" but "here's what to use instead and why"
4. Test with the sample clauses to refine the analysis quality
5. Consider building a searchable interface or interactive artifact

## Stretch Goals

- Add a "negotiation history" that shows which clause positions tend to be accepted by different types of counterparties
- Build a clause scoring system (1–10) that quantifies how favorable a clause is
- Create a "clause builder" that assembles a full contract section from selected clause components
- Generate redline suggestions that show exactly what to change in a proposed clause
