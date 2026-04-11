# Challenge 18: AI Agent Compliance Harness

## The Problem

Your company is building AI agents everywhere — in HR, sales, procurement, IT, marketing, and finance. Some were spun up by a developer in an afternoon. Some are running in n8n or Zapier automations. Some are Claude or GPT prompts called via API. Nobody has a complete list of them. Nobody has assessed their risk. Nobody is logging their outputs. Nobody has checked whether they comply with the EU AI Act.

The EU AI Act entered into force on 1 August 2024. Prohibitions applied from 2 February 2025. High-risk system requirements are phasing in through 2026. **The deployer bears the liability** — not the AI vendor. That means your company is exposed for every agent it runs, whether or not Legal knows it exists.

A policy document that nobody reads will not solve this. What the company needs is a **compliance harness** — a governance layer that makes compliant behavior the path of least resistance, and non-compliant deployment the hard path.

## Your Mission

Design and prototype an AI Agent Compliance Harness — a governance layer that can be applied to any AI agent your company deploys. Your solution can tackle one, two, or all three of the following layers:

---

### Layer 1: Agent Registry & Risk Classifier

Before an agent goes live, it must be registered and classified. Build a tool that:

1. **Collects basic agent metadata**: name, owner, department, purpose, deployment date, AI model/platform used
2. **Classifies the agent by EU AI Act risk tier** using a structured questionnaire:
   - Does it process biometric, health, or criminal data?
   - Does it make or materially influence decisions about employees, job applicants, students, or loan applicants?
   - Does it interact with users who may not know they're talking to AI?
   - Does it operate in a safety-critical domain (healthcare, infrastructure, law enforcement)?
3. **Outputs the applicable compliance obligations** for that risk tier — what the agent must have before it can be deployed (conformity assessment, human oversight mechanism, transparency notice, audit logging, etc.)

**Use the fictional agent registry in `mock-data/agent-registry-unaudited.json`** — 10 agents currently running in the company with no risk classification. Your job: classify them all and identify which ones have compliance gaps.

---

### Layer 2: Compliance Wrapper

Build a **reusable compliance layer** that can be added to any agent's system prompt or workflow to enforce the following at runtime:

| Requirement | What it means in practice |
|-------------|--------------------------|
| **Transparency** | Every interaction starts with a disclosure that the user is talking to an AI system |
| **Prohibited use filter** | The agent refuses requests that fall into EU AI Act prohibited categories (social scoring, emotional manipulation, biometric identification without consent) |
| **Human escalation gate** | For high-risk decisions, the agent must flag for human review rather than acting autonomously |
| **Data minimization** | The agent does not retain, repeat, or process personal data beyond what's needed for the task |
| **Audit trail** | Every input/output is structured for logging: timestamp, user ID (anonymized), request type, output summary, confidence level, escalated Y/N |

See `mock-data/compliance-wrapper-system-prompt.md` for a starter template. Your job: test it, improve it, and adapt it to a specific agent use case from the registry.

---

### Layer 3: Governance Dashboard Concept

Design (or build) a **central governance view** showing:
- All registered agents, their risk tier, and compliance status
- Which agents are missing required controls
- A deployment gate: agents cannot be marked "live" without completing the required steps for their risk tier
- An audit log viewer: show recent decisions flagged for human review

This can be a working prototype (Claude artifact, Antigravity app, n8n dashboard) or a detailed design spec with mockups.

---

## What the EU AI Act Actually Requires (Relevant Excerpts)

### Prohibited Practices (Art. 5 — applies now)
These are **absolutely forbidden**, regardless of business justification:
- AI systems that manipulate users through subliminal techniques or by exploiting vulnerabilities
- Social scoring of natural persons by public authorities
- Real-time remote biometric identification in public spaces (with narrow exceptions)
- AI used to infer emotions of workers or students in workplace/educational settings
- Predictive policing based on profiling alone (without objective evidence)
- Facial recognition databases built by scraping the internet

### High-Risk Categories (Annex III — obligations phasing in)
An agent is **high-risk** if it operates in any of these areas:
- **Employment**: CV screening, hiring decisions, performance monitoring, promotion/demotion
- **Credit & insurance**: creditworthiness assessment, risk scoring
- **Education**: student assessment, examination monitoring, admission decisions
- **Essential services**: access to housing, utilities, social benefits
- **Law enforcement**: crime prediction, evidence assessment, profiling
- **Migration**: asylum decisions, border control
- **Critical infrastructure**: safety components of energy, water, transport, finance

High-risk agents require: conformity assessment, technical documentation, human oversight mechanism, accuracy/robustness/cybersecurity standards, registration in the EU database.

### Transparency Obligations (Art. 50 — applies to all)
- Users must be informed when interacting with an AI system (unless obvious)
- Deepfakes and AI-generated content must be labeled
- Emotion recognition and biometric categorization systems must notify subjects

---

## What Success Looks Like

- You can take any agent from `agent-registry-unaudited.json`, run it through your classifier, and receive a clear compliance verdict: **Prohibited / High-Risk (compliant) / High-Risk (gaps) / Limited Risk / Minimal Risk**
- A legal or compliance professional can use your tool without technical knowledge
- For at least one high-risk agent, you can demonstrate what the compliance wrapper looks like in action
- The output is actionable: a team running a non-compliant agent knows exactly what they need to fix and by when

## Mock Data Provided

| File | Description |
|------|-------------|
| `agent-registry-unaudited.json` | 10 fictional AI agents currently running in the company — no risk classification, no compliance controls documented |
| `eu-ai-act-risk-rubric.md` | A structured decision tree for classifying agents by EU AI Act risk tier |
| `compliance-wrapper-system-prompt.md` | A starter compliance wrapper that can be added to any agent's system prompt |
| `prohibited-use-cases.md` | Plain-language breakdown of Art. 5 prohibited practices mapped to realistic company scenarios |

## Suggested Approaches

### Option A: Policy + Classification Tool (no code)
Build a well-structured intake form (or prompt chain) that classifies any agent by risk tier and outputs the compliance checklist it must complete before deployment. Deliverable: a polished prompt, a Claude artifact form, or a structured document.

### Option B: Compliance Wrapper in Action
Take one of the unclassified agents from the registry (e.g., the hiring screener or the HR leave bot), wrap it with the compliance layer, and demonstrate the difference in behavior — before and after. Deliverable: a demo with the wrapper applied.

### Option C: Full Governance Prototype
Build a working app (using Claude Code, Antigravity, or n8n) that includes a registry, a risk classifier, and a compliance status dashboard. Deliverable: a working prototype.

### Option D: Legal Framework + Deployment Policy
Forget the tech entirely. Draft the governance policy that makes this mandatory — the internal regulation that says: "No AI agent may be deployed without completing the following steps." Define the process, the sign-off requirements, the prohibited use list, and the audit obligations. Deliverable: a working paper or policy document.

## Prompt Starter

```
You are an EU AI Act compliance advisor specializing in AI agent governance.

A company has asked you to assess their AI agent portfolio for EU AI Act compliance.
For each agent described, you will:

1. Classify it by risk tier: Prohibited | High-Risk | Limited Risk | Minimal Risk
2. Cite the specific EU AI Act article or Annex III category that determines the classification
3. List the compliance obligations triggered by that classification
4. Identify the most critical compliance gap based on what the company has told you
5. State whether this agent can be deployed as-is, needs remediation, or must be shut down

Be direct. If an agent should be shut down, say so clearly and explain why.
If an agent is technically deployable but has serious gaps, name exactly what needs to change before it goes live.
```

## Stretch Goals

- **GPAI Model Register**: Many companies use third-party AI models (Claude, GPT-4, Gemini) as the foundation for their agents. Build a companion register that tracks which GPAI models are in use and whether they meet the EU AI Act's GPAI transparency requirements (technical documentation, copyright policy, energy consumption disclosure for systemic models)
- **Automated audit log analyzer**: Take a sample audit log from a deployed agent and use AI to identify patterns that suggest compliance risk (e.g., consistently ignoring escalation triggers, processing data types outside its stated scope)
- **Employee-facing disclosure generator**: Auto-generate the required transparency notices for each agent, tailored to the audience (workers, job applicants, customers) and compliant with both the EU AI Act and DSGVO
- **Incident response playbook**: What happens when a non-compliant agent causes harm? Draft the playbook: who is notified, what gets preserved, how is the regulator informed, who is legally exposed
