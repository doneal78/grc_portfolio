---
layout: default
title: AWS Account Governance Case Study
permalink: /projects/aws-account-governance/
---

# AWS Account Governance Case Study

**Objective**: Design an AWS account structure aligned to NIST CSF, with least privilege and continuous monitoring.

## Problem
Teams adopting AWS often face:
- Siloed accounts without consistent guardrails  
- Over‑privileged identities  
- Manual compliance checks that don’t scale  

## Approach
1. **Baseline Controls** — mapped NIST CSF categories to AWS native services.  
   - Identity & Access → AWS IAM Identity Center  
   - Configuration Management → AWS Config rules  
   - Continuous Monitoring → Security Hub  
2. **Least Privilege** — role‑based access with scoped permissions.  
3. **Guardrails** — Service Control Policies (SCPs) for region use, MFA, budgets.  
4. **Evidence** — screenshots of configs, CLI output, CloudTrail logs for audit packages.

## Outcome
- Reduced risk of unauthorized changes via SCPs across **100% of accounts**  
- Aligned AWS guardrails to **50+ NIST CSF subcategories**  
- Repeatable onboarding pattern with governance pre‑baked

## Evidence Packages

<div class="btn-row">
  <a class="btn-download"
     href="/grc_portfolio/assets/files/aws-config-controls.csv"
     download
     aria-label="Download AWS Config controls mapping CSV">
    <svg viewBox="0 0 24 24" aria-hidden="true"><path fill="currentColor" d="M12 3a1 1 0 0 1 1 1v9.586l2.293-2.293a1 1 0 1 1 1.414 1.414l-4.007 4.007a1.25 1.25 0 0 1-1.768 0l-4.007-4.007a1 1 0 1 1 1.414-1.414L11 13.586V4a1 1 0 0 1 1-1zM5 20a1 1 0 0 1 0-2h14a1 1 0 1 1 0 2H5z"/></svg>
    Download Config Control Map (CSV)
  </a>

  <a class="btn-view"
     href="/grc_portfolio/assets/files/aws-config-controls.csv"
     aria-label="View AWS Config controls mapping CSV in browser">
    <svg viewBox="0 0 24 24" aria-hidden="true"><path fill="currentColor" d="M14 3h7v7h-2V6.414l-7.293 7.293-1.414-1.414L17.586 5H14V3zM5 5h6v2H7v10h10v-4h2v6a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2V7a2 2 0 0 1 2-2z"/></svg>
    View Online
  </a>
</div>

