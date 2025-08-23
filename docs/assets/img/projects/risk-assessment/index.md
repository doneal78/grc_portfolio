---
layout: default
title: Risk Assessment (Simulated)
permalink: /projects/risk-assessment/
---

# Risk Assessment (Simulated)

**Objective**  
Demonstrate a repeatable risk analysis workflow using a FAIR‑lite approach that produces audit‑ready artifacts and business‑aligned decisions.

## Scope & Assumptions
- Pilot scope: one business unit, 10 simulated risks.
- Control catalog referenced: NIST CSF (selected subcategories).
- Scoring model: **FAIR‑lite** (qualitative impact × likelihood) with an explicit treatment decision for each risk.

## Method at a Glance
1. **Inventory** — gather risks with owners, controls, and ties to business processes.  
2. **Score** — apply FAIR‑lite: Impact (Low/Med/High) × Likelihood (Rare/Unlikely/Possible/Likely).  
3. **Prioritize** — heatmap and top‑N list.  
4. **Treat** — mitigate, accept, or transfer; log the why and the by‑when.  
5. **Evidence** — keep artifacts (register, scoring notes, tickets) in source control.

---

## Risk Register (Excerpt)
| ID | Title | Owner | Key Control(s) | Impact | Likelihood | Current Treatment |
|---:|---|---|---|---|---|---|
| R‑01 | Privilege escalation via stale admin role | Platform Eng | IAM review SOP, Just‑In‑Time access | High | Possible | Mitigate (JIT & review) |
| R‑02 | Public S3 bucket exposure | Cloud Eng | S3 Block Public Access, Config rules | High | Unlikely | Mitigate (SCP + rule) |
| R‑03 | Vendor breach of PII | GRC | DPA, SOC 2 review, key mgmt | High | Possible | Transfer (contract) |
| R‑04 | Phishing leads to Okta session hijack | IT Sec | FIDO2, Conditional Access | Medium | Likely | Mitigate (MFA hardening) |

> Full register lives in repo for audit traceability (CSV/MD). Tie each risk to a control, owner, status, and a dated decision.

---

## FAIR‑Lite Scoring Notes
- **Impact** bins reflect business objectives (e.g., regulatory fines, revenue loss, downtime).  
- **Likelihood** bins reflect threat frequency + control strength.  
- **Why this works:** keeps decisions consistent, explainable, and fast enough for quarterly cycles.

<!--
## Visual Evidence — add when ready

Uncomment any block below after you upload screenshots to:
docs/assets/img/projects/risk-assessment/

<div class="figure">
  <img src="/grc_portfolio/assets/img/projects/risk-assessment/risk-register.jpg"
       alt="Risk register view with owners, controls, impact, likelihood and treatment fields">
  <div class="figcaption">Risk register snapshot — owners, controls, and status for audit clarity.</div>
</div>

<div class="figure">
  <img src="/grc_portfolio/assets/img/projects/risk-assessment/fair-heatmap.jpg"
       alt="FAIR-lite heatmap matrix of impact versus likelihood highlighting high-priority risks">
  <div class="figcaption">FAIR‑lite heatmap used to prioritize the top risks for the quarter.</div>
</div>

<div class="figure">
  <img src="/grc_portfolio/assets/img/projects/risk-assessment/treatment-plan.jpg"
       alt="Treatment plan table showing mitigate, accept, transfer decisions with due dates and owners">
  <div class="figcaption">Treatment plan — decision, rationale, owner, and due date for each top risk.</div>
</div>
-->

---

## Treatment Decisions (Top 3)
- **R‑01 Privilege escalation** — *Mitigate*: enforce JIT elevation; 90‑day admin review; alert on unused roles.  
- **R‑02 Public S3 exposure** — *Mitigate*: org‑level **Block Public Access**, SCPs, Config rule remediation.  
- **R‑03 Vendor breach of PII** — *Transfer*: tighten DPA language; escrow keys; quarterly assurance reviews.

---

## Outcomes
- Top risks aligned to business impact with clear owners and dates.  
- Documented, repeatable scoring workflow; decisions are explainable in audits.  
- Evidence artifacts (register, scoring notes, tickets) are version‑controlled and re‑usable.

---

## What’s Next
- Add quarterly diffs showing risk movement.  
- Include screenshots of the heatmap and treatment tracker (see **Visual Evidence** section when ready).
