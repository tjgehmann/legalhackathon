# Challenge 16: AI-Powered Negotiation Preparation Tool

## The Problem

Contract negotiations are won or lost before the first meeting. Yet most lawyers walk in with only their own positions prepared — without a clear view of their BATNA, a realistic ZOPA, or a structured read of what the counterparty actually needs (as opposed to what they're asking for).

The result: negotiations stall on positions rather than interests, deals collapse that didn't need to, and lawyers either give up too much or hold out too long because they never mapped the full space of possible agreement.

## Your Mission

Build an AI-powered negotiation preparation tool that helps a lawyer or deal team:

1. **Map their own position** — clarify their opening ask, target, and walk-away point for each key issue
2. **Identify their BATNA** (Best Alternative to a Negotiated Agreement) — what happens if no deal is reached, and how strong is that alternative?
3. **Estimate the ZOPA** (Zone of Possible Agreement) — based on what's known about the counterparty, where do the acceptable ranges overlap?
4. **Surface the counterparty's real interests** — go beyond stated positions to ask: what outcome does the other side actually need? What constraints are they under? What would a win look like for them?
5. **Generate a negotiation strategy** — recommend tactics, sequencing, concession patterns, and potential value-creating trades based on principled negotiation best practices

## Core Concepts to Build Around

### BATNA (Best Alternative to a Negotiated Agreement)
Your BATNA is your best option if negotiations fail. The stronger your BATNA, the more leverage you have. The tool should help the user articulate:
- What they will do if no deal is reached
- How attractive that alternative really is (honestly)
- Whether steps could be taken to strengthen the BATNA before or during negotiations

### ZOPA (Zone of Possible Agreement)
The ZOPA is the range between each party's reservation point — the minimum acceptable outcome for each side. A deal is only possible if this zone exists. The tool should help the user:
- Define their own reservation point (walk-away threshold) for each issue
- Estimate the counterparty's likely reservation point based on available information
- Visualize whether and where a ZOPA exists

### Interests vs. Positions
Positions are what parties say they want ("We need 90-day payment terms"). Interests are why they want it ("Our cash flow is tight in Q4"). The tool should prompt users to dig beneath surface demands — both their own and the counterparty's — to identify trades that satisfy underlying interests even when stated positions appear incompatible.

### Principled Negotiation (Fisher & Ury)
The tool should apply the core principles from *Getting to Yes*:
- Separate the people from the problem
- Focus on interests, not positions
- Invent options for mutual gain
- Insist on objective criteria

## What Success Looks Like

- A lawyer inputs key deal parameters and counterparty context, and receives a structured negotiation brief within minutes
- The brief clearly maps the ZOPA for each negotiated issue
- The tool surfaces at least 3 potential "value trades" — areas where the parties can give on something they value less in exchange for something they value more
- A junior associate can use it to prepare a negotiation brief that a partner finds genuinely useful
- The output includes a concession strategy: what to offer first, what to hold back, and at what point to walk away

## Mock Data Provided

In the `mock-data/` folder you'll find:

| File | Description |
|------|-------------|
| `negotiation-scenario-saas-renewal.md` | A SaaS contract renewal negotiation with known positions on both sides |
| `counterparty-intelligence-brief.md` | Background on the counterparty company, their business context, and known constraints |
| `negotiation-prep-template.md` | A blank preparation worksheet to fill in with AI assistance |

## Suggested Approach

### Option A: Guided Negotiation Prep Assistant (no code)
Build a structured prompt or prompt chain that walks the user through:
1. Defining their issues and positions
2. Stress-testing their BATNA
3. Estimating the counterparty's interests and constraints
4. Generating a ZOPA map and strategy brief

This can be delivered as a polished prompt, a Claude artifact, or a reusable template.

### Option B: Interactive Web Tool (with Claude Code or Antigravity)
Build a form-based web app where the user inputs deal parameters and receives a structured negotiation brief. Consider:
- An intake form with fields for each negotiation issue (user's ask, target, walk-away, BATNA)
- A section for counterparty analysis (industry, business pressure, known constraints)
- An AI-generated output section with ZOPA visualization, interest analysis, and strategy recommendations

### Option C: Negotiation Simulation (stretch goal)
Build a tool that simulates the counterparty's responses based on their likely interests, allowing the user to practice negotiation moves before the real meeting.

## Prompt Starter

```
You are an expert negotiation advisor trained in principled negotiation (Fisher & Ury) and deal strategy.

A lawyer is preparing for a contract negotiation. Your job is to help them:
1. Clarify their BATNA and assess how strong it truly is
2. Define their reservation point (walk-away threshold) for each issue
3. Estimate the counterparty's interests, constraints, and likely reservation points
4. Map the ZOPA — where does a mutually acceptable zone of agreement exist?
5. Generate a strategy: opening moves, value trades, concession sequencing, and red lines

Be direct. Challenge assumptions. If the user's stated BATNA is weak, say so and suggest how to strengthen it. 
If their opening position is unrealistic, explain why and propose an adjustment.
Focus on interests, not just positions.

Start by asking the user to describe: (1) what they're negotiating, (2) the key issues, and (3) what happens if no deal is reached.
```

## Stretch Goals

- Add a **pre-mortem feature**: "If this negotiation fails, what's the most likely reason?" — forces the user to think through failure modes in advance
- Build a **real-time concession tracker**: as the negotiation progresses, log concessions made and received to maintain a live view of the deal's balance
- Add a **cultural intelligence layer**: flag negotiation style differences for cross-border deals (e.g., high-context vs. low-context communication, relationship vs. transaction orientation)
- Generate a **BATNA improvement plan**: specific steps the user can take before the negotiation to strengthen their outside option
