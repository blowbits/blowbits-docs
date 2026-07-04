---
title: BACKUP & RECOVERY POLICY
company: Blowbits Solutions LLP
classification: Internal
revision: "1.1"
last_update_date: 2026-02-05
---

# 1. Purpose

This policy establishes the backup and recovery framework for the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective of this policy is to ensure that critical platform components, PostgreSQL database information, application configurations and operational information can be restored following operational disruptions, supporting the continuity and reliability of GSP services.

# 2. Scope

This policy applies to production systems, PostgreSQL databases, application configurations, infrastructure components, operational information and supporting resources associated with the Blowbits Solutions LLP GSP platform.

Supporting procedures, technical standards, backup records, recovery test records and implementation evidence are maintained separately.

# 3. Backup & Recovery Framework

Backup and recovery controls are implemented to support restoration of platform services following operational events.

The framework is established to:

- Protect critical platform information through scheduled backup and replication processes.
- Maintain continuous PostgreSQL streaming replication to a second availability zone.
- Maintain weekly full PostgreSQL backups.
- Maintain PostgreSQL archive log backups every 5 minutes to support point-in-time recovery.
- Protect application configurations required for restoration of GSP services.
- Retain backup information for 30 days.
- Support restoration of services following operational disruptions.
- Maintain the integrity and availability of backup information.
- Protect backup information from unauthorized access, modification or deletion.
- Support recovery readiness through periodic verification and documented recovery testing.

# 4. Recovery Objectives

The GSP platform maintains recovery objectives based on the backup and replication controls implemented for critical database services.

The target Recovery Point Objective (RPO) for PostgreSQL database recovery is 1 minute, supported by continuous streaming replication and frequent archive log backups.

The target Recovery Time Objective (RTO) for critical GSP database service restoration is 30 minutes, subject to the nature of the disruption, infrastructure availability and operational conditions at the time of recovery.

# 5. Backup & Recovery Principles

The GSP platform operates according to the following principles:

- Backup processes are performed in accordance with established operational procedures.
- Backup information is protected from unauthorized access and modification.
- PostgreSQL replication and backup mechanisms are monitored and verified.
- Failed backups are investigated and corrective action is taken where required.
- Backup information is retained for 30 days.
- Backup information is encrypted in S3.
- Access to backup storage is restricted to authorised individuals.
- Backup information is maintained separately from production environments.
- Recovery activities are performed through controlled operational procedures.
- Recovery capabilities are periodically verified and recovery testing is documented.
- Backup and recovery controls are periodically reviewed.

# 6. Recovery Operations

Backup and recovery activities are managed through structured operational processes.

The operational framework includes:

- Backup planning.
- Backup execution and monitoring.
- Backup failure handling.
- Backup protection and access control.
- Recovery initiation and authorisation.
- Restoration activities.
- Recovery verification.
- Recovery testing and evidence retention.
- Periodic review of recovery readiness.

# 7. Compliance

Compliance with this policy is supported through documented procedures, operational practices, backup records, replication evidence, recovery test records, access control evidence and implementation evidence.

Detailed operational processes and technical controls are maintained separately to support the effective implementation of this policy.

# Revision History

| Date | Revision | Change Summary |
| ---- | -------- | -------------- |
| 2025-11-14 | 1.0 | Initial release of the backup and recovery policy. |
| 2026-02-05 | 1.1 | Updated backup scope, PostgreSQL replication, retention, RPO, RTO and recovery testing expectations. |
