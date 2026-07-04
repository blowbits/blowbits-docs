---
title: USER & CREDENTIAL MANAGEMENT PROCEDURE
company: Blowbits Solutions LLP
classification: Internal
revision: "1.1"
last_update_date: 2026-01-20
logo: ../assets/octa-gst-logo.png
---

# 1. Purpose

This Standard Operating Procedure (SOP) defines the process for requesting, approving, provisioning, modifying, reviewing, protecting and revoking user accounts, privileged accounts, service accounts and authentication credentials within the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective of this procedure is to ensure that user identities, access permissions and authentication credentials are managed through controlled operational processes to protect the confidentiality, integrity and availability of GSP services.

# 2. Scope

This procedure applies to user accounts, privileged accounts, administrative accounts, service accounts, application credentials, API credentials and system credentials used within the Blowbits Solutions LLP GSP platform.

Operational records and supporting evidence generated during account, access and credential lifecycle management are maintained separately.

# 3. Roles & Responsibilities

User and credential management activities shall be performed by authorised internal roles defined in the Roles, Responsibilities & Access Matrix.

| Role                          | User & Credential Management Responsibility                                                                                              |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **Platform Operations Lead**  | Provision, modify and revoke approved user accounts, service accounts, access permissions and operational credentials.                   |
| **Information Security Lead** | Review privileged access, credential protection controls, suspected credential compromise and access-related security concerns.          |
| **GSP Governance Lead**       | Approve privileged access, access exceptions, credential exceptions and significant access decisions where required.                     |
| **All Personnel**             | Protect assigned credentials, use access only for authorised purposes and report suspected credential compromise or unauthorised access. |

# 4. Account and Credential Types

This procedure applies to the following account and credential types:

- User accounts.
- Administrative or privileged accounts.
- Service accounts.
- Application identities and application credentials.
- API credentials.
- System credentials and secrets.

# 5. User & Credential Management Procedure

## Step 1 – Access Request

Access requests shall be submitted through the prescribed operational process.

The request shall specify:

- User, application or service identity.
- Required access level.
- Business justification.
- Required systems, services or credentials.
- Whether privileged access is required.
- Required duration, where access is temporary.

## Step 2 – Access Review and Approval

Access requests shall be reviewed before accounts are created or modified.

The review shall consider:

- Business need.
- Assigned role or responsibility.
- Least privilege.
- Need-to-know.
- Privileged access impact.
- Segregation of duties or compensating controls where applicable.

Privileged access, access exceptions and credential exceptions shall be approved by the GSP Governance Lead or an authorised delegate where required.

## Step 3 – Account Provisioning

Following approval, the Platform Operations Lead shall provision accounts and access permissions according to approved requirements.

Provisioning activities may include:

- Creating user, administrative, service or application accounts.
- Assigning approved access permissions.
- Enabling multi-factor authentication (MFA) where supported and applicable.
- Provisioning authentication credentials.
- Limiting access according to operational requirements.
- Recording provisioning activity.

## Step 4 – Credential Provisioning and Protection

Authentication credentials shall be protected throughout their lifecycle.

Credential protection controls include:

- Controlled generation of credentials.
- Secure storage of system credentials and secrets.
- Encryption or approved secure secret storage where supported.
- Protection against unauthorised disclosure.
- Prohibition of plaintext credential storage.
- Prohibition of hardcoding credentials in application source code, scripts, configuration repositories or client-side components.
- Controlled administrative access to credential stores.
- Restriction of credential access according to least privilege.

## Step 5 – Privileged Access Handling

Privileged access shall be limited to authorised operational requirements and approved before assignment.

Privileged access activities include:

- Confirming approval before provisioning.
- Restricting privileges according to least privilege.
- Enabling MFA where supported.
- Logging or monitoring privileged activity where supported by the system or service.
- Reviewing privileged access periodically.
- Removing privileged access promptly when no longer required.

## Step 6 – Access Modification

Access shall be modified when operational responsibilities, system access requirements or security requirements change.

Modification activities may include:

- Adding approved access.
- Reducing access no longer required.
- Changing role-based permissions.
- Updating service account or application credential scope.
- Suspending access temporarily where required.

## Step 7 – Access Review

User, administrative, privileged and service account access shall be reviewed periodically to verify continued operational need.

The review should verify:

- Assigned access remains required.
- Privileged access remains justified.
- Service accounts and application credentials remain active and necessary.
- Unnecessary or obsolete access is removed.
- Exceptions remain valid and compensating controls remain appropriate.

Access review evidence shall be retained.

## Step 8 – Credential Rotation or Replacement

Credentials shall be rotated or replaced where required by operational or security requirements.

Credential rotation or replacement shall be performed when:

- Credential compromise is suspected or confirmed.
- A credential is exposed or mishandled.
- Operational responsibility changes.
- A service account or application identity no longer requires the credential.
- Security or compliance considerations require replacement.

Credential replacement activities shall be recorded where applicable.

## Step 9 – Access Revocation

Access shall be revoked promptly when:

- Access is no longer required.
- Employment or contractual engagement ends.
- Operational responsibilities change.
- Service accounts, application identities or API credentials are retired.
- Security or compliance considerations require access removal.

Revocation activities may include:

- Disabling or removing user accounts.
- Removing privileged access.
- Revoking service account or API credentials.
- Rotating shared or dependent credentials where required.
- Updating access records.

## Step 10 – Credential Compromise Response

Suspected or confirmed credential compromise shall be reported to the Information Security Lead.

Response activities may include:

- Disabling affected accounts or credentials.
- Rotating or replacing exposed credentials.
- Reviewing logs or activity records where available.
- Assessing unauthorised access or data exposure.
- Initiating incident response where required.
- Recording corrective actions.

# 6. Records and Evidence

The following records may be maintained, where applicable:

- Access request records.
- Access approval records.
- Account provisioning records.
- MFA enablement evidence where applicable.
- Privileged access approval and review records.
- Service account or application credential records.
- Access review evidence.
- Access modification records.
- Access revocation evidence.
- Credential rotation or replacement evidence.
- Credential compromise response records.
- Exception approval records.

# 7. Review

This procedure shall be reviewed annually or whenever significant changes occur to access control processes, credential management processes, platform architecture, identity systems or operational responsibilities.

# 8. Compliance

Compliance with this procedure is supported through documented operational records, access records, credential records, review records and implementation evidence maintained in accordance with organisational procedures.

# Reference Documents

- POL-002 – Access Control Policy
- POL-003 – Password & Credential Management Policy
- Roles, Responsibilities & Access Matrix

# Revision History

| Date | Revision | Change Summary |
| ---- | -------- | -------------- |
| 2025-11-18 | 1.0 | Initial release of the user and credential management procedure. |
| 2026-01-20 | 1.1 | Updated account lifecycle, privileged access, credential protection and evidence requirements. |
