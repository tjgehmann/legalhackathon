# COURT DECISION

## European Court of Justice — Case C-412/24 (Fictional)

**DataFlow International Ltd v. Bundesbeauftragter für den Datenschutz und die Informationsfreiheit (BfDI)**

**Date of Judgment:** October 15, 2025

**Subject:** Validity of supplementary measures for international data transfers under Standard Contractual Clauses; obligations of data exporters in assessing third-country legal frameworks

---

### SUMMARY OF FACTS

1. DataFlow International Ltd ("DataFlow"), a UK-incorporated cloud computing company, provides data analytics services to customers across the European Union. Following Brexit, DataFlow continued to process personal data of EU data subjects through its UK data centers and, for certain processing operations, through subprocessors located in India and the Philippines.

2. DataFlow relied on Standard Contractual Clauses (SCCs) approved by the European Commission Decision 2021/914 as the legal basis for transferring personal data from its EU customers to its processing facilities in the UK, India, and the Philippines. DataFlow conducted a Transfer Impact Assessment (TIA) in 2022 which concluded that the legal frameworks in all three countries provided adequate protections, supplemented by technical measures including encryption in transit and at rest.

3. The Bundesbeauftragter für den Datenschutz und die Informationsfreiheit (BfDI), the German Federal Commissioner for Data Protection, commenced an investigation following a complaint by a German data subject whose personal data was processed by DataFlow's subprocessor in India. The data subject alleged that the transfer lacked adequate safeguards, as Indian data protection law at the time did not provide an adequate level of protection as determined by the European Commission.

4. Following its investigation, the BfDI issued a decision ordering DataFlow to (a) cease all transfers of EU personal data to its Indian subprocessor, (b) pay an administrative fine of EUR 2,300,000, and (c) implement additional safeguards for its UK transfers. The BfDI found that DataFlow's Transfer Impact Assessment was insufficient because it (i) did not adequately assess the Indian government's surveillance capabilities and access rights, (ii) relied on encryption as a supplementary measure without demonstrating that encryption keys were inaccessible to the Indian subprocessor, and (iii) failed to reassess its TIA following changes to Indian data protection legislation.

5. DataFlow appealed the BfDI's decision. The German administrative court referred several questions to the European Court of Justice for a preliminary ruling.

---

### QUESTIONS REFERRED

The referring court submitted the following questions to the ECJ:

1. **Must a data exporter relying on Standard Contractual Clauses conduct a new Transfer Impact Assessment each time there is a material change in the legal framework of the third country, even if the change is generally viewed as an improvement in data protection standards?**

2. **What level of detail and specificity is required in a Transfer Impact Assessment to satisfy the obligations under Articles 44–49 GDPR, particularly regarding the assessment of government surveillance laws and access rights in the third country?**

3. **Can encryption alone constitute a sufficient supplementary measure under SCCs where the data importer or subprocessor has potential access to encryption keys, even if contractual provisions prohibit such access?**

4. **Does the principle of accountability under Article 5(2) GDPR require the data exporter to independently verify the data importer's representations about the legal framework in the third country, or may the exporter reasonably rely on the importer's self-assessment?**

---

### JUDGMENT

The Court, sitting as the Grand Chamber, rules as follows:

**On the First Question**

5. The Court observes that the obligation to ensure an essentially equivalent level of protection for personal data transferred to third countries is a continuing obligation, not a one-time assessment at the point of transfer. The data exporter must monitor relevant developments in the legal framework of the receiving country on an ongoing basis.

6. However, the Court clarifies that this does not require a formal reassessment in response to every legislative change. A material change in the legal framework — that is, a change that could reasonably affect the level of protection afforded to the transferred data — triggers the obligation to reassess. The data exporter must exercise diligence and judgment in determining whether a change is material.

7. The Court notes that even a change generally perceived as an improvement in data protection standards (such as the enactment of a new comprehensive data protection law) may introduce new provisions or exceptions that could negatively impact the protection of transferred data. Therefore, **the direction of the change is not determinative; what matters is whether the change is material to the protection of the specific data being transferred.**

8. The Court rules that **a data exporter relying on SCCs must reassess the adequacy of its safeguards whenever there is a material change in the legal framework of the third country, regardless of whether the change is generally viewed as positive or negative.**

**On the Second Question**

9. The Court holds that a Transfer Impact Assessment must go beyond a general overview of the third country's data protection framework. It must include:

   (a) **A specific assessment of the laws and practices governing government access to personal data**, including surveillance legislation, national security laws, and law enforcement access provisions. The assessment must consider not only the text of the law but also publicly available information about its practical application.

   (b) **An analysis of the data importer's specific circumstances**, including the sector in which it operates, the type of data being transferred, and whether the data importer has received government access requests in the past.

   (c) **An evaluation of the effectiveness of the supplementary measures** adopted to address any identified gaps, taking into account the specific risks identified in the assessment.

   (d) **Documentation of the methodology used** to conduct the assessment, including the sources consulted, the experts involved, and the reasoning leading to the conclusions.

10. The Court emphasizes that the level of detail required is proportionate to the risk. Transfers involving sensitive data, large volumes of data, or data subjects in vulnerable situations require more rigorous assessments.

11. The Court concludes that **a Transfer Impact Assessment that consists primarily of a general description of the third country's legal framework, without specific analysis of government access laws and the effectiveness of supplementary measures, does not satisfy the requirements of Articles 44–49 GDPR.**

**On the Third Question**

12. The Court addresses the sufficiency of encryption as a supplementary measure. It notes that encryption is widely recognized as an important technical safeguard, but its effectiveness depends entirely on the implementation.

13. The Court holds that **encryption can constitute an effective supplementary measure only if the encryption keys are under the exclusive control of the data exporter or a party located in a jurisdiction providing an adequate level of protection.** If the data importer or subprocessor has the technical ability to access the encryption keys — even if contractual provisions prohibit such access — the encryption cannot be considered an effective supplementary measure against government access in the third country.

14. The Court reasons that contractual prohibitions, while relevant, cannot override legal obligations imposed by the third country's government. If the third country's law could compel the data importer to provide access to encryption keys, a contractual prohibition alone does not provide an adequate safeguard.

15. The Court notes that in such cases, additional technical measures may be necessary, such as:
   (a) split-key encryption where no single party has access to the complete key;
   (b) processing of pseudonymized data where the re-identification data is retained exclusively in the EU;
   (c) the use of secure multi-party computation or other privacy-enhancing technologies.

**On the Fourth Question**

16. The Court holds that the principle of accountability under Article 5(2) GDPR requires the data exporter to take an **active role** in assessing the legal framework of the third country. While the data exporter may take into account the representations and information provided by the data importer, it may not **solely rely** on such representations without independent verification.

17. The Court specifies that independent verification may take various forms, including:
   (a) consultation of publicly available legal analyses and government reports;
   (b) engagement of independent legal experts with knowledge of the third country's legal framework;
   (c) review of supervisory authority guidance on transfers to the specific third country;
   (d) consideration of the European Data Protection Board's adequacy referentials.

18. The Court acknowledges that perfect knowledge of a third country's legal framework cannot be expected, but the data exporter must demonstrate that it has taken **reasonable and documented steps** to independently verify the key aspects of the assessment, particularly regarding government access laws.

---

### RULING

The Court rules:

1. A data exporter relying on Standard Contractual Clauses must reassess the adequacy of its safeguards whenever there is a material change in the legal framework of the third country, regardless of whether the change is generally perceived as an improvement.

2. A Transfer Impact Assessment must include a specific analysis of government access laws, the data importer's circumstances, the effectiveness of supplementary measures, and must document the methodology used. General descriptions of the third country's legal framework are insufficient.

3. Encryption constitutes an effective supplementary measure only if the encryption keys are under the exclusive control of the data exporter or a party in a jurisdiction with adequate protection. Contractual prohibitions on key access do not suffice where local law could compel disclosure.

4. The accountability principle requires data exporters to independently verify the data importer's representations about the third-country legal framework through reasonable and documented steps.

---

### COSTS

The costs incurred by the German Government, the European Commission, and the European Data Protection Board, which submitted observations to the Court, are not recoverable. Since the proceedings constitute, for the parties to the main proceedings, a step in the proceedings before the referring court, the decision on costs is a matter for that court.

---

*Done at Luxembourg, October 15, 2025.*
