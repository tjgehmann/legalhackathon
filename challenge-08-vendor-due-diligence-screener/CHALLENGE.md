# Challenge 8: Vendor Due Diligence Screener

## The Problem

Before onboarding a new vendor, supplier, or business partner, companies are legally required to perform due diligence screening. This means checking the entity and its key individuals against government-issued sanctions lists, watchlists, and adverse media — including lists from the EU, the US (OFAC), the UN, and the German Federal Office of Economics and Export Control (BAFA).

Today, this process is painful. Compliance officers manually search multiple databases, cross-reference names (accounting for spelling variations, transliterations, and aliases), review results for false positives, and document their findings. A single screening can take 30–60 minutes, and the company onboards 15–25 new vendors per month. When screening is delayed, business deals stall. When it's rushed, risks are missed.

The legal and compliance team needs a faster, more reliable way to screen vendors — one that reduces false positives, explains *why* a match was flagged, and produces audit-ready documentation.

## Your Mission

Build an AI-powered vendor due diligence screener that:

1. **Takes vendor information as input** (company name, country, key individuals, industry sector) and screens it against provided sanctions and watchlist data
2. **Identifies potential matches** using intelligent name matching that accounts for spelling variations, abbreviations, transliterations, and aliases
3. **Classifies results** as confirmed match, potential match (needs review), or no match — with clear explanations for each classification
4. **Generates an audit-ready screening report** documenting the search performed, lists checked, results found, and recommended next steps

## What Success Looks Like

- A compliance officer enters vendor details and receives a structured screening report within seconds
- The tool correctly identifies true matches while minimizing false positives (e.g., "Al-Rashid Trading LLC" should match a sanctioned entity "Al Rashid Trading Co." but not "Rashid's Restaurant")
- Each flagged result includes a clear explanation of *why* it was flagged and *which list* it appeared on
- The screening report is detailed enough to satisfy auditors and regulators — documenting what was searched, when, and what was found

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `sanctions-watchlist-data.json` | A consolidated sanctions/watchlist dataset with entries from EU, OFAC, UN, and German sources (fictional but realistic) |
| `vendor-screening-requests.json` | 8 vendor screening scenarios covering clean vendors, sanctioned entities, close-name matches, and edge cases |
| `screening-report-template.md` | A template for structuring the screening report with all required compliance documentation fields |

## Suggested Approach

1. Study the sanctions/watchlist data structure to understand the types of entries and identifying information available
2. Design a vendor intake form that captures the key information needed for screening
3. Build a prompt that performs intelligent name matching and cross-referencing against the watchlist data
4. Iterate on match classification — getting the right balance between catching real matches and filtering false positives is key
5. Test with all 8 vendor scenarios to verify accuracy across different match types

## Stretch Goals

- Add adverse media screening — generate search queries and analyze news results for negative coverage about a vendor
- Build a risk scoring model that combines sanctions screening with other risk factors (country risk, industry risk, transaction size)
- Create a re-screening workflow that flags when previously cleared vendors appear on newly updated lists
- Implement PEP (Politically Exposed Person) screening for key individuals associated with the vendor
