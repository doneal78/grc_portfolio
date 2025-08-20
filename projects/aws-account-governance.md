# AWS Account Governance & Security Foundations

**Objective**  
Demonstrate AWS account governance and baseline security setup for a small-to-medium enterprise environment, ensuring compliance alignment and audit readiness.

---

## Scope
- **Identity and Access Management**: Implement AWS IAM Identity Center (SSO) with enforced MFA and least-privilege role design.  
- **Compliance Monitoring**: Configure AWS Config with baseline rules (unencrypted EBS volumes, public S3 buckets, security group hygiene).  
- **Centralized Security Visibility**: Enable AWS Security Hub across multiple regions for aggregated findings.  
- **Audit Logging**: Configure AWS CloudTrail with centralized storage and log file validation.  
- **Cost Controls**: Implement AWS Budgets with threshold-based alerts.

---

## Control Mapping
- **NIST Cybersecurity Framework (CSF)**: ID.AM, PR.AC, PR.DS, DE.CM, RS.MI  
- **CIS Controls v8**: 4 (Controlled Use of Admin Privileges), 5 (Account Management), 6 (Access Control Management), 8 (Audit Log Management), 15 (Service Provider Management), 16 (Application Software Security)  
- **ISO 27001 Annex A**: A.5 (Information security policies), A.8 (User access management), A.12 (Operations security), A.18 (Compliance)

---

## Artifacts
- [Architecture Diagram](../assets/img/aws-gov-architecture.png)  
- [Control-to-Service Matrix](../assets/control-matrix.csv)  
- [Security Hub Baseline Checklist](../assets/aws-securityhub-baseline.md)

---

## Outcomes
- Centralized governance structure for AWS account.  
- Reduced detection time for misconfigurations from “manual review” to automated near-real time.  
- Provided audit-ready evidence for IAM, configuration drift, and budget monitoring.  

---

## Next Steps
- Implement **Service Control Policies (SCPs)** for organization-wide guardrails.  
- Deploy **infrastructure-as-code (Terraform/CloudFormation)** for reproducibility.  
- Add **auto-remediation workflows** (e.g., Lambda responding to public S3 buckets).  
