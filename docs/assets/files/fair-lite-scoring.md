# FAIR‑lite Scoring Worksheet

> Purpose: quick, explainable scoring for quarterly risk reviews. Outcome = **Impact × Likelihood** and a treatment decision with rationale.

---

## 1) Context
- **Risk ID:** R-XX  
- **Title:**  
- **Owner:**  
- **Process / System:**  
- **Related Controls / Framework:** NIST CSF (ID.AM‑, PR.AC‑, DE.AE‑ …)

---

## 2) Impact Scale (choose one)
| Level | Description | Example consequences |
|------:|-------------|----------------------|
| High  | Regulatory fines, major outage, material revenue impact | PII breach, prolonged service downtime |
| Medium| Noticeable customer/ops impact, manageable cost | Service degradation, contained incident |
| Low   | Minor localized effect | Isolated team process issue |

**Selected Impact:** `High | Medium | Low`  
**Why:**  

---

## 3) Likelihood Scale (choose one)
Consider **threat frequency** + **control strength**.

| Level  | Description | Heuristics |
|-------:|-------------|------------|
| Likely | Expected this quarter | Seen attempts, weak controls |
| Possible | Could occur this year | Threat exists, controls mixed |
| Unlikely | Rare under current controls | Strong preventive/detective controls |

**Selected Likelihood:** `Likely | Possible | Unlikely`  
**Why:**  

---

## 4) Inherent vs Residual
- **Inherent Risk (Impact × Likelihood):** `High | Medium | Low`
- **Proposed Treatment:** `Mitigate | Accept | Transfer | Avoid`
- **Residual Risk (post‑control):** `High | Medium | Low`
- **Rationale for treatment:**  

---

## 5) Actions & Evidence
- **Action(s):**  
- **Owner(s):**  
- **Due Date:**  
- **Evidence to capture:** screenshots (controls), tickets/changes, metrics.

---

## 6) Review History
| Date | Reviewer | Notes / Decision |
|------|----------|------------------|
| YYYY‑MM‑DD | | |

---

## 7) Quick Heatmap (optional)
> Mark the selected cell.

|            | **Unlikely** | **Possible** | **Likely** |
|------------|--------------:|-------------:|-----------:|
| **High**   |      Medium   |     High     |    High    |
| **Medium** |       Low     |     Medium   |    High    |
| **Low**    |       Low     |      Low     |   Medium   |

---

**Template Version:** v1.0 (FAIR‑lite quick scoring)
