# Risk Appetite Profiles

TechForward's leadership operates under different risk appetite levels depending on the business context. Use these profiles to adjust the Regulatory Horizon Map assessment — the same regulatory gap may be a "Deal Breaker" under a conservative profile but a "Managed Risk" under an aggressive one.

---

## Profile 1: Conservative

**When this applies:** Regulated industry clients (banks, healthcare), public sector deals, situations where regulatory scrutiny is likely, or first entry into a new market.

### Decision Thresholds

| Risk Level | Threshold | Action |
|------------|-----------|--------|
| **Deal Breaker** | Any requirement where non-compliance could result in fines, enforcement action, or client liability | **Cannot launch** until fully resolved |
| **Managed Risk** | Any requirement where compliance is partially in place but gaps exist | **Cannot launch** until a documented remediation plan is approved by legal |
| **Clear** | Requirement is fully met or does not apply | **Proceed** |

### Principles

- All regulatory requirements must be met **before** launch, not after
- DPIAs, TIAs, and conformity assessments must be completed and signed off
- External legal review required for any novel regulatory question
- Works council agreements must be in place before deploying employee-affecting tools
- Zero tolerance for "launch and fix later" approach
- Board-level sign-off required for any residual risk acceptance

### Escalation

- Any "Managed Risk" item must be escalated to General Counsel
- Any "Deal Breaker" item must be escalated to the Board

---

## Profile 2: Moderate

**When this applies:** Standard B2B product launches, existing markets, established client relationships, or situations where TechForward has prior regulatory experience.

### Decision Thresholds

| Risk Level | Threshold | Action |
|------------|-----------|--------|
| **Deal Breaker** | Requirements where non-compliance creates direct legal liability or enforcement risk | **Cannot launch** until resolved |
| **Managed Risk** | Requirements where partial compliance is in place and a clear remediation plan exists with a deadline within 90 days of launch | **Can launch** with documented risk acceptance and remediation timeline |
| **Clear** | Requirement is fully met or does not apply | **Proceed** |

### Principles

- Critical legal requirements (lawful basis, core GDPR, high-risk AI classification) must be met before launch
- Secondary requirements (full documentation, optimization of consent flows, complete RoPA update) can be completed within 90 days post-launch if interim measures are in place
- Internal legal review is sufficient for known regulatory areas
- Risk acceptance decisions can be made by General Counsel without Board involvement
- "Launch with safeguards" approach is acceptable where interim measures reduce risk to an acceptable level

### Escalation

- "Deal Breaker" items escalated to General Counsel
- Residual risks above EUR 500K potential exposure escalated to CFO

---

## Profile 3: Aggressive

**When this applies:** Competitive time pressure, significant revenue opportunity at risk, fast-follower market dynamics, or situations where delay has a higher cost than regulatory risk.

### Decision Thresholds

| Risk Level | Threshold | Action |
|------------|-----------|--------|
| **Deal Breaker** | Only requirements where non-compliance would result in immediate enforcement action, criminal liability, or existential business risk | **Cannot launch** until resolved |
| **Managed Risk** | Requirements where non-compliance creates regulatory risk but enforcement is unlikely in the short term, or where a good-faith compliance effort is documented | **Can launch** with risk accepted by executive sponsor and remediation plan within 180 days |
| **Clear** | Requirement is fully met, does not apply, or risk is de minimis | **Proceed** |

### Principles

- Only true legal prohibitions are Deal Breakers (e.g., cannot process data without any lawful basis; cannot deploy prohibited AI practices)
- Documentation and process requirements can be completed post-launch if a credible plan exists
- "Good faith effort" approach: demonstrating active work toward compliance is a valid interim position
- Speed-to-market value is explicitly weighed against regulatory risk
- Executive sponsor personally accepts residual risk
- Legal provides risk assessment but does not have veto power — business makes the call

### Escalation

- "Deal Breaker" items escalated to CEO
- Risk acceptance requires written sign-off from executive sponsor with acknowledgment of potential consequences

### Guardrails (Even Under Aggressive Profile)

Even under the most aggressive risk appetite, the following are **always Deal Breakers** regardless of business pressure:

1. Processing personal data without **any** lawful basis
2. Deploying AI systems classified as **prohibited** under the EU AI Act (Art. 5)
3. Operating without **any** data processing agreement where legally required
4. Ignoring a known data breach notification obligation
5. Launching in a jurisdiction where the product is **explicitly illegal**
6. Making representations to regulators or clients that are **knowingly false**
