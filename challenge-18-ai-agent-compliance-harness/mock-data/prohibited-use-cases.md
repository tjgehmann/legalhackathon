# Prohibited AI Practices Under the EU AI Act
## Plain-Language Guide for Internal Governance

*Article 5 of Regulation (EU) 2024/1689 — applies from 2 February 2025.*
*These prohibitions are absolute. No business justification, contractual clause, or consent mechanism overrides them.*

---

## Overview

The EU AI Act prohibits eight categories of AI practice outright. Unlike the high-risk framework (which allows deployment subject to safeguards), prohibited practices **cannot be made compliant** — they must be stopped entirely.

Below each prohibition is a translation into realistic company scenarios, so teams can recognize prohibited practices when they see them.

---

## 1. Subliminal or Manipulative Techniques
**Legal text (Art. 5(1)(a)):** AI systems that deploy subliminal techniques beyond a person's consciousness, or that intentionally manipulate or deceive, causing or likely to cause significant harm.

**What this means in practice:**
- A customer-facing chatbot designed to create artificial urgency ("Only 2 left — decide now!") using psychological pressure tactics the customer can't consciously identify → **PROHIBITED** if designed to exploit rather than inform
- A sales AI trained to exploit known emotional vulnerabilities (bereavement, financial stress) to push upsells → **PROHIBITED**
- An AI that mimics grief counseling language to make users more susceptible to offers → **PROHIBITED**

**What is NOT prohibited:** Persuasion through accurate, transparent information; recommendations based on stated preferences; A/B testing of messaging (without psychological exploitation).

---

## 2. Exploitation of Vulnerabilities
**Legal text (Art. 5(1)(b)):** AI that exploits vulnerabilities of specific groups — due to age, disability, or social/economic situation — in a way that distorts behavior, causing or likely to cause significant harm.

**What this means in practice:**
- A debt collection AI that targets consumers in financial distress with messaging designed to exploit anxiety and shame → **PROHIBITED**
- An AI in a children's game that uses addictive design patterns (variable rewards, social pressure) to drive in-app purchases → **PROHIBITED**
- A welfare services chatbot that presents options in a misleading way to discourage benefit claims by vulnerable users → **PROHIBITED**

**What is NOT prohibited:** Age-appropriate content filtering; accessibility features; targeted support for vulnerable groups that genuinely serves their interests.

---

## 3. Social Scoring
**Legal text (Art. 5(1)(c)):** AI systems that evaluate or classify individuals based on social behavior or personal characteristics, leading to detrimental or unfavorable treatment in unrelated contexts, or treatment that is disproportionate to its social significance.

**What this means in practice:**
- An employee "trustworthiness score" based on punctuality, email tone, and social media activity, used to determine who gets promoted or assigned to high-profile projects → **PROHIBITED**
- A vendor scoring system that rates suppliers based on political or social views of their leadership → **PROHIBITED**
- A customer loyalty AI that penalizes users for past complaints, public reviews, or social media criticism → **PROHIBITED** (if used to deny/restrict services)

**What is NOT prohibited:** Credit scoring using financial data for credit decisions; performance reviews based on documented work quality; customer satisfaction tracking that doesn't restrict access to services.

---

## 4. Real-Time Remote Biometric Identification in Public Spaces
**Legal text (Art. 5(1)(d)–(f)):** Real-time remote biometric identification of natural persons in publicly accessible spaces for law enforcement purposes — with very narrow exceptions (imminent terrorist threat, specific missing persons, specific serious crime suspects).

**What this means in practice:**
- Installing facial recognition cameras in a store to identify shoplifters in real time → **PROHIBITED** (unless law enforcement, with prior authorization)
- Using biometric analysis at a company event to identify attendees or monitor emotional reactions → **PROHIBITED**
- A building security system that continuously scans faces of everyone entering and matches against any database → **PROHIBITED**

**Note:** Post-hoc biometric identification (after the fact, not real-time) by law enforcement with judicial authorization is not covered by this prohibition but has its own requirements.

---

## 5. Emotion Recognition in Workplace and Educational Settings
**Legal text (Art. 5(1)(f)):** AI systems that infer emotions of natural persons in the workplace or educational institutions.

**What this means in practice:**
- An AI that analyzes call center recordings to infer whether agents are stressed, happy, bored, or disengaged, and feeds this into performance reviews → **PROHIBITED**
- A video interview AI that assesses candidates' emotional reactions during job interviews → **PROHIBITED**
- A student monitoring system that uses webcam analysis to detect engagement, stress, or emotional state during online exams → **PROHIBITED**
- An AI that analyzes employee chat messages for sentiment and reports this to managers as "mood scores" → **PROHIBITED**

**What is NOT prohibited:** Sentiment analysis of voluntary customer feedback; emotion detection for genuine medical/safety purposes (e.g., detecting driver drowsiness) with appropriate safeguards — but the workplace/education exception is strict.

**Key point for your company:** `EmotionScan` (agent-004 in the registry) almost certainly falls into this category. Immediate assessment required.

---

## 6. Biometric Categorization for Sensitive Attributes
**Legal text (Art. 5(1)(g)):** AI that uses biometric data to infer race, ethnicity, political opinion, trade union membership, religious or philosophical beliefs, sexual orientation, or health status.

**What this means in practice:**
- Facial analysis software that infers race or ethnicity from employee photos for any purpose → **PROHIBITED**
- An AI that analyzes voice patterns to infer political or religious affiliation → **PROHIBITED**
- A system that categorizes job applicants by inferred ethnicity derived from name, photo, or linguistic patterns → **PROHIBITED**

---

## 7. Predictive Policing Based on Profiling
**Legal text (Art. 5(1)(d)):** AI used by law enforcement to assess the likelihood that a natural person will commit a crime, based solely on profiling or assessed personality traits.

**What this means in practice:** This primarily targets law enforcement, but companies operating security systems should be careful:
- A security AI that flags employees as "theft risks" based on behavioral profiling alone → edge case, legal assessment needed
- An AI that recommends pre-emptive disciplinary action based on predicted future behavior rather than actual conduct → **likely PROHIBITED** under the spirit of this provision

---

## 8. Facial Recognition Databases Built from Scraping
**Legal text (Art. 5(1)(e)):** AI used to compile or expand facial recognition databases by untargeted scraping of facial images from the internet or from CCTV footage.

**What this means in practice:**
- Buying or using any database of facial images that was built by scraping social media or public internet → **PROHIBITED**
- Building an internal system that scrapes LinkedIn or employee directories to build a face recognition corpus → **PROHIBITED**

---

## Summary Table for Internal Review

| Prohibited Practice | Most Likely Internal Risk Vector |
|--------------------|----------------------------------|
| Subliminal manipulation | Customer-facing chatbots with conversion optimization |
| Vulnerability exploitation | Debt collection AI, customer retention AI |
| Social scoring | Employee "culture fit" scoring, customer trust scores |
| Real-time biometric identification | Building security, event monitoring |
| Emotion inference in workplace | Call monitoring, video interview tools, productivity monitoring |
| Biometric categorization (sensitive attributes) | Hiring AI using photos, voice analysis tools |
| Predictive policing/profiling | Security anomaly agents, behavioral risk systems |
| Facial recognition database scraping | Any system using third-party face recognition |

---

## What To Do If You Identify a Prohibited Practice

1. **Stop the system** — do not wait for a formal compliance process. Suspend the agent immediately.
2. **Document the discovery** — note who discovered it, when, and what the system was doing.
3. **Notify Legal** — the EU AI Act creates direct liability for the deployer. Early notification matters.
4. **Preserve evidence** — do not delete logs, outputs, or configuration before Legal has reviewed.
5. **Do not redeploy** — even with modifications, any system in a prohibited category must be assessed by Legal before any form of redeployment.

---

*Questions? Contact Legal Operations at [legal-ops@company.com]*
*Last updated: April 2026 | Owner: Legal / Compliance*
