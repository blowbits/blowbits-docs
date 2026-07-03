---
title: INFORMATION SECURITY RISK ASSESSMENT
company: Blowbits Solutions LLP
classification: Internal
---

# 1. Purpose

This document identifies the key information security risks associated with the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform and the controls implemented to manage those risks.

The objective is to support effective risk management and ensure the confidentiality, integrity and availability of the GSP platform, taxpayer information and supporting infrastructure.

# 2. Scope

This assessment applies to the production GSP platform, cloud infrastructure, applications, databases, network components, supporting services and operational processes.

# 3. Risk Assessment Methodology

Information security risks are identified, assessed and managed through:

- Periodic information security reviews.
- Vulnerability Assessment and Penetration Testing (VAPT).
- Continuous operational monitoring and security event analysis.
- Review of security advisories and threat intelligence from trusted sources, including GSTN communications, CERT-In advisories, cloud service providers, software vendors and other recognised security advisories.
- Infrastructure, application and configuration changes.
- Security incidents and root cause analysis.
- Periodic management reviews.

Identified risks are evaluated based on their potential business impact and likelihood of occurrence. Appropriate preventive, detective and corrective controls are implemented to reduce identified risks to an acceptable level.

# 4. Information Security Risk Assessment

| Risk                                      | Potential Impact                                        | Existing Controls                                                                       | Residual Risk |
| ----------------------------------------- | ------------------------------------------------------- | --------------------------------------------------------------------------------------- | ------------- |
| Unauthorised access to production systems | Compromise of taxpayer information or critical services | Role-based access control, least privilege, MFA, periodic access review                 | Low           |
| Application vulnerabilities               | Data compromise or service interruption                 | Secure development practices, VAPT, patch management and security reviews               | Low           |
| Cloud infrastructure failure              | Service disruption                                      | AWS high availability, monitoring, backup and disaster recovery procedures              | Low           |
| Malware or ransomware                     | Data loss or operational disruption                     | Endpoint protection, backup strategy, monitoring and restricted administrative access   | Low           |
| Insider misuse                            | Unauthorised system changes or data access              | Role-based access, audit logging, management oversight and periodic access review       | Low           |
| Network attacks                           | Service disruption or unauthorised access               | Firewall, reverse proxy, TLS encryption, intrusion prevention and continuous monitoring | Low           |
| Data loss                                 | Loss or corruption of taxpayer information              | Automated backups, recovery testing, access controls and monitoring                     | Low           |
| Third-party service disruption            | Temporary interruption of external integrations         | Monitoring, failover procedures and incident management process                         | Low           |

# 5. Risk Treatment

Identified risks are managed through preventive, detective and corrective controls, including:

- Secure system configuration and hardening.
- Periodic Vulnerability Assessment and Penetration Testing (VAPT).
- Patch and vulnerability management.
- Security monitoring and log review.
- Backup and disaster recovery procedures.
- Access control and periodic access reviews.
- Security awareness and operational procedures.
- Incident response and corrective action management.

# 6. Risk Review

Information security risks shall be reviewed:

- At least annually.
- Following major infrastructure or application changes.
- Following significant security incidents.
- Following Vulnerability Assessment and Penetration Testing (VAPT).
- Whenever new threats or significant vulnerabilities are identified.

# 7. Review

This document shall be reviewed annually or whenever significant operational, organisational or regulatory changes occur.
