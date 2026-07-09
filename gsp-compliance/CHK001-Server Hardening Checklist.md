---
title: SERVER HARDENING CHECKLIST
company: Blowbits Solutions LLP
classification: Internal
revision: '1.0'
last_update_date: 2026-07-09
logo: ../assets/octa-gst-logo.png
---

# 1. Purpose

This checklist defines the minimum hardening checks for AWS-hosted ARM-based Debian GNU/Linux 12 (bookworm) servers supporting the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The checklist is used to validate that GSP servers are securely configured, patched, monitored and operated using a consistent baseline.

# 2. Scope

This checklist applies to AWS-hosted ARM-based Debian 12 servers used for GSP application, API, monitoring, support and related infrastructure functions.

AWS-managed services and externally managed platforms are governed through their respective cloud security and operational controls.

# 3. Server Hardening Checklist

| Area                  | Check                                                                                                            | Expected Status              | Evidence                                             |
| --------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------- | ---------------------------------------------------- |
| Server baseline       | Server is provisioned using an approved AWS instance, VPC, subnet and Debian 12 image.                           | Implemented                  | AWS instance details, inventory or deployment record |
| Server baseline       | Server uses supported Debian 12 repositories and ARM-compatible trusted packages.                                | Implemented                  | Package source or update evidence                    |
| Server baseline       | AWS tags, hostname and inventory records identify the server purpose and ownership.                              | Implemented                  | AWS tags or inventory screenshot                     |
| Storage protection    | Attached storage volumes are encrypted where supported.                                                          | Implemented                  | AWS volume encryption evidence                       |
| Network access        | Inbound access is restricted to approved ports and trusted source networks using AWS security groups.            | Implemented                  | Security group screenshot or rule export             |
| Network access        | Unused inbound ports are blocked through AWS security groups and local firewall rules where applicable.          | Implemented                  | Security group, firewall or port review evidence     |
| Administrative access | Direct root login over SSH is disabled.                                                                          | Implemented                  | SSH configuration evidence                           |
| Administrative access | SSH key-based access is used where applicable.                                                                   | Implemented                  | SSH configuration or access record                   |
| Administrative access | Password-based SSH login is disabled where key-based access is implemented.                                      | Implemented                  | SSH configuration evidence                           |
| Administrative access | Administrative access uses named users or approved access mechanisms.                                            | Implemented                  | User list or access record                           |
| Administrative access | Sudo privileges are restricted to authorised administrators only.                                                | Implemented                  | Sudoers or group membership review                   |
| Administrative access | Unused, default or unauthorised accounts are removed or disabled.                                                | Implemented                  | User account review evidence                         |
| Least privilege       | Server access is limited to operational need and approved role ownership.                                        | Implemented                  | Access approval or review record                     |
| Patch management      | Operating system and security updates are applied in accordance with patch management requirements.              | Implemented                  | Patch status or update record                        |
| Patch management      | Critical Debian, AWS and application dependency advisories are reviewed.                                         | Implemented                  | Advisory review or patch ticket                      |
| Patch management      | Servers are rebooted after kernel or critical system updates where required.                                     | Implemented                  | Update/reboot record where applicable                |
| Package management    | Unused packages, tools and services are removed or disabled where not required.                                  | Implemented                  | Package/service review evidence                      |
| Service hardening     | Only required services, listeners and scheduled jobs are enabled.                                                | Implemented                  | Service list or port scan evidence                   |
| Service hardening     | Application services run with least required privileges.                                                         | Implemented                  | Service account or unit file evidence                |
| Secrets management    | Secrets and credentials are stored using approved secure mechanisms.                                             | Implemented                  | Configuration review or secret storage evidence      |
| Secrets management    | Credentials are not hardcoded in scripts, configuration files or source code.                                    | Implemented                  | Configuration or code review evidence                |
| File permissions      | Application, configuration and log paths have restricted permissions.                                            | Implemented                  | File permission review evidence                      |
| Logging               | System, authentication, application and security-relevant logs are enabled where applicable.                     | Implemented                  | Logging configuration evidence                       |
| Logging               | Logs are forwarded or retained in accordance with logging and monitoring requirements.                           | Implemented                  | Log group, retention or forwarding evidence          |
| Logging               | Logs are protected from unauthorised access, modification or deletion.                                           | Implemented                  | IAM, log storage or access control evidence          |
| Time synchronisation  | AWS-managed or approved time synchronisation is used for accurate timestamps.                                    | Implemented                  | Time sync configuration evidence                     |
| Monitoring            | Service health, resource utilisation and security-relevant events are monitored where applicable.                | Implemented                  | Monitoring dashboard or alert evidence               |
| Backup readiness      | Application, infrastructure and operational configurations required for recovery are backed up where applicable. | Implemented                  | Backup configuration or ticket evidence              |
| Backup readiness      | Database backup and recovery controls are maintained in accordance with backup and recovery requirements.        | Implemented                  | Backup records or recovery evidence                  |
| Backup protection     | Backup storage is encrypted and access-restricted.                                                               | Implemented                  | S3/IAM/encryption evidence                           |
| Validation            | Hardening is reviewed after provisioning, significant configuration changes and periodic review.                 | Implemented                  | Review ticket, checklist or approval record          |
| Exception handling    | Deviations are remediated or documented with compensating controls and approval where required.                  | Implemented / Not Applicable | Exception or risk acceptance evidence                |

# 4. Review and Sign-off

| Field                     | Value |
| ------------------------- | ----- |
| Server / Environment      |       |
| Review Date               |       |
| Reviewed By               |       |
| Approved By               |       |
| Review Result             |       |
| Open Actions / Exceptions |       |
| Next Review Due           |       |

# 5. Reference Documents

- POL002 - Access Control Policy
- POL005 - Infrastructure Security Policy
- POL006 - Logging and Monitoring Policy
- POL007 - Backup and Recovery Policy
- SOP002 - User & Credential Management Procedure
- SOP003 - Change Management Procedure
- SOP004 - Backup & Recovery Procedure
- SOP007 - Log Monitoring & Review Procedure
- SOP008 - Patch & Security Update Procedure
- Roles, Responsibilities & Access Matrix

# Revision History

| Date       | Revision | Change Summary                                                                       |
| ---------- | -------- | ------------------------------------------------------------------------------------ |
| 2026-07-09 | 1.0      | Formalised existing server hardening practices for AWS-hosted Debian 12 ARM servers. |
