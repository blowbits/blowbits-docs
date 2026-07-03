# BLOWBITS SOLUTIONS LLP

# ANNEXURE A

# GSP PLATFORM ARCHITECTURE, SECURITY DESIGN & INTEGRATION MODEL

**Prepared for:** GSTN GSP Security Assessment

---

# 1. Purpose

This annexure describes the logical architecture, integration model, request processing lifecycle and trust boundary design governing the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The GSP platform provides a secure integration framework through which authorised consuming applications access the Goods and Services Tax Network (GSTN). The architecture establishes a common processing model to ensure consistent authentication, request validation, secure communication and controlled request processing for all authorised applications.

---

# 2. Platform Overview

The Blowbits Solutions LLP GSP platform operates as a centralized API integration platform between authorised consuming applications and GSTN services.

The platform is currently consumed by an internal compliance application interface for accessing GSTN services. The same architectural framework is designed to support authorised Application Service Providers (ASPs), ensuring that all consuming applications interact with GSTN through an identical authenticated integration model.

## 2.1 Architecture Scope

This annexure describes the logical architecture of the Blowbits GSP platform.

Operational controls relating to identity management, infrastructure security, monitoring, logging, backup, vulnerability management and operational governance are documented in their respective annexures.

## 2.2 GSP Service Interaction Model

```text
                  +----------------------+
                  |     GSTN Services    |
                  +----------------------+
                             ▲
                             │
                   Secure Communication
                             │
                  +----------------------+
                  |  Blowbits GSP APIs   |
                  |     & Services       |
                  +----------------------+
                       ▲            ▲
                       │            │
               +---------------+  +------------------+
               |   Internal App   |  | Authorised ASPs |
               +---------------+  +------------------+
```

All authorised consuming applications access GSTN services exclusively through the Blowbits GSP platform. Direct communication between consuming applications and GSTN is not supported.

---

# 3. Trust Boundary Architecture

The platform separates participating systems into distinct trust boundaries. Appropriate security controls are applied whenever requests transition between these boundaries.

```text
+-----------------------------------------+
|       Consuming Applications            |
|     (Internal App / Authorised ASPs)        |
+-----------------------------------------+
                  │
                  │ Secure Transport
                  ▼
+-----------------------------------------+
|        Blowbits GSP Platform            |
|      Secure Request Processing          |
+-----------------------------------------+
                  │
                  │ Secure Transport
                  ▼
+-----------------------------------------+
|            GSTN Services                |
+-----------------------------------------+
```

## 3.1 Operational Domains

### Consuming Applications

Applications authorised to access GSP services, including the internal consumer application and authorised ASP applications.

### Blowbits GSP Platform

Provides authentication, request validation, request processing, secure communication with GSTN and transaction recording.

### GSTN Services

Represents the external GSTN services accessed through the Blowbits GSP platform.

---

# 4. Request Processing Lifecycle

Every request processed by the Blowbits GSP platform follows a defined lifecycle before communication with GSTN.

```text
Application Request
        │
        ▼
Authentication
        │
        ▼
Request Validation
        │
        ▼
Request Processing
        │
        ▼
Secure Communication with GSTN
        │
        ▼
Response Processing
        │
        ▼
Application Response

(Transaction activities are recorded throughout the processing lifecycle.)
```

## 4.1 Access Revocation

The platform provides administrative controls to suspend or revoke application credentials.

During authentication, application status is verified before request processing begins. Applications that have been suspended or revoked are prevented from accessing GSP services.

---

# 5. Communication Security & Credential Protection

## 5.1 Credential Protection

Credentials used for communication with GSTN are protected through server-side security controls.

- Credentials are encrypted before being stored in persistent storage.
- Hardcoding credentials within application source code is prohibited.
- Access to active credentials is restricted to authorised server-side processes responsible for establishing authenticated communication with GSTN.

## 5.2 Secure Communication

Communication between the Blowbits GSP platform and GSTN is established through secure communication channels in accordance with GSP connectivity requirements.

---

# 6. Architectural Principles

The Blowbits GSP platform is designed around the following principles:

- All communication with GSTN occurs through the GSP platform.
- Consuming applications do not communicate directly with GSTN.
- Every request is authenticated before processing.
- Requests are validated prior to communication with GSTN.
- Communication between systems uses secure transport.
- The platform provides a common authenticated integration framework for authorised applications.

---

# 7. Architecture Characteristics

| Characteristic | Description |
|---------------|-------------|
| Single Integration Platform | All authorised applications access GSTN through a common GSP platform. |
| Authenticated Request Processing | Every request is authenticated before processing. |
| Trust Boundary Separation | The architecture separates consuming applications, the GSP platform and GSTN services. |
| Secure Communication | Communication between systems uses secure transport mechanisms. |
| Controlled Request Processing | Every request follows a defined processing lifecycle before communication with GSTN. |

---

