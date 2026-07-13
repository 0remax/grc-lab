---
layout: default
title: Vendor Risk Assessment
nav_order: 7
---

# Third-Party Vendor Risk Assessment (TPRM)

Effective Third-Party Risk Management is critical to securing our supply chain and ensuring that our partners maintain a security posture consistent with our internal standards.

## 1. Vendor Security Questionnaire
To vet new partners, I utilize the following technical assessment criteria:

* **Identity Management:** Does the vendor enforce Multi-Factor Authentication (MFA) across all administrative domains?
* **Data Protection:** Is data encrypted at rest (AES-256) and in transit (TLS 1.2+)?
* **Vulnerability Management:** How frequently are penetration testing logs reviewed and remediated?
* **Access Control:** Does the vendor provide Least Privilege access to corporate resources?
* **Business Continuity:** Does the vendor have a tested Disaster Recovery plan with defined RTO/RPO targets?

## 2. Risk Scoring Matrix
I classify vendor risk based on their level of system integration and data access requirements.

| Risk Level | Access Tier | Mitigation Criteria |
| :--- | :--- | :--- |
| **High** | Critical / Full Access | Vendor has access to PII or core infrastructure. Mandatory annual security audit required. |
| **Medium** | Limited / Application | Vendor integrates with non-sensitive APIs. Bi-annual security review required. |
| **Low** | Public / None | Vendor has no access to corporate data. Periodic security check-in required. |
