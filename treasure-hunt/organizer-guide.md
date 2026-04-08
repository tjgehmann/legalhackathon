# Legal Hackathon AI Treasure Hunt — Organizer Guide

## Overview

A 5-station treasure hunt that teaches participants to use **Gemini + Google Workspace** before the hackathon challenges begin. Each station requires using a specific AI tool to uncover a hidden code word. The combined code words unlock the final link to the GitHub challenge repository.

**Duration:** ~30–45 minutes
**Group size:** Teams of 2–4 (same as hackathon teams)
**Requirements:** Each team needs a laptop with access to Google Workspace + Gemini

---

## Setup Checklist

### Before the Event

1. **Google Drive folder**: Create a shared folder called `Treasure Hunt` that all participants can access
2. **Station 1 — Google Doc**: Create a Google Doc called `Station 1 — The Mystery Clause` and paste the contract text from the clue below
3. **Station 2 — Google Sheet**: Create a Google Sheet called `Station 2 — Vendor Risk Data` with the data table below
4. **Station 3 — Gmail draft**: Prepare the scrambled email text (participants will use their own Gmail)
5. **Station 4 — Google Slides**: Create a blank Google Slides deck called `Station 4 — One-Slide Brief`
6. **Station 5 — Final puzzle**: This is on the treasure hunt webpage itself
7. **Share the treasure hunt link**: Host `treasure-hunt.html` (e.g., on GitHub Pages, or share the file directly)

---

## Station Details & Answer Keys

### Station 1: "The Hidden Penalties" (Gemini in Google Docs)

**Skill taught:** Using Gemini to find hidden risks and punitive clauses buried in a long contract — the #1 real-world legal AI use case

**Why Gemini is essential:** The Google Doc contains a realistic 19-section consulting agreement (~8 pages of dense legal text). Six sections contain hidden penalty clauses that impose financial consequences **on the Client**. These penalties use varied language ("liquidated damages", "surcharge", "additional charge", "penalty", "remediation fee", "deduction") so a simple Ctrl+F search won't catch them all. Each hidden penalty references a "Penalty Schedule" with a letter code. Gemini can semantically find all penalty clauses regardless of wording — exactly how lawyers use AI for contract review.

**Setup:** Create a Google Doc called "Station 1 — The Hidden Penalties" and paste the full contract below. Six sections contain a penalty clause with a Penalty Schedule reference. The Schedule letters, in the order they appear, spell **B-E-A-C-O-N**.

> **PROFESSIONAL SERVICES AGREEMENT**
>
> This Professional Services Agreement ("Agreement") is entered into as of the date of last signature (the "Effective Date") by and between TechCorp Solutions GmbH, a company organized under the laws of Germany, with its registered office at Friedrichstraße 123, 10117 Berlin ("Client"), and LegalEdge Consulting AG, a company organized under the laws of Switzerland, with its registered office at Bahnhofstrasse 45, 8001 Zürich ("Provider"), each referred to individually as a "Party" and collectively as the "Parties."
>
> WHEREAS, the Client desires to engage the Provider to deliver certain legal technology consulting services; and WHEREAS, the Provider has the expertise, resources, and willingness to provide such services on the terms set forth herein; NOW, THEREFORE, in consideration of the mutual covenants and agreements contained herein, the Parties agree as follows:
>
> ---
>
> **Section 1. TERM AND DURATION OF ENGAGEMENT**
> 1.1 This Agreement shall become effective on the Effective Date and shall remain in force for an initial period of thirty-six (36) months (the "Initial Term"). Thereafter, the Agreement shall automatically renew for successive twelve (12) month periods (each a "Renewal Term"), unless either Party provides written notice of non-renewal at least one hundred and twenty (120) days prior to the expiration of the then-current term. The Initial Term and any Renewal Terms are collectively referred to as the "Term."
> 1.2 Either Party may terminate this Agreement for convenience upon one hundred and eighty (180) days' prior written notice to the other Party, provided that all outstanding fees for services rendered through the effective date of termination shall remain due and payable. Any such termination shall not relieve either Party of obligations accrued prior to the effective date of termination.
> 1.3 In the event of early termination by the Client without cause, the Client shall pay the Provider a termination fee equal to twenty-five percent (25%) of the remaining fees that would have been payable during the then-current term, calculated based on the average monthly fees invoiced during the preceding six (6) months. Additionally, if the Client fails to provide the required one hundred and eighty (180) days' notice as stipulated in Section 1.2, the Client shall incur a supplementary administrative charge as further detailed in Penalty Schedule B, which shall be payable within fifteen (15) business days of the effective termination date.
>
> **Section 2. HANDLING OF CONFIDENTIAL INFORMATION**
> 2.1 Each Party acknowledges that in the course of performing its obligations under this Agreement, it may receive or have access to Confidential Information of the other Party. "Confidential Information" means all non-public information disclosed by one Party (the "Disclosing Party") to the other Party (the "Receiving Party"), whether orally, in writing, electronically, or by any other means, that is designated as confidential or that a reasonable person would understand to be confidential given the nature of the information and the circumstances of disclosure.
> 2.2 Confidential Information includes, without limitation: (a) trade secrets, inventions, patents, copyrights, and other intellectual property; (b) business plans, financial data, and projections; (c) customer and supplier lists and information; (d) technical data, designs, algorithms, and source code; (e) pricing information and fee structures; (f) employee and personnel information; and (g) any information marked "Confidential," "Proprietary," or with a similar designation.
> 2.3 The Receiving Party agrees to: (i) hold all Confidential Information in strict confidence using at least the same degree of care it uses to protect its own confidential information, but in no event less than reasonable care; (ii) not disclose Confidential Information to any third party without the prior written consent of the Disclosing Party; (iii) limit access to Confidential Information to those employees, agents, and advisors who have a legitimate need to know and who are bound by confidentiality obligations at least as protective as those contained herein; and (iv) not use Confidential Information for any purpose other than performing obligations under this Agreement.
> 2.4 The obligations set forth in this Section shall survive the termination or expiration of this Agreement for a period of seven (7) years. Upon termination or expiration, each Party shall promptly return or destroy all Confidential Information of the other Party in its possession, and shall certify such return or destruction in writing within thirty (30) days.
>
> **Section 3. ENGAGEMENT SCOPE AND DELIVERABLES**
> 3.1 The Provider shall perform the consulting services described in Exhibit A (the "Services"), which is attached hereto and incorporated by reference. The Services may include, but are not limited to: legal process optimization, technology needs assessment, vendor evaluation, implementation support, change management advisory, and post-implementation review.
> 3.2 The Provider shall deliver the work products specified in Exhibit A (the "Deliverables") in accordance with the timelines, specifications, and acceptance criteria set forth therein. Each Deliverable shall be subject to a review and acceptance process as described in Section 3.4 below.
> 3.3 The scope of Services may be amended, expanded, or reduced only by a written change order executed by authorized representatives of both Parties (a "Change Order"). Each Change Order shall specify: (a) the nature and extent of the change; (b) the impact on fees, timelines, and resources; and (c) any modifications to existing Deliverables. No change to the scope shall be effective unless documented in a signed Change Order.
> 3.4 Upon delivery of each Deliverable, the Client shall have fifteen (15) business days to review and either accept or reject the Deliverable (the "Review Period"). Rejection must be accompanied by a detailed written explanation of deficiencies. The Provider shall have ten (10) business days to cure any identified deficiencies and resubmit the Deliverable. If the Client fails to respond within the Review Period, the Deliverable shall be deemed accepted.
> 3.5 In the event that the Client requests more than three (3) rounds of revisions to any single Deliverable beyond the scope originally specified in Exhibit A, the Provider shall be entitled to apply an excess revision surcharge to compensate for the additional resources required, as calculated in accordance with Penalty Schedule E. The Client shall be notified of any such surcharge prior to the commencement of additional revision work.
>
> **Section 4. COMPENSATION AND PAYMENT SCHEDULE**
> 4.1 In consideration of the Services, the Client shall pay the Provider the fees set forth in Exhibit B (the "Fee Schedule"), which is attached hereto and incorporated by reference. Fees may be structured as fixed fees, time-and-materials rates, milestone-based payments, or a combination thereof, as specified in Exhibit B.
> 4.2 The Provider shall submit invoices monthly in arrears, or upon completion of the applicable milestone, in accordance with the billing schedule set forth in Exhibit B. Each invoice shall include: (a) a description of Services performed; (b) the applicable billing period; (c) hours worked (for time-and-materials engagements); (d) expenses incurred; and (e) the total amount due.
> 4.3 The Client shall pay all undisputed invoices within thirty (30) days of receipt. Late payments shall accrue interest at the rate of one and one-half percent (1.5%) per month, or the maximum rate permitted by applicable law, whichever is less. If any invoice or portion thereof is disputed, the Client shall pay the undisputed portion and provide written notice of the disputed amount within fifteen (15) days of receipt.
> 4.4 All fees are exclusive of applicable taxes, duties, and levies, including but not limited to value-added tax (VAT), goods and services tax (GST), and withholding taxes. Such taxes shall be the responsibility of the Client unless the Client provides a valid tax exemption certificate prior to the issuance of the relevant invoice.
> 4.5 The Provider reserves the right to suspend performance of the Services upon thirty (30) days' written notice if any undisputed invoice remains unpaid for more than sixty (60) days after its due date. Such suspension shall not constitute a breach of this Agreement and shall not relieve the Client of its payment obligations.
>
> **Section 5. OBLIGATIONS AND RESPONSIBILITIES OF THE CLIENT**
> 5.1 The Client shall designate a project manager (the "Client Project Manager") who shall serve as the primary point of contact for all matters relating to this Agreement. The Client Project Manager shall have the authority to make day-to-day decisions regarding the Services, approve Deliverables, and authorize Change Orders up to a value of EUR 25,000.
> 5.2 The Client shall provide the Provider with timely access to all documents, data, personnel, systems, and facilities reasonably necessary for the Provider to perform the Services. The Client acknowledges that delays in providing such access may result in corresponding delays in the delivery of Services and Deliverables, and that the Provider shall not be responsible for any such delays.
> 5.3 The Client shall ensure that all information and materials provided to the Provider are accurate, complete, and up-to-date to the best of the Client's knowledge. The Provider shall be entitled to rely on the accuracy of such information and materials without independent verification, and shall not be liable for any deficiency in the Services or Deliverables attributable to inaccurate or incomplete information provided by the Client.
> 5.4 Where the Client's failure to provide access to documents, systems, or personnel as required under Section 5.2 results in a delay of more than ten (10) business days to the project timeline, the Client acknowledges that a resource reallocation deduction may be applied to account for idle personnel costs and schedule disruption, the methodology for which is set forth in Penalty Schedule A.
> 5.5 The Client shall comply with all applicable laws and regulations in connection with its performance under this Agreement, including but not limited to data protection laws, export control regulations, and anti-corruption laws.
>
> **Section 6. DUTIES AND RESPONSIBILITIES OF THE PROVIDER**
> 6.1 The Provider shall perform the Services in a professional and workmanlike manner, in accordance with generally accepted industry standards and practices. The Provider shall assign qualified personnel with appropriate skills and experience to perform the Services.
> 6.2 The Provider shall designate a project manager (the "Provider Project Manager") who shall serve as the primary point of contact for all matters relating to this Agreement. The Provider Project Manager shall coordinate with the Client Project Manager on all aspects of service delivery, including scheduling, resource allocation, and issue resolution.
> 6.3 The Provider shall maintain adequate staffing levels to meet the agreed-upon timelines and quality standards. In the event that a key team member becomes unavailable, the Provider shall promptly notify the Client and propose a qualified replacement for the Client's approval, which shall not be unreasonably withheld.
> 6.4 The Provider shall comply with all applicable laws and regulations in connection with its performance under this Agreement, and shall maintain all licenses, permits, and certifications required to perform the Services.
>
> **Section 7. EXPENSE REIMBURSEMENT AND TRAVEL POLICY**
> 7.1 The Client shall reimburse the Provider for all reasonable and pre-approved out-of-pocket expenses incurred in connection with the performance of the Services, including but not limited to travel, accommodation, meals, and incidental expenses. All expenses must comply with the Client's travel and expense policy, a copy of which is attached as Exhibit C.
> 7.2 Air travel shall be at economy class for flights under five (5) hours and business class for flights of five (5) hours or more. Hotel accommodations shall not exceed EUR 250 per night in major metropolitan areas and EUR 180 per night in other locations, unless otherwise approved in writing by the Client Project Manager.
> 7.3 The Provider shall submit expense reports with supporting documentation (receipts, boarding passes, etc.) within thirty (30) days of incurring the expenses. Expense reports submitted more than sixty (60) days after the expense was incurred may be rejected at the Client's discretion.
>
> **Section 8. WARRANTIES AND REPRESENTATIONS**
> 8.1 Each Party represents and warrants that: (a) it is duly organized, validly existing, and in good standing under the laws of its jurisdiction of organization; (b) it has full power and authority to enter into this Agreement and to perform its obligations hereunder; (c) the execution and performance of this Agreement does not conflict with any other agreement to which it is a party; and (d) this Agreement constitutes a legal, valid, and binding obligation enforceable against it in accordance with its terms.
> 8.2 The Provider represents and warrants that: (a) the Services shall be performed in a professional and workmanlike manner consistent with generally accepted industry standards; (b) the Deliverables shall materially conform to the specifications and acceptance criteria set forth in Exhibit A; (c) the Provider has and shall maintain all necessary skills, qualifications, licenses, and certifications to perform the Services; and (d) the Services and Deliverables shall not infringe, misappropriate, or violate any intellectual property rights of any third party.
> 8.3 In the event that any Deliverable fails to conform to the warranties set forth in Section 8.2 and such non-conformance is not cured within the timeframe specified in Section 3.4, the Client shall be entitled to a remediation fee covering the cost of engaging alternative resources to rectify the deficiency, calculated pursuant to the terms of Penalty Schedule C. The Provider shall have the right to dispute the applicability of such fee by providing evidence that the non-conformance resulted from Client-provided specifications or materials.
> 8.4 THE WARRANTIES SET FORTH IN THIS SECTION ARE EXCLUSIVE AND IN LIEU OF ALL OTHER WARRANTIES, WHETHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING BUT NOT LIMITED TO WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT, TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW.
>
> **Section 9. OWNERSHIP OF WORK PRODUCT AND INTELLECTUAL PROPERTY**
> 9.1 All Deliverables and work products created by the Provider specifically for the Client under this Agreement (the "Work Product") shall be the exclusive property of the Client upon full payment of all applicable fees. The Provider hereby assigns to the Client all right, title, and interest in and to the Work Product, including all intellectual property rights therein.
> 9.2 Notwithstanding the foregoing, the Provider shall retain ownership of all pre-existing intellectual property, tools, methodologies, frameworks, templates, and know-how (collectively, "Provider IP") that existed prior to or were developed independently of this Agreement. To the extent that any Provider IP is incorporated into the Work Product, the Provider hereby grants the Client a non-exclusive, perpetual, irrevocable, worldwide, royalty-free license to use, reproduce, modify, and distribute such Provider IP solely as part of and in connection with the Work Product.
> 9.3 The Client shall retain ownership of all pre-existing intellectual property, data, and materials provided to the Provider in connection with the Services (the "Client IP"). The Provider shall not acquire any right, title, or interest in the Client IP except the limited right to use it for the purpose of performing the Services.
>
> **Section 10. REGULATORY COMPLIANCE AND LEGAL OBLIGATIONS**
> 10.1 Each Party shall comply with all applicable laws, regulations, directives, and orders of any governmental authority having jurisdiction over the subject matter of this Agreement, including but not limited to: (a) the General Data Protection Regulation (EU) 2016/679 ("GDPR"); (b) applicable national data protection laws; (c) anti-bribery and anti-corruption laws, including the UK Bribery Act 2010 and the U.S. Foreign Corrupt Practices Act; (d) export control and economic sanctions laws; (e) anti-money laundering laws; and (f) competition and antitrust laws.
> 10.2 Neither Party shall take any action that would cause the other Party to be in violation of any applicable law or regulation. Each Party shall promptly notify the other Party of any investigation, proceeding, or enforcement action by any governmental authority that may affect the other Party's rights or obligations under this Agreement.
> 10.3 The Provider shall maintain and, upon request, provide evidence of compliance with all applicable regulatory requirements, including data protection impact assessments, records of processing activities, and evidence of appropriate technical and organizational measures.
>
> **Section 11. DATA PROTECTION AND PROCESSING**
> 11.1 To the extent that the Provider processes personal data on behalf of the Client in connection with the Services, the Parties shall enter into a separate Data Processing Agreement ("DPA") in substantially the form attached as Exhibit D, which shall form an integral part of this Agreement.
> 11.2 The Provider shall implement and maintain appropriate technical and organizational measures to protect personal data against unauthorized or unlawful processing and against accidental loss, destruction, or damage, as further specified in the DPA. Such measures shall include, at a minimum: (a) encryption of personal data in transit and at rest; (b) regular testing of security measures; (c) access controls and authentication mechanisms; (d) employee training on data protection; and (e) incident response procedures.
> 11.3 The Provider shall not engage any sub-processor for the processing of personal data without the prior specific or general written authorization of the Client. In the case of general written authorization, the Provider shall inform the Client of any intended changes concerning the addition or replacement of sub-processors, giving the Client the opportunity to object to such changes.
> 11.4 Should a personal data incident occur that is attributable to the Client's failure to comply with the data handling requirements specified in Exhibit D or to implement the security measures reasonably requested by the Provider, the Client shall bear all costs associated with the incident response, including but not limited to forensic investigation, regulatory notification, and credit monitoring services, and shall additionally be subject to an accelerated compliance levy as outlined in Penalty Schedule O, reflecting the Provider's increased exposure and remediation burden.
>
> **Section 12. INDEMNIFICATION AND HOLD HARMLESS**
> 12.1 The Provider shall indemnify, defend, and hold harmless the Client and its officers, directors, employees, agents, successors, and assigns from and against any and all claims, damages, losses, costs, and expenses (including reasonable attorneys' fees and court costs) arising out of or relating to: (a) the Provider's breach of this Agreement; (b) the Provider's negligent or willful acts or omissions; (c) any infringement or misappropriation of any third party's intellectual property rights by the Services or Deliverables; or (d) any violation of applicable law by the Provider.
> 12.2 The Client shall indemnify, defend, and hold harmless the Provider and its officers, directors, employees, agents, successors, and assigns from and against any and all claims, damages, losses, costs, and expenses (including reasonable attorneys' fees and court costs) arising out of or relating to: (a) the Client's breach of this Agreement; (b) the Client's negligent or willful acts or omissions; (c) the Client's use of the Services or Deliverables in a manner not contemplated by this Agreement; or (d) any violation of applicable law by the Client.
> 12.3 The indemnifying Party's obligations under this Section are conditioned upon the indemnified Party: (i) providing prompt written notice of any claim; (ii) granting the indemnifying Party sole control of the defense and settlement of the claim; and (iii) providing reasonable cooperation and assistance at the indemnifying Party's expense.
>
> **Section 13. SUBCONTRACTING AND THIRD-PARTY ENGAGEMENT**
> 13.1 The Provider may subcontract portions of the Services to qualified third parties, provided that: (a) the Provider obtains the Client's prior written consent, which shall not be unreasonably withheld; (b) the Provider remains fully responsible for the performance of the subcontracted Services; (c) the subcontractor is bound by confidentiality and data protection obligations at least as protective as those contained in this Agreement; and (d) the Provider provides the Client with the identity and qualifications of the proposed subcontractor.
> 13.2 Neither Party may assign, transfer, or delegate this Agreement or any of its rights or obligations hereunder without the prior written consent of the other Party, except that either Party may assign this Agreement to a successor entity in connection with a merger, acquisition, corporate reorganization, or sale of all or substantially all of its assets, provided that the assignee agrees in writing to be bound by the terms of this Agreement and has the financial and operational capacity to perform the assigning Party's obligations.
>
> **Section 14. BUSINESS CONTINUITY AND FORCE MAJEURE**
> 14.1 Neither Party shall be liable for any failure or delay in performing its obligations under this Agreement to the extent that such failure or delay results from a Force Majeure Event. "Force Majeure Event" means any event beyond the reasonable control of the affected Party, including but not limited to: acts of God, natural disasters, epidemics, pandemics, war, terrorism, civil unrest, government actions or orders, labor strikes or lockouts, fire, flood, earthquake, power outages, telecommunications failures, cyberattacks, or supply chain disruptions.
> 14.2 The affected Party shall promptly notify the other Party in writing of the Force Majeure Event, its expected duration, and the obligations affected. The affected Party shall use commercially reasonable efforts to mitigate the impact of the Force Majeure Event and resume performance as soon as practicable.
> 14.3 If a Force Majeure Event continues for more than ninety (90) consecutive days, either Party may terminate this Agreement upon thirty (30) days' written notice without liability, other than for payment of Services rendered and expenses incurred prior to the effective date of termination.
>
> **Section 15. ENTIRE AGREEMENT AND AMENDMENTS**
> 15.1 This Agreement, together with all Exhibits and any Change Orders executed hereunder, constitutes the entire agreement between the Parties with respect to the subject matter hereof and supersedes all prior and contemporaneous agreements, representations, warranties, and understandings, whether written, oral, or implied.
> 15.2 No amendment, modification, or waiver of any provision of this Agreement shall be effective unless it is in writing and signed by authorized representatives of both Parties. No failure or delay by either Party in exercising any right or remedy shall be construed as a waiver thereof.
> 15.3 If any provision of this Agreement is held to be invalid, illegal, or unenforceable, the remaining provisions shall continue in full force and effect. The Parties shall negotiate in good faith to replace any invalid provision with a valid provision that most closely approximates the economic and legal intent of the original provision.
>
> **Section 16. AUDIT RIGHTS AND RECORD KEEPING**
> 16.1 The Client shall have the right, upon thirty (30) days' prior written notice and no more than once per calendar year, to audit the Provider's records, systems, and facilities to verify compliance with the terms of this Agreement, including but not limited to: (a) accuracy of invoices and time records; (b) compliance with data protection obligations; (c) adequacy of security measures; and (d) compliance with applicable laws and regulations.
> 16.2 The Provider shall maintain complete and accurate records of all Services performed, fees charged, expenses incurred, and personnel assigned under this Agreement for a period of seven (7) years following the expiration or termination of this Agreement. Such records shall be maintained in a manner that is readily accessible and auditable.
> 16.3 If any audit reveals a material discrepancy (defined as a variance of five percent (5%) or more) in fees charged, the Provider shall promptly refund the overcharged amount plus interest and shall bear the reasonable costs of the audit. If no material discrepancy is found, the Client shall bear the costs of the audit.
>
> **Section 17. COMMUNICATION AND NOTICES**
> 17.1 All notices, requests, demands, and other communications required or permitted under this Agreement shall be in writing and shall be deemed duly given: (a) upon personal delivery; (b) one (1) business day after deposit with a nationally recognized overnight courier; (c) three (3) business days after deposit in the mail, postage prepaid, certified or registered, return receipt requested; or (d) upon confirmation of receipt when sent by email to the addresses specified below.
> 17.2 Notices to the Client shall be addressed to: TechCorp Solutions GmbH, Attn: General Counsel, Friedrichstraße 123, 10117 Berlin, Germany. Email: legal@techcorp-solutions.example.com. Notices to the Provider shall be addressed to: LegalEdge Consulting AG, Attn: Managing Partner, Bahnhofstrasse 45, 8001 Zürich, Switzerland. Email: contracts@legaledge-consulting.example.com.
> 17.3 Either Party may change its notice address by providing written notice to the other Party in accordance with this Section.
>
> **Section 18. ORDER OF PRECEDENCE**
> 18.1 In the event of any conflict or inconsistency among the documents constituting this Agreement, the following order of precedence shall apply (in descending order of priority): (a) any duly executed Change Orders, in reverse chronological order; (b) the Data Processing Agreement (Exhibit D); (c) the body of this Agreement; (d) the Statement of Work (Exhibit A); (e) the Fee Schedule (Exhibit B); and (f) the Travel and Expense Policy (Exhibit C).
> 18.2 Notwithstanding the foregoing, mandatory provisions of applicable law shall take precedence over any conflicting provision of this Agreement.
>
> **Section 19. NON-SOLICITATION AND NON-COMPETITION**
> 19.1 During the Term and for a period of twelve (12) months following the expiration or termination of this Agreement (the "Restricted Period"), neither Party shall, directly or indirectly, solicit, recruit, or hire any employee, contractor, or consultant of the other Party who was involved in the performance of this Agreement, without the prior written consent of the other Party.
> 19.2 This restriction shall not apply to: (a) general recruitment advertising or job postings not specifically targeted at the other Party's personnel; or (b) situations where the individual initiates contact with the hiring Party without any solicitation.
> 19.3 In the event of a breach of this Section, the breaching Party shall pay the non-breaching Party liquidated damages equal to six (6) months' compensation of the solicited individual, which the Parties agree represents a reasonable estimate of the damages that would be incurred. Where the breach involves the solicitation of more than one individual within any twelve (12) month period, the non-breaching Party shall additionally be entitled to impose a systematic recruitment disruption penalty as quantified in Penalty Schedule N, which shall be cumulative with the per-individual liquidated damages set forth above.
>
> ---
>
> IN WITNESS WHEREOF, the Parties have executed this Agreement as of the Effective Date.
>
> **CLIENT: TechCorp Solutions GmbH**
> Signature: _________________________ Date: _____________
> Name: _________________________ Title: _____________
>
> **PROVIDER: LegalEdge Consulting AG**
> Signature: _________________________ Date: _____________
> Name: _________________________ Title: _____________

**Task on the webpage:** "Your legal team just received this 19-section draft contract. Before signing, you need to find every hidden penalty clause buried in the fine print. Open Gemini in the sidebar and ask: *Find all clauses in this contract that reference a Penalty Schedule. For each one, tell me the section number, penalty amount, reason and the Penalty Schedule letter.* List the Penalty Schedule letters in the order they appear — that spells your code word."

**Answer:** The 6 hidden penalty clauses and their Penalty Schedule references (in document order):

| Section | Hidden Penalty Description | Language Used | Schedule |
|---------|---------------------------|---------------|----------|
| 1.3 | Short-notice termination charge | "supplementary administrative charge" | **B** |
| 3.5 | Excess revision surcharge | "excess revision surcharge" | **E** |
| 5.4 | Delayed access idle-cost deduction | "resource reallocation deduction" | **A** |
| 8.3 | Warranty non-conformance fee | "remediation fee" | **C** |
| 11.4 | Client-caused data breach levy | "accelerated compliance levy" | **O** |
| 19.3 | Mass solicitation penalty | "systematic recruitment disruption penalty" | **N** |

Schedule letters in order: B-E-A-C-O-N → **BEACON**

> **Why Ctrl+F won't work:** Each penalty uses completely different language — "surcharge", "deduction", "remediation fee", "levy", "penalty", "charge". A keyword search only catches one or two. Gemini understands the semantic concept of "financial penalty" regardless of wording.

**Code word: BEACON**

---

### Station 2: "The Contract Portfolio Review" (Gemini in Google Sheets)

**Skill taught:** Using Gemini to query a contract portfolio tracker — the exact task legal ops and in-house counsel perform monthly to catch expiring contracts before they silently auto-renew

**Why Gemini is essential:** The spreadsheet has 50 contracts across 10 columns. The question requires combining date math (expires within next 3 months), a boolean check (auto-renewal = Yes), AND a status check (compliance certification = Expired) — simultaneously across 50 rows. Regular Sheets filters can't do date-range calculations naturally. Gemini handles it with a single natural-language question, which is exactly how a GC would want to query their contract tracker.

**Setup:** Create a Google Sheet called "Station 2 — Contract Portfolio Tracker" with this data (10 columns, 50 rows). Copy-paste into Google Sheets — make sure all rows look identical (no bolding or highlighting).

**Important:** Tell participants that today's date is **March 29, 2026** (so "next 3 months" means before July 1, 2026).

| Counterparty | Contract Type | Effective Date | Expiry Date | Annual Value (€) | Auto-Renewal | Notice Period (days) | Governing Law | Compliance Cert | Assigned Lawyer |
|---|---|---|---|---|---|---|---|---|---|
| Albrecht & Söhne GmbH | Services | 2024-04-01 | 2027-03-31 | 180,000 | Yes | 90 | Germany | Valid | M. Weber |
| Alpine Digital AG | SaaS License | 2023-07-15 | 2026-07-14 | 95,000 | Yes | 60 | Switzerland | Valid | K. Richter |
| Arcadia Consulting | Advisory | 2024-01-10 | 2026-01-09 | 120,000 | No | 30 | England | Expired | A. Novak |
| Athena Risk Solutions | Managed Services | 2023-09-01 | 2026-08-31 | 340,000 | Yes | 90 | Germany | Expired | M. Weber |
| Baltic Data Systems | Data Processing | 2024-06-15 | 2026-06-14 | 210,000 | Yes | 60 | Estonia | Valid | K. Richter |
| Bayerische Compliance AG | Advisory | 2023-03-20 | 2026-03-19 | 165,000 | No | 90 | Germany | Expired | A. Novak |
| Benelux Legal Partners | Services | 2024-08-01 | 2026-07-31 | 275,000 | Yes | 90 | Belgium | Valid | M. Weber |
| Bratislava Tech s.r.o. | SaaS License | 2023-11-01 | 2026-10-31 | 88,000 | Yes | 30 | Slovakia | Valid | K. Richter |
| Cambridge Analytics Ltd. | Data Processing | 2024-02-15 | 2027-02-14 | 430,000 | Yes | 120 | England | Valid | A. Novak |
| Cascadia Procurement Inc. | Services | 2023-05-10 | 2026-05-09 | 195,000 | No | 60 | USA (NY) | Expired | M. Weber |
| ClearView Compliance B.V. | Managed Services | 2024-09-01 | 2026-08-31 | 155,000 | Yes | 60 | Netherlands | Valid | K. Richter |
| Danubia Legal Kft. | Advisory | 2023-06-01 | 2026-05-31 | 72,000 | Yes | 30 | Hungary | Valid | A. Novak |
| Dresden Innovations GmbH | SaaS License | 2024-03-15 | 2027-03-14 | 310,000 | Yes | 90 | Germany | Valid | M. Weber |
| **Eastbridge Compliance** | **Managed Services** | **2023-06-15** | **2026-06-12** | **275,000** | **Yes** | **60** | **Singapore** | **Expired** | **K. Richter** |
| Edinburgh Partners LLP | Advisory | 2024-01-20 | 2026-07-19 | 198,000 | Yes | 90 | Scotland | Valid | A. Novak |
| Europa Consulting S.A. | Services | 2023-08-01 | 2026-07-31 | 245,000 | Yes | 60 | Luxembourg | Expired | M. Weber |
| **Foxcroft Data Services** | **SaaS License** | **2023-04-15** | **2026-04-05** | **185,000** | **Yes** | **90** | **England** | **Expired** | **M. Weber** |
| Frankfurt Legal Tech GmbH | Data Processing | 2024-07-01 | 2027-06-30 | 520,000 | Yes | 120 | Germany | Valid | K. Richter |
| Galleria Procurement S.r.l. | Services | 2023-10-15 | 2026-04-14 | 135,000 | No | 60 | Italy | Expired | A. Novak |
| Geneva Advisory SA | Advisory | 2024-04-01 | 2026-09-30 | 290,000 | Yes | 90 | Switzerland | Valid | M. Weber |
| **Grayson & Partners** | **Advisory** | **2024-06-01** | **2026-05-20** | **145,000** | **Yes** | **60** | **Germany** | **Expired** | **M. Weber** |
| Hamburg Digital GmbH | SaaS License | 2023-12-01 | 2026-11-30 | 167,000 | Yes | 60 | Germany | Valid | K. Richter |
| Helios Managed Services | Managed Services | 2024-05-15 | 2026-05-14 | 380,000 | Yes | 90 | Greece | Valid | A. Novak |
| Iberia Compliance S.L. | Advisory | 2023-07-20 | 2026-07-19 | 110,000 | Yes | 30 | Spain | Expired | M. Weber |
| InsightLaw AB | Services | 2024-10-01 | 2026-09-30 | 92,000 | No | 60 | Sweden | Valid | K. Richter |
| Kairos Procurement Ltd. | Services | 2023-04-01 | 2026-03-31 | 205,000 | Yes | 60 | England | Expired | A. Novak |
| Krakow Systems Sp. z o.o. | Data Processing | 2024-02-01 | 2027-01-31 | 148,000 | Yes | 90 | Poland | Valid | M. Weber |
| Lakeshore Advisory Inc. | Advisory | 2023-06-15 | 2026-06-14 | 260,000 | Yes | 60 | USA (DE) | Valid | K. Richter |
| Lausanne Partners SA | Services | 2024-01-01 | 2026-12-31 | 175,000 | Yes | 90 | Switzerland | Valid | A. Novak |
| Lyon Digital SAS | SaaS License | 2023-09-15 | 2026-09-14 | 132,000 | Yes | 60 | France | Valid | M. Weber |
| Meridian Legal Consulting | Advisory | 2024-03-01 | 2026-08-31 | 88,000 | No | 30 | Ireland | Valid | K. Richter |
| Munich Re-Solutions GmbH | Managed Services | 2023-10-01 | 2026-03-31 | 445,000 | Yes | 120 | Germany | Valid | A. Novak |
| Nordic Procurement AB | Services | 2024-08-15 | 2026-08-14 | 168,000 | Yes | 60 | Sweden | Expired | M. Weber |
| **Oakmont Solutions AG** | **Consulting** | **2024-04-20** | **2026-04-18** | **220,000** | **Yes** | **60** | **Switzerland** | **Expired** | **K. Richter** |
| Oslo Analytics AS | Data Processing | 2023-11-15 | 2026-05-14 | 195,000 | No | 90 | Norway | Valid | A. Novak |
| Pannonia Services Kft. | Services | 2024-07-01 | 2026-06-30 | 78,000 | Yes | 30 | Hungary | Valid | M. Weber |
| Porto Compliance Lda. | Advisory | 2023-05-01 | 2026-04-30 | 105,000 | Yes | 60 | Portugal | Valid | K. Richter |
| Rhenania Consulting GmbH | Advisory | 2024-06-15 | 2026-06-14 | 235,000 | No | 90 | Germany | Expired | A. Novak |
| **Riverdale Analytics** | **Data Processing** | **2023-05-10** | **2026-05-02** | **310,000** | **Yes** | **90** | **USA (NY)** | **Expired** | **A. Novak** |
| Roma Legal Services S.r.l. | Services | 2024-09-15 | 2026-09-14 | 142,000 | Yes | 60 | Italy | Valid | M. Weber |
| Scandia Partners AB | Managed Services | 2023-08-01 | 2026-07-31 | 298,000 | Yes | 90 | Sweden | Valid | K. Richter |
| Silesia Tech Sp. z o.o. | SaaS License | 2024-05-01 | 2026-04-30 | 118,000 | Yes | 30 | Poland | Valid | A. Novak |
| Stuttgart Innovations GmbH | Data Processing | 2023-12-15 | 2026-06-14 | 365,000 | Yes | 90 | Germany | Valid | M. Weber |
| Tallinn Digital OÜ | SaaS License | 2024-01-15 | 2026-07-14 | 79,000 | Yes | 30 | Estonia | Expired | K. Richter |
| Vienna Procurement GmbH | Services | 2023-07-01 | 2026-06-30 | 225,000 | Yes | 60 | Austria | Valid | A. Novak |
| Vilnius Advisory UAB | Advisory | 2024-04-15 | 2026-10-14 | 95,000 | No | 60 | Lithuania | Valid | M. Weber |
| Warsaw Compliance Sp. z o.o. | Managed Services | 2023-10-20 | 2026-04-19 | 188,000 | Yes | 60 | Poland | Valid | K. Richter |
| Zürich Data AG | Data Processing | 2024-02-28 | 2027-02-27 | 410,000 | Yes | 120 | Switzerland | Valid | A. Novak |

> **Note:** Do NOT bold the rows in the actual spreadsheet — they're bolded here only to show you which 5 contracts match ALL 3 criteria. In the real sheet, all 50 rows must look identical.
>
> **The 5 contracts matching ALL 3 criteria** (expiry before Jul 1 2026 + auto-renewal Yes + compliance Expired):
> - **F**oxcroft Data Services — expires 2026-04-05
> - **O**akmont Solutions AG — expires 2026-04-18
> - **R**iverdale Analytics — expires 2026-05-02
> - **G**rayson & Partners — expires 2026-05-20
> - **E**astbridge Compliance — expires 2026-06-12
>
> **Deliberate near-misses** (match 2 of 3 criteria but not all 3):
> - Athena Risk Solutions — Auto-renewal Yes + Expired, but expires **2026-08-31** (too late)
> - Bayerische Compliance AG — Expired + expires before Jul 2026, but Auto-renewal = **No**
> - Cascadia Procurement Inc. — Expired + expires before Jul 2026, but Auto-renewal = **No**
> - Europa Consulting S.A. — Auto-renewal Yes + Expired, but expires **2026-07-31** (too late)
> - Galleria Procurement S.r.l. — Expired + expires before Jul 2026, but Auto-renewal = **No**
> - Iberia Compliance S.L. — Auto-renewal Yes + Expired, but expires **2026-07-19** (too late)
> - Kairos Procurement Ltd. — Auto-renewal Yes + Expired, but expires **2026-03-31** (already expired by the exercise date of Mar 29 — judgment call; accept if included)
> - Nordic Procurement AB — Auto-renewal Yes + Expired, but expires **2026-08-14** (too late)
> - Rhenania Consulting GmbH — Expired + expires before Jul 2026, but Auto-renewal = **No**
> - Tallinn Digital OÜ — Auto-renewal Yes + Expired, but expires **2026-07-14** (too late)

**Task:** "Use Gemini in the sidebar and ask: *Today's date is March 29, 2026. Which contracts expire within the next 3 months (before July 1, 2026), have auto-renewal enabled, AND have an expired compliance certification? These are contracts that will silently auto-renew without proper compliance. Sort results by expiry date, earliest first. Create a short table here in the chat.*

Take the **first letter of each counterparty name** and read them together — that's your code word."

**Answer:** The 5 contracts matching all 3 criteria (sorted by expiry date):
- **F**oxcroft Data Services (expires 2026-04-05)
- **O**akmont Solutions AG (expires 2026-04-18)
- **R**iverdale Analytics (expires 2026-05-02)
- **G**rayson & Partners (expires 2026-05-20)
- **E**astbridge Compliance (expires 2026-06-12)

First letters: F-O-R-G-E → **FORGE**

**Code word: FORGE**

---

### Station 3: "The Scrambled Brief" (Gemini in Gmail / Gemini chat)

**Skill taught:** Using Gemini to rewrite and structure text

**Setup:** Give participants this scrambled, poorly written email text (printed card or in a shared doc):

> hi so basically the client called and theyre upset about the contract thing from last week where the delivery dates got mixed up and also they think the penalty clause is too harsh and they want to renegotiate but our sales team already promised them different terms verbally which we never put in writing and now legal needs to sort this out before thursday or the client says theyll walk and also procurement wants to know if we can just extend the existing framework agreement instead of doing a whole new contract which would save time but im not sure if thats compliant with our policies can someone please advise asap thanks

**Task:** "Open Gemini (gemini.google.com) and ask it to: *Rewrite this as a structured legal memo with clear action items, addressed to the Legal Department.* In your polished memo, count the number of distinct action items Gemini identifies. That number is your code."

**Answer:** Gemini typically identifies **5** action items (may vary slightly, accept 4–6):
1. Clarify delivery date discrepancy
2. Review penalty clause terms
3. Document verbal commitments from sales
4. Evaluate framework agreement extension for compliance
5. Respond before Thursday deadline

**Code word: FIVE**

---

### Station 4: "The Negotiation Thread" (Gemini in Google Docs)

**Skill taught:** Using Gemini to analyze a long email thread and identify who made binding commitments — the #1 risk in contract negotiations, and a task in-house counsel perform constantly

**Why Gemini is essential:** The Google Doc contains a 15-email thread between 10 people (sales, legal, finance, IT, procurement, and the vendor). Buried among the back-and-forth are 5 people who made informal but binding commitments on behalf of the company — promised timelines, agreed to terms, authorized access, or locked in payment conditions. Reading 15 emails and distinguishing "just discussing" from "actually committed" is exactly the kind of judgment task that Gemini handles well. A GC reviewing this thread before contract execution needs to know: who promised what?

**Setup:** Create a Google Doc called "Station 4 — Vendor Negotiation Thread" and paste the email chain below. Format each email with **From/To/Date/Subject** headers to look like a printed email thread.

> ---
>
> **From:** James O'Brien (james.obrien@cloudplatform.example.com)
> **To:** Thomas Weber (thomas.weber@techcorp.example.com)
> **Date:** March 3, 2026, 09:14
> **Subject:** RE: CloudPlatform SaaS Agreement — Draft Contract
>
> Hi Thomas,
>
> Great speaking with you last week. As discussed, please find attached our standard SaaS Agreement for the CloudPlatform Enterprise Suite. I've included our standard terms for data hosting, SLA commitments, and pricing.
>
> Happy to set up a call with your legal team to walk through any questions. Looking forward to working together.
>
> Best regards,
> James O'Brien, VP Sales — CloudPlatform Inc.
>
> ---
>
> **From:** Thomas Weber (thomas.weber@techcorp.example.com)
> **To:** Sarah Chen, Patrick Müller, Anna Kovacs, Robert Singh, Klara Jansen, Lisa Fernandez, David Park, Maria Santos
> **CC:** James O'Brien
> **Date:** March 3, 2026, 11:30
> **Subject:** FW: CloudPlatform SaaS Agreement — Draft Contract
>
> Team,
>
> FYI — CloudPlatform has sent over their draft contract for the Enterprise Suite we discussed in last month's steering committee. I've forwarded the attachment.
>
> Can each of you please review from your respective angles? Key areas:
> - Sarah: project timeline and go-live readiness
> - Patrick: fee structure and budget alignment
> - Anna: legal terms, liability, governing law
> - Robert: data security and hosting requirements
> - Klara: payment processing and accounts payable setup
> - Maria: vendor onboarding and procurement compliance
> - David/Lisa: technical specs and integration requirements
>
> Let's aim to have feedback consolidated by end of next week. Thanks.
>
> Thomas Weber, Head of Business Development — TechCorp Solutions GmbH
>
> ---
>
> **From:** David Park (david.park@techcorp.example.com)
> **To:** Thomas Weber
> **CC:** all
> **Date:** March 4, 2026, 08:45
> **Subject:** RE: CloudPlatform SaaS Agreement — Draft Contract
>
> Thomas,
>
> I've reviewed the technical specifications in Annex 2. The platform meets our integration requirements — API compatibility looks good, and their uptime SLA of 99.9% is in line with what we need. No concerns from the IT architecture side.
>
> One question: do we know if they support SSO via our existing Azure AD setup? I'll check with their tech team directly if needed.
>
> David
>
> ---
>
> **From:** Maria Santos (maria.santos@techcorp.example.com)
> **To:** Thomas Weber
> **CC:** all
> **Date:** March 4, 2026, 14:22
> **Subject:** RE: CloudPlatform SaaS Agreement — Draft Contract
>
> Hi Thomas,
>
> From a procurement perspective, I've benchmarked their pricing against three comparable SaaS providers in our vendor database. Their annual fee of EUR 420,000 is approximately 12-15% above market rate for similar enterprise platforms. I'd suggest we push back on the fee structure — there's room to negotiate.
>
> Also, they're not yet in our approved vendor registry. I'll need a completed vendor questionnaire and evidence of ISO 27001 certification before I can process the onboarding. I've sent the forms to James directly.
>
> Maria Santos, Senior Procurement Manager — TechCorp Solutions GmbH
>
> ---
>
> **From:** Sarah Chen (sarah.chen@techcorp.example.com)
> **To:** Thomas Weber, James O'Brien
> **CC:** all
> **Date:** March 5, 2026, 10:08
> **Subject:** RE: CloudPlatform SaaS Agreement — Timeline Confirmation
>
> Hi James, Thomas,
>
> Following our project planning session yesterday, I want to confirm the timeline we discussed. I've committed our team to having the data migration environment ready by August 15, 2026, and I've confirmed with our department heads that we will be fully operational on the CloudPlatform system by September 1, 2026. I've already blocked the resources on our side and notified our current vendor of the planned transition.
>
> James — you mentioned your implementation team needs 6 weeks of lead time. Based on our September 1 go-live, that means we'd need your team to start onboarding by mid-July. Can you confirm that works on your end?
>
> Sarah Chen, Project Lead — Digital Transformation — TechCorp Solutions GmbH
>
> ---
>
> **From:** Lisa Fernandez (lisa.fernandez@techcorp.example.com)
> **To:** Anna Kovacs, Patrick Müller
> **CC:** Thomas Weber
> **Date:** March 6, 2026, 09:15
> **Subject:** FW: CloudPlatform SaaS Agreement — Draft Contract
>
> Hi Anna, Patrick,
>
> Forwarding this to make sure it's on your radar. Thomas mentioned the legal and finance review is the critical path right now. Let me know if you need me to set up any calls with the CloudPlatform team.
>
> Lisa
>
> ---
>
> **From:** Patrick Müller (patrick.mueller@techcorp.example.com)
> **To:** Thomas Weber, James O'Brien
> **CC:** all
> **Date:** March 7, 2026, 16:45
> **Subject:** RE: CloudPlatform SaaS Agreement — Fee Structure
>
> Thomas, James,
>
> I've completed the financial review. Based on Maria's benchmarking and our budget allocation, I spoke with James's CFO, Diana Torres, this morning. We've agreed that the total annual spend will be capped at EUR 400,000 for the first two contract years, with a structured review mechanism in Year 3 tied to usage metrics. I've confirmed that our budget can accommodate this for FY2026 and FY2027, and I've allocated the funds in our financial planning system.
>
> James — Diana mentioned she'll update Section 4 of the contract to reflect the revised pricing. Can you send us the updated version?
>
> Patrick Müller, Head of Finance & Controlling — TechCorp Solutions GmbH
>
> ---
>
> **From:** James O'Brien (james.obrien@cloudplatform.example.com)
> **To:** Patrick Müller, Thomas Weber
> **CC:** all
> **Date:** March 8, 2026, 10:30
> **Subject:** RE: CloudPlatform SaaS Agreement — Fee Structure
>
> Patrick,
>
> Confirmed — Diana is updating the pricing section now. We'll have the revised draft over to you by Monday. Thanks for working through this so efficiently.
>
> James
>
> ---
>
> **From:** Thomas Weber (thomas.weber@techcorp.example.com)
> **To:** Robert Singh
> **CC:** all
> **Date:** March 10, 2026, 08:15
> **Subject:** RE: CloudPlatform SaaS Agreement — Data Hosting Question
>
> Robert,
>
> James asked if we can confirm the data hosting location requirements. Their standard setup is multi-region (Frankfurt + Dublin), but they can do single-region if we need it for compliance. Can you weigh in on what we need from a data protection perspective?
>
> Thomas
>
> ---
>
> **From:** Anna Kovacs (anna.kovacs@techcorp.example.com)
> **To:** Thomas Weber, James O'Brien
> **CC:** all
> **Date:** March 10, 2026, 14:30
> **Subject:** RE: CloudPlatform SaaS Agreement — Legal Review Update
>
> Thomas, James,
>
> I've completed my initial review of the contract. I have redline comments on Sections 8 (Limitation of Liability), 11 (Data Protection), and 14 (Termination). I'll send the full markup by end of day tomorrow.
>
> One preliminary concern: their standard liability cap is set at 1x annual contract value, which is below our minimum threshold. I'll need to negotiate this upward. Also, the draft specifies Swiss law as governing law with Zurich arbitration — I'd strongly prefer German law with Frankfurt arbitration given our headquarters location.
>
> Will schedule a call with their legal team for later this week.
>
> Anna Kovacs, Senior Legal Counsel — TechCorp Solutions GmbH
>
> ---
>
> **From:** Robert Singh (robert.singh@techcorp.example.com)
> **To:** Thomas Weber, James O'Brien
> **CC:** all
> **Date:** March 15, 2026, 11:20
> **Subject:** RE: CloudPlatform SaaS Agreement — Security & Data Hosting
>
> Thomas, James,
>
> I've completed the security assessment review. Confirmed with CloudPlatform's CISO that all data will be hosted exclusively in the Frankfurt data center — single region, EU-only. This satisfies our GDPR requirements and internal data residency policy.
>
> To move things forward, I've authorized CloudPlatform to begin their pre-onboarding security audit. I've granted their security team access to our penetration testing environment and shared the VPN credentials for the sandbox. They should be able to start the technical assessment by end of this week.
>
> Robert Singh, Data Protection Officer — TechCorp Solutions GmbH
>
> ---
>
> **From:** Anna Kovacs (anna.kovacs@techcorp.example.com)
> **To:** Thomas Weber, James O'Brien
> **CC:** all
> **Date:** March 14, 2026, 17:10
> **Subject:** RE: CloudPlatform SaaS Agreement — Legal Terms Agreed
>
> All,
>
> Good news. I had a productive call with CloudPlatform's General Counsel, Mark Stevens, this afternoon. We've reached agreement on the key legal terms:
>
> After extensive negotiation, I've accepted their limitation of liability at 2x the annual contract value (up from their standard 1x). I've also agreed that German law will govern the agreement, with arbitration seated in Frankfurt under ICC rules. Their original draft had Swiss law — this is a significantly better outcome for us.
>
> I've also secured a mutual audit right (Section 16) and strengthened the data breach notification window from 72 hours to 48 hours.
>
> Mark is sending the revised contract reflecting all changes by Monday. I recommend we move to signature once Patrick and Klara have confirmed the financial and payment terms.
>
> Anna Kovacs, Senior Legal Counsel — TechCorp Solutions GmbH
>
> ---
>
> **From:** James O'Brien (james.obrien@cloudplatform.example.com)
> **To:** Anna Kovacs, Thomas Weber
> **CC:** all
> **Date:** March 15, 2026, 09:00
> **Subject:** RE: CloudPlatform SaaS Agreement — Legal Terms Agreed
>
> Anna,
>
> Thanks — we're aligned. Mark will have the updated version to you on Monday as promised. Can someone on your side confirm the payment terms and schedule so we can finalize everything in one round?
>
> James
>
> ---
>
> **From:** Klara Jansen (klara.jansen@techcorp.example.com)
> **To:** James O'Brien, Thomas Weber
> **CC:** all
> **Date:** March 17, 2026, 13:45
> **Subject:** RE: CloudPlatform SaaS Agreement — Payment Schedule Confirmed
>
> Hi James, Thomas,
>
> I've set up the payment schedule in our SAP system. We will process quarterly payments of EUR 100,000 each, with the first payment due 30 days after the go-live date. I've committed our accounts payable department to NET-30 terms for all invoices under this agreement, and I've added CloudPlatform to our automatic payment run.
>
> James — please make sure your invoicing matches this quarterly schedule. Our system will reject invoices that don't align with the agreed billing periods.
>
> Klara Jansen, Head of Accounts Payable — TechCorp Solutions GmbH
>
> ---
>
> **From:** Maria Santos (maria.santos@techcorp.example.com)
> **To:** Thomas Weber
> **CC:** all
> **Date:** March 18, 2026, 10:00
> **Subject:** RE: CloudPlatform SaaS Agreement — Vendor Onboarding Status
>
> Thomas,
>
> Quick update on onboarding status: I've received CloudPlatform's completed vendor questionnaire and their ISO 27001 certificate. Both check out. The vendor registration is in progress — I'll need the fully executed contract before I can close out the procurement file.
>
> No further action required from my side until then. Everything looks good to proceed to signature.
>
> Maria Santos, Senior Procurement Manager — TechCorp Solutions GmbH

**Task on the webpage:** "Open the Google Doc with the email thread. Use the Gemini sidebar and ask: *Which people in this email thread made a binding commitment or promise on behalf of TechCorp? A binding commitment means they confirmed a specific timeline, agreed to contract terms, authorized access to systems, or locked in financial conditions — not just providing information, asking questions, or forwarding emails. List only the people who made commitments, in chronological order by the date of their commitment.*

Take the **first letter of each person's FIRST NAME** and read them together — that's your code word."

**Answer:** The 5 people who made binding commitments (in chronological order):

| Person | Email Date | What They Committed | Type |
|--------|-----------|-------------------|------|
| **S**arah Chen | Mar 5 | Confirmed go-live date of Sep 1 and data migration readiness by Aug 15; notified current vendor | Timeline commitment |
| **P**atrick Müller | Mar 7 | Agreed to EUR 400K annual cap with vendor's CFO; allocated budget in planning system | Financial commitment |
| **A**nna Kovacs | Mar 14 | Accepted 2x liability cap; agreed to German law / Frankfurt arbitration | Legal terms commitment |
| **R**obert Singh | Mar 15 | Authorized pre-onboarding security audit; granted VPN and pen-test access | System access authorization |
| **K**lara Jansen | Mar 17 | Set up quarterly EUR 100K payments; committed AP department to NET-30 terms | Payment terms commitment |

Chronological order: Sarah (Mar 5) → Patrick (Mar 7) → Anna (Mar 14) → Robert (Mar 15) → Klara (Mar 17) = **S-P-A-R-K**

> **People who did NOT make commitments** (and why — for organizer reference):
> - Thomas Weber — only forwarded emails and asked questions; made no promises
> - David Park — reported technical findings; no commitment or authorization
> - Lisa Fernandez — forwarded the thread; no substantive action
> - Maria Santos — provided benchmarking data and onboarding status; stated "no action from my side"
> - James O'Brien — vendor counterpart, not a TechCorp representative

First letters (chronological): S-P-A-R-K → **SPARK**

**Code word: SPARK**

---

### Station 5: "The Final Key" (Combining code words)

**Skill taught:** Putting it all together

The treasure hunt webpage handles this station. Teams enter their 4 code words:
- **BEACON** (Station 1)
- **FORGE** (Station 2)
- **FIVE** (Station 3)
- **SPARK** (Station 4)

The webpage reveals the GitHub repository link: **https://github.com/tjgehmann/legalhackathon**

---

## Tips for Organizers

- **Print station cards** with the instructions for each station — don't rely solely on the webpage
- **Have helpers** at each station to assist teams who get stuck with Gemini
- **Gemini availability:** Make sure all participants have Gemini enabled in their Google Workspace. Test this beforehand!
- **Flexibility on answers:** Station 3 (the email rewrite) may produce varying numbers of action items. Accept reasonable answers (4–6)
- **Time limit:** Give teams ~8 minutes per station, with a 5-minute buffer
- **Prizes:** Consider a small prize for the first team to unlock the GitHub link

## Fallback Plan

If Gemini is unavailable or slow:
- Provide the code words directly after teams attempt each task
- The learning goal (trying the tool) is more important than getting the exact answer
