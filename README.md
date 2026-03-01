# Legal Hackathon: AI-Powered Solutions for Everyday Legal Challenges

## What Is This Hackathon About?

Legal departments everywhere face the same problem: too much work, not enough time. Meanwhile, business teams wait days for answers to simple legal questions, contracts sit in review queues, and repetitive tasks eat into time that could be spent on high-value strategic work.

This hackathon brings together legal professionals, business analysts, and anyone curious about legal tech to build **practical, AI-powered solutions** that solve real everyday legal problems — in just one day.

No prior coding experience is required. The tools available today (Claude, Gemini, ChatGPT, and others) allow you to build working prototypes using natural language alone.

---

## Who Should Participate?

- **Legal professionals** (lawyers, paralegals, legal ops) who want to automate repetitive parts of their work
- **Business professionals** (procurement, HR, sales, compliance) who regularly interact with legal and want self-service tools
- **Anyone** interested in making legal work faster, more accessible, and less painful

---

## How the Hackathon Works

### Format
- **Duration:** 1 day (8 hours of working time)
- **Team size:** 1–4 people per team
- **Output:** A working prototype or proof-of-concept that demonstrates your solution

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

### Judging Criteria

| Criterion | Weight | Description |
|-----------|--------|-------------|
| **Practical Impact** | 30% | Does this solve a real, recurring problem? Would people actually use it? |
| **Quality of Output** | 25% | How good are the results the solution produces? |
| **Creativity** | 20% | Is the approach novel or surprisingly effective? |
| **Usability** | 15% | Could a non-technical user pick this up and use it? |
| **Presentation** | 10% | Is the demo clear, compelling, and well-structured? |

---

## The Challenges

Each challenge has its own folder with a detailed brief and mock data to get you started. Pick the one that excites your team the most.

| # | Challenge | Who Benefits | Folder |
|---|-----------|-------------|--------|
| 1 | **Contract Review Assistant** | Legal teams | [challenge-01](./challenge-01-contract-review-assistant/) |
| 2 | **Self-Service NDA Generator** | Business teams (Sales, Partnerships) | [challenge-02](./challenge-02-self-service-nda-generator/) |
| 3 | **Legal FAQ Bot for Non-Legal Teams** | All departments | [challenge-03](./challenge-03-legal-faq-bot/) |
| 4 | **Clause Library & Comparison Tool** | Legal teams | [challenge-04](./challenge-04-clause-library/) |
| 5 | **Compliance Checklist Generator** | Product, Marketing, HR | [challenge-05](./challenge-05-compliance-checklist-generator/) |
| 6 | **Legal Document Summarizer & Risk Flagger** | Legal teams, Management | [challenge-06](./challenge-06-legal-document-summarizer/) |
| 7 | **German Court Case Checker** | Legal teams, Management | [challenge-07](./challenge-07-german-court-case-checker/) |
| 8 | **Vendor Due Diligence Screener** | Compliance, Procurement | [challenge-08](./challenge-08-vendor-due-diligence-screener/) |
| 9 | **AGB & Einkaufsbedingungen Review Tool** | Legal teams, Procurement | [challenge-09](./challenge-09-agb-review-tool/) |
| 10 | **Regulatory Horizon Map** | Executives, Legal teams | [challenge-10](./challenge-10-regulatory-horizon-map/) |
| 11 | **Contract Bottleneck & Deal Velocity Dashboard** | Sales, Legal, CFO | [challenge-11](./challenge-11-contract-bottleneck-dashboard/) |

---

## How to Use AI Tools to Build Your Solution

You don't need to be a developer. Modern AI tools let you build real prototypes through conversation. Here's how to get the most out of them.

### Recommended Tools

#### Claude (by Anthropic) — [claude.ai](https://claude.ai)
- **Best for:** Long document analysis, nuanced legal reasoning, structured output, building apps with artifacts
- **Key strengths:** Handles very long documents (up to 200K tokens), strong at following complex instructions, excellent at generating structured formats (JSON, Markdown, tables)
- **Pro tips:**
  - Use Claude's **Projects** feature to upload your mock data and reference documents, then chat with them across multiple conversations
  - Ask Claude to create **artifacts** — it can build interactive HTML/CSS/JS applications, dashboards, and forms right in the chat
  - For complex prompts, ask Claude to help you write the prompt first: *"Help me write a system prompt for a contract review assistant that flags risky clauses"*
  - Use the **extended thinking** toggle for tasks that require deep analysis or multi-step reasoning

#### Gemini (by Google) — [gemini.google.com](https://gemini.google.com)
- **Best for:** Integration with Google Workspace, multimodal analysis, web-grounded responses
- **Key strengths:** Can work with Google Docs/Sheets natively, good at processing tables and spreadsheets, access to current web information
- **Pro tips:**
  - Use Gemini within **Google Docs** to draft, review, and refine legal content directly
  - Upload PDFs and images for analysis — useful for scanned contracts or legacy documents
  - Ask Gemini to create **Google Apps Script** automations that connect Sheets, Docs, and Forms

#### ChatGPT (by OpenAI) — [chat.openai.com](https://chat.openai.com)
- **Best for:** Custom GPTs, code generation, broad general knowledge
- **Key strengths:** Custom GPT builder for creating shareable tools, strong code interpreter, large plugin ecosystem
- **Pro tips:**
  - Build a **Custom GPT** as your deliverable — it's a ready-to-share tool with instructions and uploaded knowledge
  - Use **Code Interpreter** to analyze CSV data, generate charts, or process documents programmatically

### General Tips for All Tools

1. **Start with a system prompt.** Define the role, rules, and output format before asking your first question.
   ```
   You are a contract review assistant for a mid-size technology company.
   Your role is to review vendor contracts and flag:
   - Unusual liability clauses
   - Missing standard protections
   - Terms that deviate from our standard positions
   Always output your findings as a structured table.
   ```

2. **Provide examples.** Show the AI what good output looks like. Include a sample input and your expected output.

3. **Iterate, don't start over.** If the output isn't right, tell the AI what to fix: *"The liability analysis is too vague — be more specific about which party bears the risk and reference the exact clause number."*

4. **Break complex tasks into steps.** Instead of *"Review this entire contract"*, try:
   - Step 1: *"Extract all clauses related to liability and indemnification"*
   - Step 2: *"For each clause, assess whether it favors our company, the vendor, or is neutral"*
   - Step 3: *"Flag any clauses that deviate from market standard terms"*

5. **Use structured output formats.** Ask for tables, JSON, bullet points, or checklists rather than free-form text. Structured output is easier to integrate into workflows.

6. **Upload your mock data.** Every challenge folder contains realistic mock data. Upload it to your AI tool of choice and build your solution around it.

### What Your Deliverable Could Look Like

Your prototype can take many forms — pick what makes sense for your solution:

- **A well-crafted prompt or prompt chain** that reliably produces high-quality output (with a demo)
- **An interactive artifact** built inside Claude (HTML/JS applications, forms, dashboards)
- **A Custom GPT** with uploaded knowledge and instructions
- **A Google Workspace automation** powered by Gemini
- **A Jupyter notebook** or script that processes documents using an AI API
- **A workflow diagram + demo** showing how AI fits into an existing process

---

## Getting Started

1. **Browse the challenges** in the folders below and pick one
2. **Form your team** (or go solo — that's fine too)
3. **Read the challenge brief** and explore the mock data
4. **Choose your AI tool(s)** — you can combine multiple tools
5. **Start building!** Begin with the simplest version that works, then improve it

---

## Rules & Guidelines

- You may use any publicly available AI tool (Claude, Gemini, ChatGPT, open-source models, etc.)
- All mock data provided is fictional — do not use real client data, privileged information, or confidential documents
- Solutions should be designed with data privacy in mind — explain how your approach would handle sensitive information in production
- Have fun, ask for help, and learn something new

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
└── challenge-11-contract-bottleneck-dashboard/
    ├── CHALLENGE.md
    └── mock-data/
```

Good luck — go build something that makes legal work better for everyone.
