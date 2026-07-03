---
title: ANNEXURE B - IDENTITY, API SECURITY & CRYPTOGRAPHIC CONTROLS
company: Blowbits Solutions LLP
classification: Internal
---

**Prepared for:** GSTN GSP Security Assessment

# 1. Purpose

This annexure describes the identity management framework, API security controls and cryptographic protection mechanisms implemented within the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective of these controls is to ensure that only authorised applications are permitted to access GSP services and that authentication credentials and sensitive connection information remain protected throughout their lifecycle.

# 2. Identity Management

The Blowbits GSP platform maintains a controlled identity framework for all authorised consuming applications.

## 2.1 Identity Framework

Each authorised application is assigned a unique application identity before access to GSP services is provisioned.

Application identities are maintained independently to ensure logical separation between consuming applications and to support controlled access management.

## 2.2 Identity Lifecycle

Application identities are managed throughout their operational lifecycle.

The identity lifecycle supports:

- Provisioning of authorised applications.
- Modification of application information.
- Suspension of application access.
- Revocation of application access.
- Periodic review of active application identities.

Application status is verified during authentication before requests are processed.

# 3. API Security Framework

The Blowbits GSP platform applies security controls before processing every request received from consuming applications.

## 3.1 Authentication

Every request is authenticated before processing.

Requests that fail authentication are rejected before communication with GSTN.

## 3.2 Request Validation

Incoming requests are validated to ensure that only authorised and valid requests are processed.

Requests that fail validation are rejected without being forwarded to GSTN.

## 3.3 Request Identification

Each request is assigned a unique transaction identifier to support operational monitoring, transaction traceability and audit activities.

# 4. Credential Protection

Authentication credentials used for communication with GSTN are protected through controlled security mechanisms.

The implemented controls include:

- Encryption of credentials before persistent storage.
- Prohibition of plaintext credential storage.
- Restricted access to active credentials through authorised server-side processes only.
- Prohibition of embedding credentials within application source code or client-side components.

# 5. Cryptographic Controls

The Blowbits GSP platform applies cryptographic controls to protect authentication credentials and secure communication between participating systems.

The cryptographic framework includes the following control objectives:

- Protection of sensitive credentials stored within the platform.
- Protection of authentication information during transmission.
- Secure communication between authorised applications, the GSP platform and GSTN.
- Controlled access to cryptographic material used by the platform.

# 6. Identity & Security Principles

The identity and API security framework is based on the following principles.

- Every authorised application possesses a unique identity.
- Authentication is completed before request processing.
- Requests are validated before communication with GSTN.
- Sensitive credentials are protected throughout their operational lifecycle.
- Secure communication is used for external integrations.
- Administrative controls support suspension and revocation of application access.

# 7. Security Characteristics

| Characteristic                | Description                                                                                                 |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------- |
| Unique Application Identity   | Each authorised application is assigned an independent identity.                                            |
| Controlled Identity Lifecycle | Application identities are provisioned, maintained and revoked through controlled administrative processes. |
| Authentication                | Every request is authenticated before processing.                                                           |
| Request Validation            | Invalid or unauthorised requests are rejected before processing.                                            |
| Credential Protection         | Sensitive credentials are protected through encryption and controlled access mechanisms.                    |
| Secure Communication          | Communication between participating systems uses secure transport mechanisms.                               |

## Document Relationship

This annexure defines the identity management and API security framework of the Blowbits GSP platform.

Operational procedures, infrastructure controls, monitoring, logging, backup, vulnerability management and governance processes are documented separately within the relevant annexures and supporting operational documents.
