---
title: LOGGING & MONITORING POLICY
company: Blowbits Solutions LLP
classification: Internal
revision: "1.1"
last_update_date: 2026-02-10
---

# 1. Purpose

This policy establishes the logging and monitoring framework for the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective of this policy is to support operational visibility, security monitoring and accountability through the collection, protection and review of relevant system and operational events.

# 2. Scope

This policy applies to applications, infrastructure components, network devices, operating environments and operational activities associated with the Blowbits Solutions LLP GSP platform.

Logging and monitoring controls apply to relevant production and supporting systems, including:

- Application and API events.
- Authentication, access and privileged activity events.
- Infrastructure, operating environment and cloud service events.
- Database and data service events where applicable.
- Network, firewall, security group and connectivity events where available.
- Backup, replication and recovery events.
- Security alerts and monitoring tool events.

Supporting procedures, technical standards and implementation evidence are maintained separately.

# 3. Logging & Monitoring Framework

Logging and monitoring controls are implemented to support secure operation and effective management of the GSP platform.

The framework is established to:

- Record operational and security-related events.
- Support monitoring of platform availability and operational health.
- Assist in troubleshooting and incident investigation.
- Maintain accountability for administrative activities.
- Support audit and compliance requirements.

# 4. Logging & Monitoring Principles

The GSP platform operates according to the following principles:

- Operational events are recorded through appropriate logging mechanisms.
- Monitoring supports timely identification of operational and security-related events.
- Access to log information is restricted to authorised personnel.
- Log information is protected against unauthorised modification or deletion.
- Logging and monitoring records are protected from unauthorised access and are retained according to defined retention requirements.
- Logging configurations should avoid recording secrets, credentials, tokens or sensitive taxpayer information where practicable.
- Systems use cloud-provider managed time synchronisation, where available, to support reliable timestamps and event correlation.
- Monitoring information supports operational decision-making and incident response.
- Logging and monitoring controls are reviewed at least annually or when significant platform changes occur.

# 5. Retention Requirements

Logging and monitoring records shall be retained based on their purpose and audit relevance.

The minimum retention requirements are:

- Security, access and audit logs: 7 years.
- Operational troubleshooting logs: 90 days.
- Incident-related logs and extracts: retained with the applicable incident records.

# 6. Operational Monitoring

Logging and monitoring activities are performed through structured operational processes.

The operational framework includes:

- Collection of operational events.
- Monitoring of platform health and availability.
- Review of security-related events.
- Protection of operational log information.
- Investigation of significant operational events.

# 7. Compliance

Compliance with this policy is supported through documented procedures, operational practices, monitoring activities and implementation evidence.

Detailed operational processes and technical controls are maintained separately to support the effective implementation of this policy.

# Revision History

| Date | Revision | Change Summary |
| ---- | -------- | -------------- |
| 2025-11-13 | 1.0 | Initial release of the logging and monitoring policy. |
| 2026-02-10 | 1.1 | Added log source coverage, retention requirements, time synchronisation and sensitive data guidance. |
