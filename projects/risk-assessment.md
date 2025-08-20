# Enterprise Risk Assessment (Simulated)

**Objective**  
Demonstrate a full risk management cycle for a fictional organization, going beyond a static risk register to show process maturity.

---

## Process

1. **Risk Appetite Definition**  
   - Conducted simulated executive interviews to define tolerance thresholds for operational, regulatory, and reputational risks.  

2. **Risk Identification**  
   - Assessed risks across Identity, Patch/Vulnerability, Data, Cloud, and Third-Party domains.  

3. **Scoring Methodology**  
   - Applied Likelihood × Impact scoring, supported by FAIR-lite (Factor Analysis of Information Risk) estimates for impact modeling.  

4. **Prioritization**  
   - Identified “Top 10” risks for board-level reporting, focusing on high likelihood/high impact categories.  

5. **Treatment Planning**  
   - Applied avoid/transfer/mitigate/accept decisions with defined owners, budgets, and timelines.  

6. **Tracking & Monitoring**  
   - Created a living risk register with monthly re-assessments and metrics tracking.  

---

## Example Risk Entry

- **Risk:** Unauthorized privilege escalation in AWS  
- **Drivers:** Overly broad IAM roles, inconsistent MFA adoption, limited CIEM (Cloud Infrastructure Entitlement Management) visibility.  
- **Likelihood:** Medium  
- **Impact:** High (regulatory + operational disruption)  
- **Treatment:**  
  - Enforce SSO with MFA  
  - Apply permission boundaries and SCPs  
  - Monthly CIEM review  
- **Metrics:** # of admin roles, % of accounts with enforced MFA, reduction in unused IAM policies.  

---

## Artifacts
- [Risk Register (CSV)](../assets/risk-register.csv)  
- [Heat Map Visualization](../assets/img/risk-heatmap.png)  
- [Board-Level Risk Briefs](../assets/board-risk-briefs.pdf)  

---

## Outcomes
- Delivered actionable insights with measurable KPIs.  
- Translated technical risks into business impacts for leadership.  
- Provided a repeatable framework for ongoing risk cycles.  

---

## Next Steps
- Expand to include **Third-Party Vendor Risk** scenarios.  
- Introduce **Key Risk Indicators (KRIs)** tied to monitoring dashboards.  
- Simulate a **6-month reassessment cycle** to show trend data.  
