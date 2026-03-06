# Challenge 15: Law Enforcement Request Compliance Assistant

## The Problem

NetHost GmbH is a mid-sized German hosting and domain registrar operating under German law. It provides shared hosting, VPS, dedicated servers, managed email (Postfächer), domain registration, and DNS services to approximately 45,000 customers.

Every week, NetHost's compliance team receives law enforcement requests. Most arrive by fax or post, some by email, a few by phone. They range from formal court orders to informal police emails. They cite different legal bases. They ask for different types of data. They come from different authorities. They have different deadlines.

The current process is a spreadsheet and an overworked compliance officer.

**The risks are real and they cut both ways:**

**Risk 1 — Complying when you shouldn't:** A company that hands over customer data without a valid legal basis violates the DSGVO and the TTDSG. Data protection fines, civil liability to the customer, and reputational damage follow.

**Risk 2 — Not complying when you must:** A company that refuses a valid Beschlagnahmebeschluss from a court, or delays a lawful Auskunftsverlangen, obstructs justice. Criminal liability, regulatory sanction, and contempt proceedings follow.

**Risk 3 — Complying incorrectly:** A company that provides the wrong data category in response to a request that only authorizes a narrower disclosure goes beyond what is legally permitted. DSGVO violation.

**Risk 4 — Missing the deadline:** A valid request with a 24-hour response deadline that sits in the fax queue over the weekend exposes NetHost to enforcement action.

The compliance officer needs to make the right call, quickly, on every request. Today that takes 30–90 minutes per request. With AI assistance, it should take 5 minutes.

---

## The Legal Landscape

German law enforcement requests to hosting and domain companies are governed by a specific set of laws. Understanding the differences between them is critical — the same request may be lawful under one provision and unlawful under another.

### Core Legal Framework

| Law | Relevance |
|-----|-----------|
| **StPO** (Strafprozessordnung) | Criminal procedure — primary basis for seizure, search, and disclosure orders in criminal investigations |
| **§ 94–98 StPO** | Sicherstellung und Beschlagnahme (seizure and confiscation) of evidence |
| **§ 99–101 StPO** | Postbeschlagnahme — originally postal items, applied by courts to email |
| **§ 100a StPO** | Telekommunikationsüberwachung (TKÜ) — real-time interception of communications |
| **§ 100g StPO** | Verkehrsdatenerhebung — traffic/connection data (IP logs, timestamps, connection records) |
| **§ 161, 163 StPO** | General investigation authority of Staatsanwaltschaft and police |
| **§ 174–177 TKG** | Disclosure obligations for telecommunications providers — Bestandsdaten, Zugangsdaten |
| **§ 22–23 TTDSG** | Data disclosure for telemedia services (hosting, websites) |
| **Art. 10 GG** | Constitutional protection of Fernmeldegeheimnis (telecommunications secrecy) — the constitutional floor |
| **DSGVO Art. 6(1)(c)** | Legal obligation basis — processing is lawful when required by law |
| **DSGVO Art. 23** | Restrictions on data subject rights for law enforcement purposes |
| **ICANN RAA / RDSAP** | Registrar obligations for domain WHOIS data disclosure |

### The Two Most Important Distinctions

**Distinction 1: Who is issuing the request?**

| Issuer | Authority Level | What They Can Order |
|--------|----------------|---------------------|
| **Richter** (judge / court) | Highest | All orders including TKÜ, Postbeschlagnahme, Beschlagnahme |
| **Staatsanwalt** (prosecutor) | High | Bestandsdatenauskunft, Verkehrsdaten (with court order), Beschlagnahme in urgent cases (Gefahr im Verzug) |
| **Polizei** (police) | Limited | Bestandsdatenauskunft in specific circumstances; most requests require StA or court order |
| **Ausländische Behörde** (foreign authority) | None directly | Must go through MLAT / European Investigation Order (EIO) — no direct compliance obligation |

**Distinction 2: What type of data is being requested?**

| Data Type | German Term | Legal Basis Required | Sensitivity |
|-----------|-------------|---------------------|-------------|
| Customer identity data | Bestandsdaten | § 174 TKG, § 22 TTDSG, § 161/163 StPO | Medium |
| Domain registration data | Registrierungsdaten | § 174 TKG, ICANN RAA | Medium |
| Traffic/connection data | Verkehrsdaten | § 100g StPO + court order | High |
| Email content (stored) | Inhaltsdaten (gespeichert) | § 94/99 StPO + court order | Very High |
| Real-time communications | Inhaltsdaten (live) | § 100a StPO + court order | Very High |
| Stored files / hosted content | Gespeicherte Daten | § 94 StPO + court order | Very High |
| IP address → customer mapping | Zugangsdaten | § 174 TKG | High |

---

## The Requests NetHost Receives

### Type 1 — Bestandsdatenauskunft (Customer Data Request)
Law enforcement asks: "Who is the customer behind domain example.com / IP 1.2.3.4 / account #12345? Give us their name, address, and contact details."

**Legal basis:** § 174 TKG (for TK providers), § 22 TTDSG (for hosting/telemedia), § 161/163 StPO
**Court order required?** No — but formal written request from Staatsanwaltschaft or authorized police officer required. Informal emails or phone calls are not sufficient.
**Response obligation:** Exists if the formal requirements are met. DSGVO Art. 6(1)(c) covers this.
**Response time:** Typically 24–72 hours; immediate in Gefahr im Verzug situations.

### Type 2 — Postfachbeschlagnahme (Email Mailbox Seizure)
Law enforcement asks: "Secure and hand over all emails in mailbox user@example.com from [date] to [date] / all stored emails."

**Legal basis:** § 99 StPO (Postbeschlagnahme) applied to electronic mail by courts; § 94 StPO as alternative
**Court order required?** YES — Richterlicher Beschluss required (§ 100 StPO). Staatsanwaltschaft can order in Gefahr im Verzug but must obtain judicial confirmation "unverzüglich".
**Constitutional basis:** Art. 10 GG — email content enjoys constitutional protection of Fernmeldegeheimnis.
**Response time:** As specified in the order. For Gefahr im Verzug: immediate.
**Key check:** Is the Beschluss signed by a judge? Does it specify the exact mailbox and time period? Is it current (not expired)?

### Type 3 — Allgemeine Beschlagnahme (General Data Seizure)
Law enforcement asks: "Seize and hand over all data associated with account #12345 / all files hosted at domain example.com."

**Legal basis:** § 94 StPO (Sicherstellung), § 98 StPO (Beschlagnahmebeschluss)
**Court order required?** Yes for formal Beschlagnahme. Police/StA can make an interim Sicherstellung which must be confirmed by court.
**Response time:** As specified. Often requires immediate compliance.

### Type 4 — Verkehrsdatenauskunft (Traffic Data Request)
Law enforcement asks: "Who had IP address 1.2.3.4 on [date] at [time]? Provide all connection logs for account #12345 from [date] to [date]."

**Legal basis:** § 100g StPO
**Court order required?** YES — Richterlicher Beschluss required (§ 101a StPO)
**Key issue:** Vorratsdatenspeicherung (VDS — data retention) has been repeatedly struck down by ECJ and German courts. NetHost may not even have the requested historical traffic data if it complies with DSGVO minimal retention — this must be disclosed in the response.
**Response time:** As specified in the court order.

### Type 5 — Telekommunikationsüberwachung (Real-time Interception)
Law enforcement asks: "Provide us with a real-time feed of all communications from/to account #12345 / mailbox user@example.com."

**Legal basis:** § 100a StPO
**Court order required?** YES — Always requires a Richterlicher Beschluss. No exceptions.
**TKÜ technical obligation:** Hosting companies may have a Mitwirkungspflicht (obligation to cooperate technically) under § 170 TKG — if NetHost is classified as an "öffentliches Telekommunikationsnetz"/"öffentlich zugänglicher Telekommunikationsdienst". This is fact-dependent.
**Key issue:** Real-time interception is technically complex and may require SINA hardware or similar. Many hosting companies are not in scope for TKÜ. Legal assessment required.

### Type 6 — Domain-Daten / WHOIS-Auskunft (Domain Data)
Law enforcement asks: "Who registered domain example.com? Provide registrant contact data, registration date, and WHOIS record."

**Legal basis:** § 174 TKG, ICANN Registrar Accreditation Agreement (RAA), RDSAP (Registration Data Access Protocol)
**Court order required?** No — Bestandsdaten level request sufficient.
**Special consideration:** ICANN has specific procedures for law enforcement WHOIS access that run parallel to German law obligations.

### Type 7 — Informelle Polizeianfragen (Informal Police Requests)
A police officer calls or emails: "Hey, we're investigating a fraud case — can you tell me who owns the account hosting website xyz.de?"

**Legal basis:** NONE that creates a compliance obligation.
**Correct response:** Refer the officer to the Staatsanwaltschaft for a formal Auskunftsersuchen. Do not provide any data.
**Why this matters:** An informal request, no matter how polite, does not create a legal basis under DSGVO Art. 6(1)(c) for processing (disclosing) customer data. Complying would be a DSGVO violation.

### Type 8 — Ausländische Behörden (Foreign Law Enforcement)
A US law enforcement agency (or any foreign authority) requests customer data directly.

**Legal basis:** NONE for direct compliance.
**Correct response:** Refer to the mutual legal assistance treaty (MLAT) process or European Investigation Order (EIO / Europäische Ermittlungsanordnung) for EU member states. Do not provide any data directly.
**Exception:** CLOUD Act requests for US companies with EU subsidiaries require specific legal assessment — escalate to Legal immediately.

---

## What Success Looks Like

NetHost's compliance assistant should:

1. **Parse and classify** any incoming law enforcement request — identify the request type, issuing authority, cited legal basis, data type requested, and deadline
2. **Validate the formal requirements** — is this from the right authority? Is a court order present where one is required? Is the cited legal provision correct and applicable?
3. **Check for red flags** — informal request with no legal basis, foreign authority without MLAT, court order that's expired, request that exceeds what the cited law permits
4. **Determine the response obligation** — must comply, may refuse, must partially comply, must escalate to legal counsel
5. **Calculate the deadline** — when must NetHost respond? What internal steps must happen first?
6. **Identify which data is in scope** — what exactly must be provided, and what must NOT be provided (to avoid over-disclosure)
7. **Trigger the data preservation hold** — even before responding, a valid court order may require NetHost to freeze data to prevent deletion
8. **Draft the response letter** — using pre-approved templates for each scenario
9. **Flag the DSGVO angle** — is notification of the customer required or prohibited? What basis exists for processing?
10. **Log and track** — create an immutable audit trail of every request received and action taken

---

## Mock Data Provided

| File | Description |
|------|-------------|
| `request-type-catalog.json` | 8 request types with full legal framework, formal requirements checklist, validation rules, required response actions, and data scope rules |
| `sample-requests.json` | 12 sample incoming requests — including valid ones, invalid ones, edge cases, and traps (informal requests, expired orders, requests exceeding legal scope, foreign authorities) |
| `legal-framework-stpo.md` | Deep dive into the German legal framework: StPO provisions, TKG obligations, TTDSG, DSGVO intersection, Art. 10 GG constitutional protection, Richterlicher Vorbehalt principle, Gefahr im Verzug doctrine, VDS status, and ICANN obligations |
| `response-templates.md` | Template letters in German for each response type: compliance, partial compliance, rejection (insufficient legal basis), referral to StA (for informal police requests), and request for clarification |

## Suggested Approach

1. Read `legal-framework-stpo.md` first — understanding the hierarchy of authority and the distinction between data types is the foundation
2. Build a **request classifier** that takes a request description (or scanned letter OCR) and identifies: request type, issuing authority, cited legal basis, requested data type
3. Build a **validation engine** against `request-type-catalog.json` — check each formal requirement against what the request contains
4. Build a **decision tree** with four outputs: COMPLY / PARTIAL COMPLY / REFUSE / ESCALATE TO LEGAL
5. Wire in **deadline tracking** — every request gets a response deadline in the system
6. Connect to the **response templates** to auto-draft the outgoing letter
7. Test with all 12 sample requests — ensure the 5 traps are caught

## Stretch Goals

- Build a **data preservation hold trigger**: when a valid seizure order arrives, automatically flag the relevant account in the hosting system as "legal hold — do not delete"
- Build a **DSGVO notification assessment**: for each request type, determine whether Art. 17(3)(e) DSGVO or a specific StPO prohibition blocks NetHost from notifying the customer, or whether the customer must be notified after the investigation concludes
- Add a **Vorratsdatenspeicherung status check**: before responding to a Verkehrsdaten request, check whether the requested data would even exist given NetHost's current retention policies and the VDS legal situation
- Create a **TKÜ technical obligations checker**: assess whether NetHost's various services (email hosting, VPS, shared hosting) qualify as "öffentlich zugängliche TK-Dienste" subject to § 170 TKG TKÜ requirements
- Build a **request log with immutable audit trail**: DSGVO-compliant record of every law enforcement request received, the decision taken, the data provided (with hash), and the response sent
