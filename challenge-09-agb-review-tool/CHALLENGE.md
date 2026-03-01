# Challenge 9: AGB & Einkaufsbedingungen Review Tool

## The Problem

German businesses constantly deal with Allgemeine Geschäftsbedingungen (AGB — general terms and conditions) and Einkaufsbedingungen (purchasing terms) from suppliers, vendors, and service providers. Under German law, many common clauses in AGB are subject to strict statutory limits set out in §§ 305–310 BGB (Bürgerliches Gesetzbuch). Clauses that deviate too far from these statutory defaults can be legally void — even if both parties signed the contract.

Today, reviewing AGB and Einkaufsbedingungen is a tedious, specialized task. A lawyer must read through pages of dense legal German, mentally map each clause to the relevant BGB provisions, assess whether the clause deviates from the statutory default, and determine whether that deviation is permissible or likely void under the AGB-Kontrolle (judicial review of standard terms). This takes 1–3 hours per set of terms and requires deep familiarity with German civil law and the extensive case law around § 307 BGB (the "reasonableness test").

The result: reviews pile up, business teams wait days for feedback on vendor terms, and sometimes terms are accepted without proper review because the legal team is overloaded.

## Your Mission

Build an AI-powered AGB and Einkaufsbedingungen review tool that:

1. **Analyzes a set of AGB or Einkaufsbedingungen** clause by clause and maps each to the relevant BGB provisions
2. **Identifies deviations from statutory defaults** (gesetzliche Regelung) and assesses whether each deviation is likely permissible, risky, or void under AGB-Kontrolle
3. **Flags specific risks** with a severity rating (high / medium / low) and explains in plain language why a clause is problematic
4. **Suggests alternative language** that would bring problematic clauses closer to a legally compliant and balanced position

## What Success Looks Like

- A lawyer or procurement manager pastes a set of AGB or Einkaufsbedingungen and receives a structured clause-by-clause review within seconds
- Each clause is mapped to the relevant BGB section (e.g., "This limitation of liability clause relates to § 309 Nr. 7 BGB")
- The tool correctly identifies clauses that are likely void under the AGB-Kontrolle (e.g., a blanket exclusion of liability for gross negligence)
- The risk assessment is nuanced — distinguishing between B2B and B2C applicability and noting where case law is unsettled
- Business stakeholders can understand the summary and know which terms to push back on during negotiations

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `bgb-agb-recht-reference.md` | A structured reference of key BGB provisions (§§ 305–310) governing AGB, including the statutory defaults and judicial review standards |
| `vendor-agb-it-services.md` | A complete set of AGB from a fictional IT services provider, containing several problematic clauses |
| `einkaufsbedingungen-manufacturing.md` | Purchasing terms from a fictional manufacturing company with deviations from standard BGB provisions |
| `review-scenarios.json` | 6 specific clause scenarios with expected assessments to test the tool's accuracy |

## Suggested Approach

1. Study the BGB reference to understand the statutory framework for AGB-Kontrolle
2. Feed in a set of AGB and ask the AI to perform a clause-by-clause analysis
3. Build a prompt that maps clauses to BGB provisions and assesses permissibility
4. Iterate on the risk assessment — the key challenge is distinguishing between permissible deviations and void clauses
5. Test with both the IT services AGB and the manufacturing Einkaufsbedingungen to verify the tool works across different industries and term types

## Stretch Goals

- Add a B2B vs. B2C toggle that adjusts the analysis based on whether stricter consumer protection rules apply (§ 310 Abs. 1 BGB)
- Build a clause comparison mode that shows deviations side-by-side with the statutory default
- Create a negotiation brief that prioritizes which clauses to push back on and suggests specific redline language
- Implement a "clause health score" that gives an overall risk rating for a complete set of AGB
