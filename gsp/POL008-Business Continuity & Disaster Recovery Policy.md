---
title: BUSINESS CONTINUITY & DISASTER RECOVERY POLICY
company: Blowbits Solutions LLP
classification: Internal
---

# 1. Purpose

This policy establishes the business continuity and disaster recovery framework for the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective of this policy is to support the continued availability of GSP services by establishing structured processes for responding to operational disruptions and restoring critical services within acceptable operational timeframes.

# 2. Scope

This policy applies to applications, infrastructure, operational processes, personnel and supporting resources associated with the operation of the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

Business continuity and disaster recovery coverage includes:

- GSP application and API services.
- PostgreSQL database services and supporting data services.
- Application, infrastructure and deployment configurations required for recovery.
- Cloud infrastructure and availability zone resilience.
- Network connectivity and supporting operational services.
- GSTN coordination and authorised external communication where applicable.
- Internal roles required for incident response, recovery and governance oversight.

Supporting procedures, technical standards and implementation evidence are maintained separately.

# 3. Business Continuity Framework

Business continuity and disaster recovery controls are implemented to support the resilience of GSP services.

The framework is established to:

- Minimise the impact of operational disruptions.
- Support restoration of critical platform services.
- Maintain continuity of essential business operations.
- Protect critical operational information during recovery activities.
- Support periodic evaluation of recovery readiness.

# 4. Roles and Responsibilities

Business continuity and disaster recovery responsibilities shall be assigned to authorised internal roles defined in the Roles, Responsibilities & Access Matrix.

| Role                          | BCDR Responsibility                                                                                                                                              |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Platform Operations Lead**  | Coordinate technical recovery, service restoration, infrastructure validation and recovery verification activities.                                              |
| **Information Security Lead** | Support recovery activities where security incidents, data exposure, credential compromise or security control impacts are involved.                             |
| **GSP Coordination Lead**     | Coordinate GSTN communication and other authorised external communication relating to GSP operations where applicable.                                           |
| **GSP Governance Lead**       | Provide oversight for significant continuity events, approve major recovery decisions, review exceptions and support closure of significant recovery activities. |

# 5. Business Continuity Principles

The GSP platform operates according to the following principles:

- Critical services are supported through established continuity arrangements.
- Recovery activities are performed through controlled operational procedures.
- Operational responsibilities during recovery are clearly defined.
- Recovery resources are maintained to support restoration activities.
- Backup, replication and recovery controls are maintained to support defined recovery objectives.
- Communication during significant continuity events is performed through authorised internal roles and approved contact channels.
- Recovery readiness is periodically reviewed.
- Business continuity controls are periodically evaluated for continued effectiveness.

# 6. Continuity Scenarios

The business continuity and disaster recovery framework considers disruptions that may affect the availability, integrity or recoverability of GSP services.

Continuity scenarios may include:

- Application or API outage.
- PostgreSQL database failure.
- Cloud availability zone disruption.
- Infrastructure, network or connectivity issue.
- Security incident affecting service availability.
- Loss or corruption of configuration or data.
- Key personnel unavailability.

Recovery actions for these scenarios shall be performed through approved operational, backup and recovery, incident response, communication and governance procedures, as applicable.

# 7. Recovery Objectives

Recovery objectives shall be defined based on platform criticality, available technical controls and operational requirements.

For critical PostgreSQL database services, the target Recovery Point Objective (RPO) is 1 minute and the target Recovery Time Objective (RTO) is 30 minutes, subject to the nature of the disruption, infrastructure availability and operational conditions at the time of recovery.

Recovery objectives for other platform components shall be defined and reviewed based on operational criticality and restoration requirements.

# 8. Continuity Operations

Business continuity activities are managed through structured operational processes.

The operational framework includes:

- Business continuity planning.
- Disaster recovery planning.
- Recovery coordination.
- Service restoration.
- Recovery verification.
- Authorised communication and escalation where required.
- Documentation of recovery actions and outcomes.
- Periodic review of continuity arrangements.

# 9. Testing and Review

Business continuity and disaster recovery readiness shall be reviewed periodically and whenever significant operational, organisational, regulatory or technical changes occur.

Readiness may be validated through recovery testing, incident simulations, tabletop review, post-incident review or management review of continuity and recovery records.

Issues identified during continuity review or recovery testing shall be documented and tracked where required.

# 10. Records and Evidence

The following records may be maintained, where applicable:

- Recovery test records.
- Recovery execution and verification records.
- Incident or continuity event records.
- Backup and recovery evidence.
- Communication records for significant continuity events.
- Management review, approval or exception records.

# 11. Compliance

Compliance with this policy is supported through documented procedures, operational practices, recovery exercises and implementation evidence.

Detailed operational processes and technical controls are maintained separately to support the effective implementation of this policy.
