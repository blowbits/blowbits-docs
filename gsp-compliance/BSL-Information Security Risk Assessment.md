---
title: INFORMATION SECURITY RISK ASSESSMENT
company: Blowbits Solutions LLP
classification: Internal
revision: "1.1"
last_update_date: 2026-02-23
assessment_date: 2026-02-23
reviewed_by: Information Security Lead
approved_by: GSP Governance Lead
next_review_due: 2027-02-22
logo: ../assets/octa-gst-logo.png
---

# 1. Purpose

This document records the current information security risk assessment for the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The assessment identifies key information security risks, existing controls, residual risk levels and treatment status to support effective risk management and protect the confidentiality, integrity and availability of the GSP platform, taxpayer information and supporting infrastructure.

# 2. Scope

This assessment applies to the production GSP platform, cloud infrastructure, applications, databases, network components, supporting services and operational processes.

# 3. Assessment Details

| Field           | Value                     |
| --------------- | ------------------------- |
| Assessment Date | 2026-02-23                |
| Reviewed By     | Information Security Lead |
| Approved By     | GSP Governance Lead       |
| Next Review Due | 2027-02-22                |

# 4. Risk Assessment Methodology

Information security risks are identified, assessed and managed through:

- Periodic information security reviews.
- Vulnerability Assessment and Penetration Testing (VAPT).
- Continuous operational monitoring and security event analysis.
- Review of security advisories and threat intelligence from trusted sources, including GSTN communications, CERT-In advisories, cloud service providers, software vendors and other recognised security advisories.
- Infrastructure, application and configuration changes.
- Security incidents and root cause analysis.
- Periodic governance reviews.

Risks are evaluated based on likelihood and impact before and after controls are applied.

Inherent risk represents the level of risk before considering implemented controls. Residual risk represents the remaining risk after preventive, detective and corrective controls are applied.

Residual risk may remain because no control eliminates risk completely, external dependencies cannot be fully controlled, and operational or security controls may fail or require improvement over time.

# 5. Information Security Risk Assessment

## 5.1 Unauthorised Access to Production Systems

| Field | Details |
| ----- | ------- |
| Potential Impact | Compromise of taxpayer information or critical services |
| Existing Controls | Role-based access control, least privilege, MFA, restricted privileged access, periodic access review and activity logging where supported |
| Inherent Risk | High |
| Residual Risk | Medium |
| Risk Owner | Information Security Lead |
| Treatment Status | Managed through access control, monitoring and periodic review |

## 5.2 Application Vulnerabilities

| Field | Details |
| ----- | ------- |
| Potential Impact | Data compromise, service interruption or unauthorised transaction processing |
| Existing Controls | Latest supported .NET framework, secure development practices, regular VAPT, patch management, security reviews, change control and remediation tracking |
| Inherent Risk | High |
| Residual Risk | Low |
| Risk Owner | Information Security Lead |
| Treatment Status | Managed through supported framework usage, regular VAPT, remediation tracking and validation |

## 5.3 Cloud Infrastructure Failure

| Field | Details |
| ----- | ------- |
| Potential Impact | Service disruption or reduced availability of GSP services |
| Existing Controls | AWS high availability design, second availability zone, monitoring, backup, recovery procedures and recovery testing |
| Inherent Risk | High |
| Residual Risk | Low |
| Risk Owner | Platform Operations Lead |
| Treatment Status | Managed through second availability zone design, recovery planning and periodic recovery testing |

## 5.4 Malware or Ransomware

| Field | Details |
| ----- | ------- |
| Potential Impact | Data loss, data corruption or operational disruption |
| Existing Controls | Endpoint protection, restricted administrative access, backup strategy, monitoring and incident response procedures |
| Inherent Risk | High |
| Residual Risk | Medium |
| Risk Owner | Information Security Lead |
| Treatment Status | Managed through preventive controls, monitoring, backup and incident response readiness |

## 5.5 Insider Misuse

| Field | Details |
| ----- | ------- |
| Potential Impact | Unauthorised system changes, data access or misuse of privileged access |
| Existing Controls | Role-based access, least privilege, audit logging where supported, management oversight, small-team compensating controls and periodic access review |
| Inherent Risk | High |
| Residual Risk | Medium |
| Risk Owner | GSP Governance Lead |
| Treatment Status | Managed through access review, approval controls, logging and governance oversight |

## 5.6 Network Attacks

| Field | Details |
| ----- | ------- |
| Potential Impact | Service disruption, unauthorised access or exposure of internal services |
| Existing Controls | Firewall controls, reverse proxy, TLS encryption, restricted network pathways, intrusion prevention and continuous monitoring |
| Inherent Risk | High |
| Residual Risk | Medium |
| Risk Owner | Platform Operations Lead |
| Treatment Status | Managed through network controls, monitoring and periodic review |

## 5.7 Data Loss or Corruption

| Field | Details |
| ----- | ------- |
| Potential Impact | Loss or corruption of taxpayer information or operational data |
| Existing Controls | Continuous PostgreSQL streaming replication, weekly full backup, archive log backup every 5 minutes, 30-day retention, encrypted S3 backup storage and recovery testing |
| Inherent Risk | High |
| Residual Risk | Low |
| Risk Owner | Platform Operations Lead |
| Treatment Status | Managed through replication, backup, recovery testing and access restriction |

## 5.8 Third-Party Service Disruption

| Field | Details |
| ----- | ------- |
| Potential Impact | Temporary interruption of external integrations or support services |
| Existing Controls | Monitoring, escalation through authorised contact channels, failover procedures where applicable and incident management process |
| Inherent Risk | Medium |
| Residual Risk | Medium |
| Risk Owner | GSP Coordination Lead |
| Treatment Status | Accepted with monitoring because external service availability is not fully controlled by Blowbits |

# 6. Risk Treatment

Identified risks are managed through preventive, detective and corrective controls, including:

- Secure system configuration and hardening.
- Periodic Vulnerability Assessment and Penetration Testing (VAPT).
- Patch and vulnerability management.
- Security monitoring and log review.
- Backup and disaster recovery procedures.
- Access control and periodic access reviews.
- Governance approval and compensating controls where segregation of duties is limited by team size.
- Incident response and corrective action management.

Medium residual risks are accepted for continued operation subject to ongoing monitoring, periodic review and corrective action where control weaknesses or significant changes are identified.

# 7. Risk Review

Information security risks shall be reviewed:

- At least annually.
- Following major infrastructure or application changes.
- Following significant security incidents.
- Following Vulnerability Assessment and Penetration Testing (VAPT).
- Whenever new threats or significant vulnerabilities are identified.
- Whenever material changes occur to GSTN integration, cloud architecture or external service dependencies.

# 8. Review

This document shall be reviewed annually or whenever significant operational, organisational, technical or regulatory changes occur.

# Revision History

| Date | Revision | Change Summary |
| ---- | -------- | -------------- |
| 2025-11-25 | 1.0 | Initial release of the information security risk assessment. |
| 2026-02-23 | 1.1 | Updated risk ratings, residual risk rationale, assessment details and risk presentation format. |
