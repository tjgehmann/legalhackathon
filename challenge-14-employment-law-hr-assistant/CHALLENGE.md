# Challenge 14: Employment Law Self-Service Assistant for HR

## The Problem

TechForward's HR team of four handles hiring, onboarding, performance management, and offboarding for 280 employees across three German offices. They interact with Legal on employment matters — but Legal has a backlog, and most of the questions HR asks are the same ones, over and over.

The most common: "Can we do this?" And the most common answer from Legal: "It depends."

HR has no structured way to assess whether a proposed action — dismissing an employee, issuing a warning, hiring on a fixed-term contract, extending a probation period — is legally sound before proceeding. They either send a Legal ticket (slow) or make an educated guess (risky). Two recent incidents illustrate the problem:

**Incident A:** A line manager told HR to dismiss an underperforming employee. HR drafted the dismissal letter and sent it — without consulting the Works Council first. The dismissal was void. The employee's lawyer wrote back within 48 hours. Legal had to negotiate a settlement at three times the cost of a proper process.

**Incident B:** HR was about to dismiss an employee during their probation period for performance reasons. Legal happened to see the email trail and noticed the employee had submitted a medical certificate showing she was pregnant three days earlier. The dismissal would have been illegal (§ 17 MuSchG). The dismissal was stopped in time — but only by chance.

Both incidents are textbook. Both were preventable with basic process knowledge.

## Your Mission

Build an AI-powered Employment Law Self-Service Assistant that empowers HR to:

1. **Assess any proposed HR action** against the relevant legal requirements — before taking it
2. **Follow the correct step-by-step routine** for each scenario: dismissal, warning, fixed-term contract, works council consultation, redundancy, special cases
3. **Identify protected employees** automatically — pregnant, on parental leave, severely disabled, Works Council members, Data Protection Officers — and block or redirect the workflow accordingly
4. **Know when to stop and call Legal** — not every HR decision needs Legal involvement, but some do, and the tool must get this distinction right
5. **Generate compliant HR communications** — warning letters, works council consultation notices, confirmation letters — using pre-approved templates

## The Legal Landscape (German Employment Law)

German employment law is one of the most employee-protective systems in the world. The key laws HR needs to navigate:

| Law | What It Governs |
|-----|----------------|
| **KSchG** (Kündigungsschutzgesetz) | Unfair dismissal protection — applies after 6 months' employment in companies with more than 10 employees |
| **BGB §§ 620–628** | General contract and notice period rules |
| **BGB § 622** | Statutory notice periods by length of service |
| **AGG** (Allgemeines Gleichbehandlungsgesetz) | Anti-discrimination in hiring and employment |
| **BetrVG** (Betriebsverfassungsgesetz) | Works Council rights — consultation and co-determination |
| **MuSchG** (Mutterschutzgesetz) | Maternity protection — dismissal prohibition during pregnancy and for 4 months post-birth |
| **BEEG** (Bundeselterngeld- und Elternzeitgesetz) | Parental leave protection — dismissal prohibition during Elternzeit |
| **SGB IX** (Schwerbehindertenschutz) | Severely disabled protection — Integrationsamt approval required before dismissal |
| **BDSG / DSGVO** | Data Protection Officer has special dismissal protection |
| **TzBfG** (Teilzeit- und Befristungsgesetz) | Rules for fixed-term and part-time contracts |
| **Collective Agreements (Tarifverträge)** | May grant longer notice periods, additional protections, or stricter dismissal requirements |

## What Success Looks Like

- HR can correctly assess 90% of standard employment situations without a Legal ticket
- No dismissal is issued without the Works Council consultation step being completed (where required)
- Protected employees are flagged **before** any action is taken — never after
- HR communications are consistent, professional, and use legally reviewed language
- Legal's time is freed up for complex matters — not routine process guidance
- The tool creates a documented trail showing that the correct process was followed, which is valuable if a dismissal is later challenged at the Arbeitsgericht

## Mock Data Provided

| File | Description |
|------|-------------|
| `hr-scenario-catalog.json` | 15 HR scenarios covering hiring, dismissal, warnings, fixed-term contracts, and special protections — each with legal requirements, step-by-step actions, escalation triggers, and HR authority limits |
| `employment-law-playbooks.md` | Detailed step-by-step routines for the 8 most common HR scenarios, including Works Council consultation templates and notice period calculators |
| `sample-hr-cases.json` | 10 realistic HR cases — including 4 with hidden legal complexity (protected employee, missed Works Council step, wrong dismissal type, AGG discrimination risk) |
| `legal-escalation-and-compliance.md` | Protected employee categories, statutory notice periods by tenure, Works Council rights by situation, deadlines, and prohibited actions |

## Suggested Approach

1. Read the scenario catalog and legal escalation guide first — understand the landscape before building
2. Build a **situation classifier**: HR describes what they want to do ("dismiss employee for performance reasons") — the tool identifies the correct scenario and legal framework
3. Build a **protection check**: before proceeding with any action, the tool asks about and checks all protected categories
4. For each scenario, build a **step-by-step routine** that HR follows — with explicit Legal escalation gates
5. Connect routines to **pre-approved templates** for written communications
6. Test with the 10 sample cases — confirm the 4 traps are caught

## Key Scenarios to Cover

| Scenario | Key Legal Complexity |
|----------|---------------------|
| **Dismissal during probation** | Shorter notice (2 weeks), no KSchG, but protection for pregnancy still applies |
| **Conduct dismissal (with prior warning)** | Warning required first; Works Council consultation mandatory; 2-week rule for extraordinary dismissal |
| **Performance dismissal** | Difficult to prove; clear documentation of targets and support required; Works Council consultation |
| **Redundancy (operational reasons)** | Sozialauswahl (social selection criteria) required; Works Council consultation; Interessenausgleich for large-scale redundancies |
| **Extraordinary / immediate dismissal** | 2-week deadline from becoming aware of the reason; Works Council emergency consultation (3 days); very high bar |
| **Fixed-term contract** | Sachgrund vs. sachgrundlose Befristung; 2-year limit without grounds; prior employment rule |
| **Works Council consultation** | Mandatory before all dismissals; specific content requirements; 1-week ordinary / 3-day extraordinary response window |
| **Severely disabled employee dismissal** | Integrationsamt approval required; process takes 4–6 weeks; refusal possible |
| **Pregnant / maternity employee** | Absolute dismissal prohibition; state authority approval required for very narrow exceptions |
| **Parental leave dismissal** | Dismissal prohibition; state authority (Gewerbeaufsicht) approval required in exceptional circumstances |

## Stretch Goals

- Build a **notice period calculator** that takes employment start date and employee age and outputs the correct statutory notice period under § 622 BGB, with a check for collective agreement extensions
- Add a **Sozialauswahl assistant** for redundancy situations: input the comparable employee pool, their tenure, age, maintenance obligations, and disability status, and calculate which employees have the lowest social protection score
- Build a **warning letter generator** that produces a legally compliant Abmahnung with the correct elements: specific incident description, instruction to desist, warning of consequences
- Create an **AGG-compliant job posting reviewer** that checks draft job postings for discriminatory language (age, gender, nationality, religion) and suggests neutral alternatives
- Add a **Betriebsrat consultation tracker** that tracks open consultation windows, deadlines, and responses for each dismissal in process
