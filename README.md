# Legal Hackathon: Build the Future of Legal Work — Today

> **You don't need to be a developer. You just need curiosity and a problem worth solving.**

Welcome! Today is your day to experiment, explore, and experience firsthand what AI can do for legal work. This is not a coding exam. It's a playground. There are no wrong answers, no failed attempts — only learning and building.

So take a deep breath, pick a challenge that excites you, and let's have fun.

---

## What Is This Hackathon About?

Legal teams deal with a daily overload of repetitive, time-consuming work — contract reviews, compliance checks, policy questions, document summaries. And when deals need to be won, lawyers sit across the table from counterparties without a structured read of the other side's real interests, a clear BATNA, or a mapped-out ZOPA. At the same time, AI tools have reached a point where they can genuinely help with all of this, right now, today, without writing a single line of code.

This hackathon gives you a structured day to **explore that potential hands-on**. Pick a real-world legal challenge, use the AI tools available to you, and build something — anything — that demonstrates an idea worth sharing.

---

## Every Output Counts

Here's the most important thing to understand: **there is no single correct format for your deliverable.**

You don't need to build a working app. You don't need to write code. What matters is that you explored a challenge, used AI tools to tackle it, and have something to show.

Accepted outputs include — but are not limited to:

| Format | What it looks like |
|--------|--------------------|
| **PowerPoint / Slides** | A presentation walking through the problem, your approach, and a demo of your AI interactions |
| **Process Description** | A written or visual description of how an AI-powered workflow would work in practice |
| **Prompt Prototype** | A polished, well-documented prompt (or prompt chain) that reliably solves the challenge |
| **MVP / Working Demo** | A simple app, form, or interactive tool built with AI assistance |
| **Working Paper** | A structured analysis of the challenge with AI-generated content, findings, and recommendations |
| **Hybrid** | Any combination of the above — a slide deck with a live demo, a working paper with an embedded prototype, etc. |

The goal is to **think, experiment, and learn** — not to ship production software.

---

## The Tools at Your Disposal

You have access to incredibly powerful AI tools today. Here's how to use each one:

---

### Claude Code — Desktop App or IDE Extension

**Claude Code** is Anthropic's AI coding agent that can build entire applications through conversation. You don't need to know how to code — you describe what you want, and Claude builds it.

**Two ways to use it:**

**Desktop App** — Download from [claude.ai/download](https://claude.ai/download). Open a folder, describe your idea, and Claude writes the code, runs it, fixes errors, and iterates — all from a simple chat interface.

**IDE Extension** — If you have VS Code or a JetBrains IDE, install the Claude Code extension. Claude works alongside you in your editor, reading and writing files, running tests, and explaining every step.

**What you can build with Claude Code:**
- A web app that lets users upload a contract and get an instant risk summary
- A form-based NDA generator that produces a ready-to-send PDF
- An interactive checklist tool for compliance workflows
- A document classifier that sorts and tags uploaded legal files

**Getting started:** Just say what you want to build. For example:
> *"Build a simple web app where I can paste a contract and get a structured review of liability clauses, data privacy risks, and missing standard terms. Make it look professional and easy to use."*

---

### Claude — Web App with Artifacts

**[claude.ai](https://claude.ai)** — The browser-based Claude is perfect for document analysis, legal reasoning, and building interactive artifacts without installing anything.

**What makes it great for this hackathon:**
- Upload contracts, PDFs, and documents and chat with them directly
- Create **Artifacts** — live HTML/CSS/JavaScript apps that run right in the browser
- Use **Projects** to store documents and maintain context across multiple conversations
- Extended thinking mode for deep multi-step analysis

**Ideas:**
- Paste a contract and ask Claude to generate a structured risk table
- Ask Claude to build a working HTML form for an NDA generator — it runs live in the chat
- Use Projects to upload all your mock data files, then query them in one conversation

---

### Antigravity — No-Code App Builder

**Antigravity** is a no-code platform that lets you build and deploy real web applications through conversation — no installation, no setup, no code.

**Why use it:** If you want a polished, shareable prototype that looks like a real product, Antigravity is the fastest path. Describe your legal tool, and it builds, styles, and hosts the app for you.

**Ideas:**
- A branded contract review dashboard with a file upload and analysis panel
- A self-service NDA generator with a clean intake form
- An internal legal FAQ chatbot with a chat interface

**Getting started:** Describe your vision in plain language:
> *"Build a legal FAQ tool for HR teams. They should be able to type a question about employment law, and get a clear, plain-language answer. The interface should be simple and professional."*

---

### Gemini Canvas — Google's Interactive AI Workspace

**[gemini.google.com](https://gemini.google.com)** with the **Canvas** feature gives you an interactive document editor powered by AI.

**What makes it great:**
- Canvas lets you collaboratively draft, edit, and refine documents with AI in real time
- Native integration with Google Docs and Sheets
- Great for producing polished written deliverables: playbooks, policy documents, working papers
- Can generate and run code snippets inside the canvas

**Ideas:**
- Draft a complete sales contract playbook with AI — then refine it clause by clause in Canvas
- Create a compliance checklist document that auto-populates based on user inputs
- Build a regulatory summary document and iterate on the structure with Gemini

---

## General Tips: How to Get the Most Out of AI Tools

These tips work regardless of which tool you use:

### 1. Start with a system prompt
Before asking your first question, set the context. Tell the AI who it is and what it should do:
```
You are a contract review assistant for a mid-size technology company in Germany.
Your role is to review vendor contracts and flag:
- Unusual liability or indemnification clauses
- Missing standard protections (IP ownership, confidentiality, limitation of liability)
- Terms that deviate from our standard positions
Always output findings as a structured table with: Clause | Risk Level | Recommendation
```

### 2. Upload your mock data
Every challenge folder contains realistic mock data — contracts, templates, case files. Upload them directly into your AI tool. The more context the AI has, the better the output.

### 3. Iterate, don't restart
If the output isn't quite right, tell the AI what to improve:
> *"The liability analysis is too vague. Be more specific about which party bears the risk and cite the exact clause number."*

### 4. Break complex tasks into steps
Instead of *"Review this entire contract"*, try:
- Step 1: *"Extract all clauses related to liability and indemnification"*
- Step 2: *"Assess each clause: does it favor us, the vendor, or is it neutral?"*
- Step 3: *"Flag clauses that deviate from German market standard terms"*

### 5. Ask for structured output
AI tools produce more useful results when you specify the format:
> *"Output your findings as a table with columns: Clause Number | Topic | Risk Level | Our Recommendation"*

### 6. Use AI to help you use AI
If you're stuck, just ask:
> *"Help me write a system prompt for an NDA generator that works for a German company"*
> *"What's the best way to structure a prompt for comparing two contract versions?"*

### 7. Combine tools
There's no rule that says you have to use only one tool. You might:
- Use **Claude** to analyze a contract and extract key clauses
- Use **Gemini Canvas** to turn those findings into a polished report
- Use **Claude Code** or **Antigravity** to wrap it all in a working web interface

---

## The Challenges

Each challenge has its own folder with a detailed brief and mock data. Pick the one that excites your team most — or come up with your own variation.

| # | Challenge | Who Benefits | Folder |
|---|-----------|-------------|--------|
| 1 | **Contract Review Assistant** | Legal teams | [challenge-01](./challenge-01-contract-review-assistant/) |
| 2 | **Self-Service NDA Generator** | Sales, Partnerships | [challenge-02](./challenge-02-self-service-nda-generator/) |
| 3 | **Legal FAQ Bot for Non-Legal Teams** | All departments | [challenge-03](./challenge-03-legal-faq-bot/) |
| 4 | **Clause Library & Comparison Tool** | Legal teams | [challenge-04](./challenge-04-clause-library/) |
| 5 | **Compliance Checklist Generator** | Product, Marketing, HR | [challenge-05](./challenge-05-compliance-checklist-generator/) |
| 6 | **Legal Document Summarizer & Risk Flagger** | Legal, Management | [challenge-06](./challenge-06-legal-document-summarizer/) |
| 7 | **German Court Case Checker** | Legal teams, Management | [challenge-07](./challenge-07-german-court-case-checker/) |
| 8 | **Vendor Due Diligence Screener** | Compliance, Procurement | [challenge-08](./challenge-08-vendor-due-diligence-screener/) |
| 9 | **AGB & Einkaufsbedingungen Review Tool** | Legal, Procurement | [challenge-09](./challenge-09-agb-review-tool/) |
| 10 | **Regulatory Horizon Map** | Executives, Legal | [challenge-10](./challenge-10-regulatory-horizon-map/) |
| 11 | **Contract Bottleneck & Deal Velocity Dashboard** | Sales, Legal, CFO | [challenge-11](./challenge-11-contract-bottleneck-dashboard/) |
| 12 | **Sales Contract Review Playbook** | Sales, Legal | [challenge-12](./challenge-12-sales-contract-playbook/) |
| 13 | **Customer Complaint Resolution Assistant** | Customer Care, Legal | [challenge-13](./challenge-13-customer-complaint-assistant/) |
| 14 | **Employment Law Self-Service Assistant for HR** | HR, Legal | [challenge-14](./challenge-14-employment-law-hr-assistant/) |
| 15 | **Law Enforcement Request Compliance Assistant** | Legal, Compliance, IT | [challenge-15](./challenge-15-law-enforcement-compliance/) |
| 16 | **Negotiation Preparation Tool** — ZOPA, BATNA & Counterparty Interests | Legal, Deal Teams, Procurement | [challenge-16](./challenge-16-negotiation-tool/) |

---

## How the Day Works

### Schedule

| Time | Activity |
|------|----------|
| 09:00 – 09:30 | Welcome & challenge introduction |
| 09:30 – 10:00 | Tool walkthrough & team formation |
| 10:00 – 12:30 | Build session 1 |
| 12:30 – 13:30 | Lunch break |
| 13:30 – 16:30 | Build session 2 |
| 16:30 – 17:00 | Final polish & prep |
| 17:00 – 18:00 | Presentations & judging |

### Who Should Participate
- **Lawyers and legal professionals** — you know the problems best. You don't need to know how to code.
- **Paralegals and legal ops** — you live in the workflows. You know exactly where the bottlenecks are.
- **Business professionals** (HR, procurement, sales, compliance) — you interact with legal constantly. What would make your life easier?
- **Anyone curious** — this is a day for exploration. No prerequisites required.

### Judging Criteria

| Criterion | Weight | What We're Looking For |
|-----------|--------|-----------------------|
| **Practical Impact** | 30% | Does this solve a real, recurring problem? Would people actually use it? |
| **Quality of Output** | 25% | How good are the results the solution produces? |
| **Creativity** | 20% | Is the approach novel or surprisingly effective? |
| **Usability** | 15% | Could a non-technical user pick this up and use it? |
| **Presentation** | 10% | Is the demo clear, compelling, and well-structured? |

---

## Getting Started in 5 Steps

1. **Browse the challenges** — scan the list above and pick the one that resonates with you
2. **Form your team** — 1 to 4 people; solo is fine too
3. **Read the challenge brief** in the folder and explore the mock data
4. **Choose your tool(s)** — Claude Code, claude.ai, Antigravity, Gemini Canvas, or any combination
5. **Start small and build up** — get one thing working, then improve it

---

## Rules

- Use any publicly available AI tool — Claude, Gemini, ChatGPT, open-source models, or any combination
- All mock data is fictional — do not use real client data, privileged information, or confidential documents
- Think about data privacy — be ready to explain how your solution would handle sensitive data in production
- Most importantly: **have fun, ask for help, and be open to surprises**

---

## Repository Structure

```
legalhackathon/
├── README.md                                    ← You are here
├── challenge-01-contract-review-assistant/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-02-self-service-nda-generator/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-03-legal-faq-bot/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-04-clause-library/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-05-compliance-checklist-generator/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-06-legal-document-summarizer/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-07-german-court-case-checker/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-08-vendor-due-diligence-screener/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-09-agb-review-tool/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-10-regulatory-horizon-map/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-11-contract-bottleneck-dashboard/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-12-sales-contract-playbook/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-13-customer-complaint-assistant/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-14-employment-law-hr-assistant/
│   ├── CHALLENGE.md
│   └── mock-data/
├── challenge-15-law-enforcement-compliance/
│   ├── CHALLENGE.md
│   └── mock-data/
└── challenge-16-negotiation-tool/
    ├── CHALLENGE.md
    └── mock-data/
```

---

Now go build something. You might surprise yourself with what's possible in a single day.
