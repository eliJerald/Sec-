# CompTIA Security+ SY0-701: Domain 1 - General Security Concepts Study Guide

This comprehensive guide covers all subjects outlined in Domain 1.0 (General Security Concepts) of the CompTIA Security+ SY0-701 exam objectives. It accounts for 12% of the exam.

## 1.1 Compare and Contrast Various Types of Security Controls

### Categories of Security Controls
Security controls are classified into categories based on *how* they are implemented:
*   **Technical (Logical) Controls**: Hardware or software mechanisms used to manage access and protect resources. *Examples: Firewalls, Intrusion Detection Systems (IDS), encryption, antivirus software.*
*   **Managerial (Administrative) Controls**: Policies, procedures, and rules that dictate how security is managed and implemented. *Examples: Security policies, risk assessments, training and awareness programs.*
*   **Operational Controls**: Security measures executed by people on a day-to-day basis. *Examples: Security guards, change management processes, incident response procedures.*
*   **Physical Controls**: Tangible, real-world measures designed to prevent physical access to facilities or systems. *Examples: Fences, locks, mantraps/vestibules, bollards.*

### Types of Security Controls
Controls are also classified by their *function* or *intent*:
*   **Preventive**: Designed to stop an incident from occurring. *Examples: Firewalls, locks, security guards, Data Loss Prevention (DLP).*
*   **Deterrent**: Designed to discourage an attacker from attempting an intrusion. *Examples: Warning signs, visible security cameras, lighting.*
*   **Detective**: Designed to identify and record an incident while or after it happens. *Examples: Log monitoring, IDS, security cameras (recording).*
*   **Corrective**: Designed to fix a system or mitigate damage after an incident. *Examples: Restoring from backups, patching vulnerabilities, restarting a crashed service.*
*   **Compensating**: An alternative or "Plan B" control used when the primary control is unfeasible. *Example: Placing a strict firewall in front of a legacy device that can no longer be patched.*
*   **Directive**: Rules or policies that dictate user behavior. *Examples: Acceptable Use Policy (AUP), compliance regulations.*

---

## 1.2 Summarize Fundamental Security Concepts

### Core Principles
*   **CIA Triad**:
    *   **Confidentiality**: Ensuring data is only accessible to authorized individuals (e.g., Encryption, Access Controls).
    *   **Integrity**: Ensuring data is not altered or tampered with (e.g., Hashing, Digital Signatures).
    *   **Availability**: Ensuring data and systems are accessible when needed (e.g., Redundancy, Load Balancing, Backups).
*   **Non-repudiation**: Guaranteeing that a sender cannot deny having sent a message or performed an action, achieved via **Digital Signatures**.
*   **AAA (Authentication, Authorization, and Accounting)**:
    *   **Authentication**: Proving you are who you say you are (e.g., passwords, biometrics).
    *   **Authorization**: Determining what you are allowed to do (e.g., permissions, access control lists).
    *   **Accounting**: Tracking what you did (e.g., logging, auditing).
*   **Gap Analysis**: Comparing the current state of an organization's security posture against a desired standard or framework to identify missing controls.

### Zero Trust Architecture
The principle of "never trust, always verify." No user or device is trusted implicitly, even if they are inside the corporate network.
*   **Control Plane (The Brains)**: Makes the decisions about access.
    *   **Policy Engine**: Analyzes context (device health, location) to make an access decision.
    *   **Policy Administrator**: Executes the decision and issues tokens.
    *   **Adaptive Identity**: Adjusting access privileges dynamically based on real-time risk/context.
    *   **Threat Scope Reduction**: Limiting the "blast radius" if a breach occurs.
*   **Data Plane (The Muscle)**: Where the actual traffic flows and is enforced.
    *   **Policy Enforcement Point (PEP)**: The gatekeeper that physically allows or blocks the traffic based on the Control Plane's orders.
    *   **Implicit Trust Zones**: Areas where all entities trust each other (Zero Trust tries to eliminate or shrink these).

### Physical Security
*   **Bollards**: Sturdy, short, vertical posts designed to stop vehicles from ramming into a building.
*   **Access Control Vestibule (Mantrap)**: A small space with two interlocking doors. The first door must close before the second opens, preventing **tailgating**.
*   **Fencing & Lighting**: Basic perimeter deterrents and preventive controls.
*   **Video Surveillance & Security Guards**: Provide both deterrent and detective capabilities.
*   **Sensors**:
    *   **Infrared (PIR)**: Detects body heat. Best for indoor office environments.
    *   **Pressure**: Detects weight (e.g., floor mats).
    *   **Microwave**: Emits pulses to detect movement; can penetrate walls.
    *   **Ultrasonic**: Uses sound waves; highly sensitive to air movement (HVAC).

### Deception and Disruption Technology
Used to trick attackers, waste their time, and gather intelligence.
*   **Honeypot**: A single decoy system designed to look vulnerable and attract attackers.
*   **Honeynet**: A network of multiple honeypots.
*   **Honeyfile**: A fake file meant to detect unauthorized access. *Crucial: Must never contain real user data.*
*   **Honeytoken**: A fake piece of data (like a fake API key or database record) acting as a digital tripwire.

---

## 1.3 Change Management Processes

A formalized process to ensure changes to IT systems do not cause outages or introduce security vulnerabilities.
*   **Business Processes**:
    *   **Impact Analysis**: Done *before* the change to predict what systems/users will be affected.
    *   **Backout Plan (Rollback Plan)**: The specific steps to safely undo the change and revert to the original state if things go wrong.
    *   **Maintenance Window**: The approved, scheduled timeframe (usually off-hours) to perform the change.
*   **Technical Implications**:
    *   Changes may involve updating **Allow lists/deny lists**, facing **downtime**, managing **legacy applications**, or dealing with complex **dependencies**.
*   **Documentation & Version Control**: Ensuring that network diagrams and standard operating procedures (SOPs) are updated after a change. Version control tracks code and configuration changes securely.

---

## 1.4 Cryptographic Solutions

### Public Key Infrastructure (PKI)
*   **Public Key**: Shared openly; used to encrypt data *sent to* the owner, or to verify their digital signature.
*   **Private Key**: Kept secret by the owner; used to decrypt received data, or to create a digital signature.
*   **Key Escrow**: Securely storing a copy of private keys with a trusted third party.

### Encryption
*   **Symmetric Encryption**: Uses the same key to encrypt and decrypt. Fast, good for bulk data (e.g., AES).
*   **Asymmetric Encryption**: Uses a key pair (Public/Private). Slower, good for key exchange and signatures (e.g., RSA, ECC).
*   **Levels of Encryption**:
    *   **Full-Disk Encryption (FDE)**: Encrypts the entire storage drive, protecting all data at rest from physical theft.
    *   **Database/Record/File level**: Encrypts specific pieces of data.

### Cryptographic Tools & Hardware
*   **TPM (Trusted Platform Module)**: A secure microchip built into a motherboard that generates, stores, and manages cryptographic keys at the hardware level.
*   **HSM (Hardware Security Module)**: A dedicated, external piece of enterprise hardware/appliance used to manage keys and perform intense cryptographic operations.
*   **Secure Enclave**: A secure, isolated region of a processor (CPU) for protecting sensitive data.

### Obfuscation & Hashing
*   **Tokenization**: Replacing sensitive data (like credit cards) with a non-sensitive equivalent (a token) used as a reference to a secure token vault.
*   **Data Masking**: Obscuring parts of data (e.g., `XXXX-XXXX-XXXX-1234`) for display purposes.
*   **Steganography**: Hiding a secret message inside an otherwise ordinary file (like an image or audio file).
*   **Hashing**: A one-way math function that creates a fixed-size string from any data. Used for **Integrity**. (e.g., SHA-256).
*   **Salting**: Adding random data to a password before hashing it. Defeats **Rainbow Table** attacks.
*   **Key Stretching**: Purposely slowing down the hashing process (e.g., Bcrypt, PBKDF2) to stop brute-force attacks.

### Certificates & Trust
*   **Certificate Authority (CA)**: The trusted entity that issues digital certificates.
*   **Root of Trust**: The foundational top-level CA that operating systems inherently trust.
*   **CSR (Certificate Signing Request)**: What an applicant generates and sends to the CA to apply for a certificate.
*   **Revocation**:
    *   **CRL (Certificate Revocation List)**: A downloaded list of all revoked certificates. Slow.
    *   **OCSP (Online Certificate Status Protocol)**: A real-time protocol to check a certificate's status. Fast.
*   **Self-Signed Certificates**: Created and signed by the user. Free, but inherently untrusted by web browsers.
*   **Third-Party Certificates**: Issued by a commercial CA. Trusted by default.
*   **Wildcard Certificate**: A single certificate used to secure a main domain and all its subdomains (e.g., `*.example.com`).

### Blockchain & Open Public Ledger
*   A decentralized, distributed database shared among nodes. Everyone has a copy of the ledger, making it transparent and nearly impossible to secretly alter past transactions.
