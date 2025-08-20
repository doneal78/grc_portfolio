# AWS Account Governance & Security Foundations

**Objective**  
Demonstrate AWS account governance and baseline security setup for a small-to-medium enterprise environment, ensuring compliance alignment and audit readiness.

---

## Scope
- **Identity and Access Management**: Implement AWS IAM Identity Center (SSO) with enforced MFA and least-privilege role design.
- **Compliance Monitoring**: Configure AWS Config with baseline rules (unencrypted EBS volumes, public S3 buckets, security group hygiene).
- **Centralized Security Visibility**: Enable AWS Security Hub across regions for aggregated findings.
- **Audit Logging**: Configure AWS CloudTrail with centralized storage and log file validation.
- **Cost Controls**: Implement AWS Budgets with threshold-based alerts.

---

## Identity & Access Baseline (IAM Identity Center + Least-Privilege)

**What I implemented**
- Enabled **IAM Identity Center (SSO)** and created a named user (MFA required).
- Built three permission sets: **AdminAccess** (full admin), **SecurityAudit** (read-only), **Billing**.
- Assigned **user → account → roles** and enabled **IAM access to Billing** so roles can open the Billing console.
- Set Identity Center **MFA policy = Required** (authenticator app).

**Why it matters**
- Retires daily use of the **root** user; moves workforce identity to SSO.
- Enforces separation of duties: admin vs. audit vs. billing.
- Sets the stage for org-wide scaling (SCPs and additional accounts later).

**Artifacts**
- ![SSO Tiles](/assets/img/sso-portal-tiles.png)
- ![Assignments](/assets/img/identity-center-assignments.png)
- ![MFA Required](/assets/img/identity-center-mfa-required.png)
- ![Billing Access](/assets/img/billing-iam-access.png)

**Control Mapping**
- **NIST CSF:** PR.AC-1/4 (Access control), ID.AM-1 (Asset mgmt)
- **CIS v8:** 5 (Account Mgmt), 6 (Access Control)
- **ISO 27001:** A.5, A.8 (User access), A.12 (Ops security)

**Acceptance Criteria**
- Root user has **MFA** and is **not** used for daily work.
- Identity Center **MFA required** is ON.
- User can assume **AdminAccess**, **SecurityAudit**, **Billing** via the SSO portal.
- Billing console opens with the **Billing** role.

---

## Control Mapping (platform baseline)
- **NIST Cybersecurity Framework (CSF):** ID.AM, PR.AC, PR.DS, DE.CM, RS.MI  
- **CIS Controls v8:** 4 (Admin Privileges), 5 (Account Mgmt), 6 (Access Control Mgmt), 8 (Audit Log Mgmt), 15 (Service Provider Mgmt)  
- **ISO 27001 Annex A:** A.5 (Policies), A.8 (User access), A.12 (Ops security), A.18 (Compliance)

---

## Artifacts (platform baseline)
- [Architecture Diagram](../assets/img/aws-gov-architecture.png)  
- [Control-to-Service Matrix](../assets/control-matrix.csv)  
- [Security Hub Baseline Checklist](../assets/aws-securityhub-baseline.md)  
- ![SSO Tiles](/assets/img/sso-portal-tiles.png)  
- ![Assignments](/assets/img/identity-center-assignments.png)  
- ![MFA Required](/assets/img/identity-center-mfa-required.png)  
- ![Billing Access](/assets/img/billing-iam-access.png)

---

## Outcomes
- Centralized governance structure for the AWS account.
- Reduced detection time for misconfigurations from “manual review” to automated near-real time.
- Audit-ready evidence for IAM, configuration drift, and budget monitoring.

---

## Next Steps
- Implement **Service Control Policies (SCPs)** for organization-wide guardrails.
- Deploy **infrastructure-as-code** (Terraform/CloudFormation) for reproducibility.
- Add **auto-remediation** workflows (e.g., Lambda responding to public S3 buckets).
