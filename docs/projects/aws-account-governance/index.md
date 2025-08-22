---
layout: default
title: AWS Account Governance Case Study
---

# AWS Account Governance Case Study

**Objective**: Design an AWS account structure aligned to NIST CSF, with least privilege and continuous monitoring.

---

### Problem
Organizations adopting AWS often face:
- Siloed accounts without consistent guardrails  
- Over-privileged identities  
- Manual compliance checks that don’t scale  

---

### Approach
1. **Baseline Controls**: Mapped NIST CSF categories to AWS native services.  
   - Identity & Access → AWS IAM Identity Center  
   - Configuration Management → AWS Config rules  
   - Continuous Monitoring → Security Hub  
2. **Least Privilege**: Designed role-based access with scoped permissions.  
3. **Guardrails**: Service Control Policies enforced region use, MFA, budget limits.  
4. **Evidence**: Screenshots of configs, CLI outputs, and CloudTrail logs collected for audit packages.  

---

### Outcome
- Reduced risk of unauthorized changes by implementing SCPs across **100% of accounts**.  
- Aligned AWS guardrails to **50+ NIST CSF subcategories**.  
- Created a repeatable pattern to onboard new accounts with governance pre-baked.  

---

### Evidence Artifacts
- 📄 Config rule compliance snapshots  
- 📸 IAM role/permission screenshots  
- 📝 Mapping matrix: NIST CSF ↔ AWS service  
