---
title: BACKUP & RECOVERY PROCEDURE
company: Blowbits Solutions LLP
classification: Internal
---

# 1. Purpose

This Standard Operating Procedure (SOP) defines the process for performing backups, monitoring backup completion, protecting backup information, handling backup failures, restoring platform components and verifying recovery capabilities for the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective of this procedure is to ensure that platform components and operational information required to restore GSP services are protected and recoverable following operational disruptions.

# 2. Scope

This procedure applies to production PostgreSQL databases, PostgreSQL archive logs, application configurations, infrastructure configurations and operational information required to support recovery of the Blowbits Solutions LLP GSP platform.

Operational records and supporting evidence generated during backup, replication, recovery and recovery testing activities are maintained separately.

# 3. Roles & Responsibilities

Backup and recovery activities shall be performed by authorised internal roles defined in the Roles, Responsibilities & Access Matrix.

| Role | Backup & Recovery Responsibility |
| ---- | -------------------------------- |
| **Platform Operations Lead** | Execute and monitor backup activities; investigate backup failures; perform recovery activities; validate restored services. |
| **Information Security Lead** | Review backup protection controls, backup access restrictions and security implications of recovery activities where applicable. |
| **GSP Governance Lead** | Provide approval or oversight for significant production recovery activities, exceptions and repeated backup failures where required. |

# 4. Backup Scope

Backup and recovery coverage includes:

- PostgreSQL production database information.
- PostgreSQL archive logs required for point-in-time recovery.
- Application configurations required to restore GSP services.
- Infrastructure or deployment configurations required for recovery.
- Operational records or configuration information required to support restoration and verification.

# 5. Backup Frequency, Retention and Recovery Objectives

The following backup and recovery controls are maintained for PostgreSQL database services:

| Control | Frequency / Objective | Retention / Target |
| ------- | --------------------- | ------------------ |
| PostgreSQL streaming replication | Continuous replication to a second availability zone | Target RPO: 1 minute |
| PostgreSQL full backup | Weekly | 30 days |
| PostgreSQL archive log backup | Every 5 minutes | 30 days |
| Critical database service restoration | As required during recovery | Target RTO: 30 minutes |

Application configurations and recovery-relevant operational configurations shall be backed up according to operational requirements and retained for 30 days where applicable.

Backups shall be verified for successful completion. Failed backups shall be investigated and remediated in accordance with this procedure.

# 6. Backup & Recovery Procedure

## Step 1 – Backup Planning

Backup requirements shall be identified based on operational criticality, recovery objectives and restoration requirements.

The planning process includes:

- Systems and databases requiring backup.
- Application and infrastructure configurations requiring protection.
- Backup schedule and frequency.
- Backup retention requirements.
- Backup storage location.
- Recovery objectives and verification requirements.

## Step 2 – Backup Execution

Backup activities shall be performed through approved operational processes.

The procedure includes:

- Continuous PostgreSQL streaming replication to a second availability zone.
- Weekly full PostgreSQL backup.
- PostgreSQL archive log backup every 5 minutes.
- Backup of application configurations according to operational requirements.
- Verification of successful backup completion.
- Recording of backup activities.

## Step 3 – Backup Monitoring and Failure Handling

The Platform Operations Lead shall monitor backup and replication status through available operational tools, logs or provider records.

Where a backup or replication process fails:

- The failure shall be recorded.
- The Platform Operations Lead shall investigate the cause of failure.
- The failed backup shall be retried or corrective action shall be initiated where required.
- The impact on recovery objectives shall be assessed.
- Repeated or significant backup failures shall be escalated to the GSP Governance Lead.
- Corrective action evidence shall be retained.

## Step 4 – Backup Protection

Backup information shall be stored separately from the production environment and protected through appropriate security controls.

Backup protection controls include:

- Encryption of backups stored in S3.
- Restriction of S3 backup bucket access to authorised individuals.
- Access control based on least privilege.
- Protection of backup information from unauthorised modification or deletion.
- Periodic review of access to backup storage.

## Step 5 – Recovery Initiation and Authorisation

Recovery activities may be initiated when production data, database services, application configurations or platform components require restoration.

Routine recovery verification or recovery testing may be initiated by the Platform Operations Lead.

Production restoration or significant recovery activity shall be notified to the GSP Governance Lead. Approval from the GSP Governance Lead shall be obtained where the recovery activity may affect production availability, data integrity, regulatory commitments or external communication obligations.

The Information Security Lead shall be involved where recovery activities relate to suspected compromise, data exposure, credential compromise or other security-impacting events.

## Step 6 – Restoration

Where recovery is required, restoration shall be performed using approved operational procedures.

Restoration activities may include:

- Promoting or restoring from the second availability zone where appropriate.
- Restoring PostgreSQL from full backup.
- Applying PostgreSQL archive logs for point-in-time recovery.
- Restoring application configurations.
- Restoring infrastructure or deployment configurations.
- Validating database and application availability.
- Monitoring restored services after recovery.

## Step 7 – Recovery Verification

Following restoration, the Platform Operations Lead shall verify that recovered services are operational.

Verification activities include:

- Validation of restored database availability.
- Validation of recovered application configuration.
- Confirmation of service availability.
- Confirmation of data consistency where applicable.
- Review of logs or monitoring information after recovery.
- Documentation of recovery results.

## Step 8 – Closure and Records

Following completion of backup failure remediation, recovery testing or production recovery:

- Backup, recovery or test records shall be updated.
- Corrective actions shall be tracked where applicable.
- Recovery results shall be documented.
- Required approvals or review evidence shall be retained.
- Significant issues shall be reviewed by the GSP Governance Lead where required.

# 7. Recovery Testing

Recovery testing shall be performed periodically to validate that backup and recovery procedures remain effective.

Recovery testing should validate, where applicable:

- Restoration from PostgreSQL full backup.
- Point-in-time recovery using archive logs.
- Availability and usability of restored data.
- Recovery of application configurations.
- Ability to meet defined RPO and RTO targets.

Recovery test results shall be documented. Issues identified during recovery testing shall be investigated and tracked to closure.

# 8. Backup Records and Evidence

The following records may be maintained, where applicable:

- PostgreSQL streaming replication status evidence.
- Weekly full backup completion records.
- PostgreSQL archive log backup records.
- Backup verification evidence.
- Backup failure records.
- Backup failure investigation and corrective action records.
- S3 backup encryption evidence.
- Backup storage access control evidence.
- Recovery authorisation or approval records.
- Recovery execution records.
- Restore validation evidence.
- Recovery test records.
- Corrective action records.

# 9. Review

This procedure shall be reviewed annually or whenever significant changes occur to backup architecture, recovery objectives, database configuration, application architecture, infrastructure design or operational responsibilities.

# 10. Compliance

Compliance with this procedure is supported through documented backup records, replication evidence, recovery records, recovery test evidence, access control evidence and implementation evidence maintained in accordance with organisational procedures.

# Reference Documents

- POL-007 – Backup and Recovery Policy
- Roles, Responsibilities & Access Matrix
- Contact Directory
