# Corporate Risk Register & Framework Alignment Project

## Project Overview
This project demonstrates a foundational approach to Governance, Risk, and Compliance (GRC) by identifying organizational risks, mapping them to standard regulatory frameworks (NIST CSF, PCI-DSS, HIPAA), and establishing strategic risk treatment plans with compensating controls.

## 📊 Corporate Risk Register

| Risk ID | Risk Description | Framework/Law | Risk Rating | Treatment Strategy | Chosen Controls / Mitigation |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **RSK-001** | Remote workers accessing production databases via unencrypted personal devices. | NIST CSF (Protect) | **High** | Mitigate | Drafted formal Remote Work/BYOD Policy; mandated multi-factor authentication (MFA). |
| **RSK-002** | Cardholder data (PAN) stored in plain-text Excel spreadsheets on shared network drives. | PCI-DSS (Req 3) | **Critical** | Mitigate | Migrated cardholder data to a secure, encrypted payment gateway vault. |
| **RSK-003** | Third-party live-chat vendor lacks MFA on core internal source code repositories. | Supply Chain Risk | **High** | Modify / Halt | Conditioned vendor onboarding; halted procurement until vendor enforces MFA or provides attestation. |
| **RSK-004** | Legacy Machine Learning server cannot support corporate 16-character password policy. | Internal Access Control | **Medium** | Accept (Temp) | Granted 30-day policy exception; implemented network isolation via secure VPN and mandated daily SOC log reviews. |

## 🔑 Key GRC Methodologies Applied
1. **Risk Calculation**: Evaluated qualitative risk levels using the standard formula:  
   Risk = Likelihood x Impact
2. **Third-Party Risk Management (TPRM)**: Analyzed a vendor SOC 2 Type II report, identifying a critical authentication deficiency in their access control structure.
3. **Compensating Controls**: Designed defensive network perimeters to safely authorize a temporary policy exception for legacy business systems without compromising the core infrastructure.
4. **Audit Practices**: Enforced "Trust, but Verify" principles by requiring technical configuration artifacts rather than relying on verbal assertions during compliance assessments.
