# Security+ SY0-701 Practice Questions


1. An attacker uses a 50 dollar device to copy the data from a high-level executive’s badge while standing near them in a crouded elevator. Which of the following best describes this attack type?

A. Biometric Spoofing
B. Brute force
C. Denial of Service
D. FRID Cloning
E. On path attack

**1. The Domain:**
Domain 2.0: Threats, Vulnerabilities, and Mitigations

**2. The Answer:**
D. FRID Cloning (Note: This is likely a typo for "RFID Cloning").

**3. Why that answer is correct:**
RFID (Radio Frequency Identification) cloning involves using a specialized, often inexpensive device to read and copy the information stored on a physical RFID card or badge. Because RFID technology uses radio waves to transmit data, an attacker simply needs to be in close physical proximity to the victim to secretly scan and steal the badge's credentials—perfectly describing the crowded elevator scenario.

**4. Why the other answers are incorrect:**
- **A. Biometric Spoofing:** This attack involves tricking a biometric scanner with fake biological traits (such as a fake fingerprint, an iris photo, or a 3D mask). It does not involve copying data from an electronic badge.
- **B. Brute force:** This is a computational method where an attacker guesses a password, PIN, or cryptographic key by systematically trying every possible combination until the correct one is found. It's not a physical proximity card-cloning attack.
- **C. Denial of Service (DoS):** A DoS attack aims to disrupt a system, network, or service and make it unavailable to legitimate users, usually by flooding it with traffic. It has nothing to do with stealing physical badge data.
- **E. On path attack:** Formerly known as a "Man-in-the-Middle" (MitM) attack, this involves an attacker secretly intercepting and potentially altering digital communications between two parties over a network. While it does involve intercepting data, it refers to active network traffic rather than physically copying an offline proximity badge.

--------------------------------------------------------------------------------


2. An organization is migrating its security stack to a cloud-native model to ensure mobile users receive the same security policy enforcement as office users. Which of the following would be the best choice for this requirement?

A. Software-defined networking
B. Secure Access Service Edge
C. Site-to-site IPsec tunneling
D. Next-Generation Firewall
E. Virtual Private Network Concentrator

**1. The Domain:**
Domain 3.0: Security Architecture

**2. The Answer:**
B. Secure Access Service Edge (SASE)

**3. Why that answer is correct:**
Secure Access Service Edge (SASE) is a cloud-native architecture that combines network security functions (like secure web gateways, cloud access security brokers, firewalls, and zero-trust network access) with wide area networking (WAN) capabilities. Because it is delivered as a cloud service, it ensures that all users—whether they are sitting in a corporate office or working from a mobile device at a coffee shop—are routed through the same security policies and protections before accessing the internet or corporate resources.

**4. Why the other answers are incorrect:**
- **A. Software-defined networking (SDN):** SDN separates the network's control logic from its forwarding hardware to make networks more agile and easier to manage, typically within a data center or campus. While modern, it is primarily a networking architecture, not a cloud-native security model for remote mobile users.
- **C. Site-to-site IPsec tunneling:** This creates a secure, encrypted connection between two fixed geographic locations (like a branch office and a main headquarters). It doesn't solve the problem of mobile, roaming users needing consistent security enforcement from anywhere.
- **D. Next-Generation Firewall (NGFW):** While an NGFW provides deep packet inspection and advanced security policies, traditional NGFWs are typically physical or virtual appliances deployed at a specific location's perimeter. It doesn't inherently push a cloud-native security model to remote mobile users.
- **E. Virtual Private Network Concentrator:** A VPN concentrator handles incoming remote access VPN connections, bringing remote users onto the corporate network. It forces all traffic to "trombone" or backhaul through the central data center to get security enforcement, which is exactly the non-cloud-native, legacy model organizations try to move away from with SASE.

--------------------------------------------------------------------------------


10. Sally wants to ensure that her change management process includes a procedure for what to do if the change fails. What should she create to handle this possibility?

A. An impact analysis
B. A backout plan
C. A regression test
D. A maintenance window

**1. The Domain:**
Domain 5.0: Security Program Management and Oversight

**2. The Answer:**
B. A backout plan

**3. Why that answer is correct:**
A backout plan (often called a rollback plan) defines the specific steps an organization will take to safely revert a system to its original, working state if a scheduled change fails, causes unexpected disruptions, or doesn't yield the expected results. This is a crucial fail-safe component of the change management process.

**4. Why the other answers are incorrect:**
- **A. An impact analysis:** This is performed *before* a change is implemented to evaluate what systems, processes, or users might be affected by the proposed change. It predicts risk but doesn't tell you how to undo a failed change.
- **C. A regression test:** This is a software testing practice to ensure that new code or changes didn't unintentionally break existing, previously working features. While it might *detect* a failure, it is not the procedure used to undo the change itself.
- **D. A maintenance window:** This is the approved, scheduled timeframe during which changes or disruptions are permitted (e.g., Sunday at 2 AM) to minimize business impact. It dictates *when* a change can happen, not how to recover if things go wrong.

--------------------------------------------------------------------------------


13. Ben has deployed a data loss prevention (DLP) tool that inspects data and flags specific data types for review before emails containing it are sent outside the organization. What control type best describes this type of solution?

A. Managerial
B. Detective
C. Corrective
D. Preventive

**1. The Domain:**
Domain 1.0: General Security Concepts

**2. The Answer:**
D. Preventive

**3. Why that answer is correct:**
A preventive control is designed to stop a security incident from occurring in the first place. Because this Data Loss Prevention (DLP) tool pauses or blocks the emails from actually being sent outside the organization until they are reviewed, it actively prevents the unauthorized data exfiltration from happening. 

**4. Why the other answers are incorrect:**
- **A. Managerial:** Managerial (or administrative) controls involve policies, procedures, regulations, and training. They are rules written on paper, not a technical tool actively inspecting and blocking data.
- **B. Detective:** A detective control is designed to identify and record an incident *after* or *as* it occurs (like a security camera or an alert log). If the DLP tool only sent an alert to an admin but still allowed the email to leave the network immediately, it would be detective. But because it holds the email before sending, it is preventive.
- **C. Corrective:** A corrective control is designed to fix or restore a system *after* a security incident has already happened (like restoring from a backup or applying a patch).

--------------------------------------------------------------------------------


16. Charles wants to reduce the threat scope of compromised credentials. What type of the following security controls is best suited to meeting this need?

A. Single sign-on
B. Federation
C. Zero trust
D. Multifactor authentication (MFA)

**1. The Domain:**
Domain 3.0: Security Architecture

**2. The Answer:**
C. Zero trust

**3. Why that answer is correct:**
Zero Trust Architecture operates on the principle of "never trust, always verify." If an attacker steals (compromises) a user's credentials, the "threat scope" or "blast radius" is heavily reduced because Zero Trust enforces strict least privilege and micro-segmentation. Even with a valid password, the attacker won't automatically be granted wide access to the network; their access is continuously verified and limited strictly to only what that specific user needs to do their job. 

**4. Why the other answers are incorrect:**
- **A. Single sign-on (SSO):** SSO allows a user to authenticate once to access multiple systems. If credentials are compromised in an SSO environment, it actually *increases* the threat scope because the attacker now has the keys to multiple applications with one login.
- **B. Federation:** Federation is a way to link a user's identity across multiple separate organizations or domains (like using a Google login for a third-party site). Like SSO, if federated credentials are compromised, the attacker gains access across multiple organizations, widening the threat scope.
- **D. Multifactor authentication (MFA):** MFA is highly effective at *preventing* compromised credentials from being successfully used in the first place (because the attacker lacks the second factor). However, the question specifically asks what reduces the "threat scope" of the compromised credentials (i.e., shrinking the blast radius if an attacker *is* inside or authenticated). Zero trust directly limits what compromised identities can access once they are in.

--------------------------------------------------------------------------------


17. Carol wants to obfuscate data that is contained in her database. She wants to be able to refer to the data elements without having the actual data exposed. What type of obfuscation option should she select?

A. Tokenization
B. Encryption
C. Data masking
D. Data randomization

**1. The Domain:**
Domain 5.0: Security Program Management and Oversight

**2. The Answer:**
A. Tokenization

**3. Why that answer is correct:**
Tokenization is the process of replacing sensitive data (like a credit card number) with a non-sensitive equivalent, known as a "token." This token serves as a reference or identifier that maps back to the sensitive data through a highly secure tokenization system. This allows databases and applications to process and refer to the data elements using the token without ever storing or exposing the actual sensitive data.

**4. Why the other answers are incorrect:**
- **B. Encryption:** Encryption transforms data into a secure format (ciphertext) using a cryptographic key. While highly secure, it doesn't just act as a simple reference; the encrypted data itself contains the actual data and must be decrypted to be read, which requires managing encryption keys within the database environment.
- **C. Data masking:** Data masking (or redaction) obscures parts of the data, such as changing a credit card number to `XXXX-XXXX-XXXX-1234` so it can be safely displayed on a screen. However, the masked data cannot typically be used as a backend reference to the original data in the same way a token can.
- **D. Data randomization:** Data randomization replaces sensitive data with completely random characters or values. This is typically used for generating realistic test data for development environments, but because it breaks the link to the original data, it cannot be used to refer back to the actual data elements in a production environment.

**How Tokenization and Encryption are Used in Conjunction**
  1. The actual data isn't in the main database: You are exactly right. The real sensitive data (like a credit card number) gets sent straight to a highly secure, separate server (often called a "Token Vault"—our coat check room). The Token Vault hands back the token, and the main database only stores the token.
  2. Decryption exposes data: You're right again. If you just encrypt the main database, the applications that need to use the data have to decrypt it. While the data is decrypted (even for a split second in the computer's memory), a clever hacker could snatch it.
  3. Combining both is the ultimate defense: Your final point is exactly how big companies handle security! They use tokenization software to replace the super sensitive data with tokens in the main database. Then, as an extra layer of protection, they still encrypt the main database anyway.
- **Defense in Depth:** In the real world, companies use both! They use tokenization to replace highly sensitive data with tokens in their main database, and then they *still* encrypt that database. If a hacker steals and decrypts the database, they only get a list of useless coat check tickets!

--------------------------------------------------------------------------------


19. Selah's organization has recently experienced a breach and the private keys for her organization's certificates were exposed. What should she immediately do?

A. Reissue the certificates with changed hostnames and other details.
B. Replace the certificates with self- signed certificates until they can be replaced by the vendor.
C. Revoke the certificates and place them on a certificate revocation list.
D. Replace the certificates with wildcard certificates.

**1. The Domain:**
Domain 3.0: Security Architecture

**2. The Answer:**
C. Revoke the certificates and place them on a certificate revocation list.

**3. Why that answer is correct:**
When a private key is exposed, the certificate is instantly compromised because an attacker can use that key to impersonate the organization or decrypt secure traffic. The immediate and only secure response is to revoke the certificate (invalidating it) and add its serial number to the Certificate Revocation List (CRL) or update the OCSP responder so that client browsers know it can no longer be trusted.

**4. Why the other answers are incorrect:**
- **A. Reissue the certificates with changed hostnames and other details:** The hostname hasn't changed; the key was compromised. Changing the details doesn't address the fact that the old, compromised certificate is still out there and considered "valid" by anyone who hasn't been told otherwise.
- **B. Replace the certificates with self-signed certificates:** Self-signed certificates are not inherently trusted by public browsers or operating systems. Replacing a compromised cert with a self-signed one will cause immediate security warnings and trust errors for all users.
- **D. Replace the certificates with wildcard certificates:** A wildcard certificate (e.g., `*.example.com`) is just a type of certificate used to secure multiple subdomains. It has absolutely nothing to do with incident response for a compromised private key.

--------------------------------------------------------------------------------


22. Greg wants to implement a version control system to ensure that changes are made in ways that will not cause problems for his organization's critical software. Which of the following is not a common feature of version control systems designed for software source code?

A. Atomic operations
B. File locking
C. Regression testing
D. Tagging and labeling

**1. The Domain:**
Domain 3.0: Security Architecture

**2. The Answer:**
C. Regression testing

**3. Why that answer is correct:**
Regression testing is a software *testing* practice used to ensure that recent code changes haven't unintentionally broken existing, previously working features. While a development team will certainly *perform* regression testing (often by triggering it via automated CI/CD pipelines when code is pushed), it is not a native, built-in feature of the Version Control System (VCS) itself (like Git or Subversion).

**4. Why the other answers are incorrect:**
- **A. Atomic operations:** This is a common feature of a VCS. An atomic operation ensures that a commit is treated as a single unit—it either entirely succeeds or entirely fails, preventing partial or corrupted code updates from breaking the repository.
- **B. File locking:** This is a common feature (especially in centralized VCS like Subversion or Team Foundation Version Control) that prevents multiple developers from editing the same file at the exact same time and causing conflicts.
- **D. Tagging and labeling:** This is a standard VCS feature used to mark specific points in the repository's history as important (e.g., tagging a specific commit as "Version 1.0").

--------------------------------------------------------------------------------

24. Lisa wants to ensure that theft of a device will not lead to exposure of the data contained on the device if the device is locked or turned off. What type of encryption should she select to best ensure this?

A. Volume-level encryption
B. Full- disk encryption
C. File-level encryption
D. Partition-level encryption

**1. The Domain:** Domain 3: Security Architecture

**2. The Answer:** B. Full- disk encryption

**3. Why that answer is correct:**
Full-disk encryption (FDE) protects the entire contents of a storage drive. It encrypts the operating system, all system files, temporary files, swap space (virtual memory), and all user data. When a device is powered off or locked, the encryption keys are wiped from the computer\'s memory. If the device is stolen in this state, a thief cannot read any data without the proper authentication credentials. This provides the most comprehensive protection against physical theft.

**4. Why the other answers are incorrect:**
- **A. Volume-level encryption:** This only encrypts a specific storage volume. If sensitive data is written outside of this volume (like in temporary files or a pagefile on the main system volume), it remains unencrypted and vulnerable to exposure.
- **C. File-level encryption:** This only encrypts individually selected files. It requires the user to remember to encrypt specific data. The operating system, metadata, and temporary copies of the files remain unencrypted, creating opportunities for data leakage.
- **D. Partition-level encryption:** Similar to volume-level encryption, this only protects a single partition. If any sensitive data makes its way to a different, unencrypted partition on the device, it will be exposed if the device is stolen.

--------------------------------------------------------------------------------

25. Mahmoud has been asked to implement an allow list for websites that users at his company can visit. What concern should he bring up to management due to this request?

A. Allow lists cannot be used for websites.
B. Allow lists are overly permissive and are likely to allow unwanted sites to be visited.
C. Using an allow list for websites will take a lot of time to maintain.
D. Using an allow list for websites is easily bypassed.

**1. The Domain:** Domain 3: Security Architecture (and Domain 4: Security Operations)

**2. The Answer:** C. Using an allow list for websites will take a lot of time to maintain.

**3. Why that answer is correct:**
An allow list (also known as a whitelist) operates on the principle of "Implicit Deny." This means that every single website on the internet is automatically blocked by default, and a user can only access a site if the administrator has manually added it to the approved list. Because modern businesses rely on hundreds of different websites, and those websites constantly pull resources (like images and scripts) from many other hidden domains, building and constantly updating this list creates a massive, ongoing administrative burden for the IT team. 

**4. Why the other answers are incorrect:**
- **A. Allow lists cannot be used for websites:** This is false. Web proxies and enterprise firewalls can easily implement allow lists to control web traffic.
- **B. Allow lists are overly permissive and are likely to allow unwanted sites to be visited:** This is the exact opposite of reality. Allow lists are extremely restrictive, not permissive. A *block list* (blacklist) is what is considered overly permissive because it allows access to everything except what is explicitly blocked.
- **D. Using an allow list for websites is easily bypassed:** If implemented correctly on a corporate network (like routing all traffic through a secure web gateway or firewall), an allow list is very difficult for a standard user to bypass.

**Notes: Alternatives to Allow Lists**
Instead of a strict Allow List (which creates a huge administrative burden), companies typically use a combination of three methods:
1. **Block List (Deny List):** The exact opposite of an Allow List. The entire internet is open by default, *except* for specific websites manually added to a "banned" list.
2. **Content Filtering (Category Filtering):** A system (like a firewall or secure web gateway) automatically categorizes the internet. IT can block entire categories (like Gambling or Malware) with a single click.
3. **Exception List:** If a legitimate site is accidentally caught in a blocked category, IT can add that specific site to an Exception List (a tiny, manageable Allow List) to let it through.

--------------------------------------------------------------------------------

27. What hardware component is used to generate, store, and manage cryptographic keys?

A. A CPU
B. A NSA
C. A TPM
D. A CCA

**1. The Domain:** Domain 3: Security Architecture

**2. The Answer:** C. A TPM

**3. Why that answer is correct:**
A TPM (Trusted Platform Module) is a specialized, secure hardware microchip that is usually permanently installed on a computer's motherboard. Its primary purpose is to act as a secure vault to generate, store, and manage cryptographic keys. Because the keys are locked inside this dedicated hardware chip, they are highly protected against software-based attacks and malware. It is the exact chip we talked about earlier that stores the keys for Full-Disk Encryption!

**4. Why the other answers are incorrect:**
- **A. A CPU:** The Central Processing Unit is the "brain" of the computer that handles general calculations and runs the operating system. While it helps process data, it is not a dedicated, secure vault designed specifically for storing cryptographic keys.
- **B. A NSA:** The National Security Agency (NSA) is a United States government intelligence agency responsible for global monitoring, collection, and processing of information. It is an organization, not a piece of computer hardware.
- **D. A CCA:** In a cybersecurity context, CCA usually stands for "Chosen-Ciphertext Attack" (a type of cryptographic attack model) or "Common Cryptographic Architecture." Regardless, it is not a physical hardware component installed in a computer for key storage.

--------------------------------------------------------------------------------

28. Chris wants to check to see if a certificate has been revoked. What protocol can he use to validate the current status of a certificate?

A. TLS
B. OCRS
C. SSL
D. OCSP

**1. The Domain:** Domain 3: Security Architecture

**2. The Answer:** D. OCSP

**3. Why that answer is correct:**
OCSP stands for **Online Certificate Status Protocol**. When your web browser wants to make sure a website's digital certificate is still valid and hasn't been compromised, it uses OCSP to ask the Certificate Authority (the organization that issued the certificate) for a real-time status check. The server responds quickly with "good," "revoked," or "unknown." This is much faster and more efficient than downloading a massive list of every revoked certificate (which is called a CRL, or Certificate Revocation List).

**4. Why the other answers are incorrect:**
- **A. TLS (Transport Layer Security):** This is the actual encryption protocol used to secure traffic over the internet (it's what makes the "S" in HTTPS). While TLS relies on valid certificates to build that secure connection, it is not the protocol used to check the *revocation status* of those certificates.
- **B. OCRS:** This is a made-up acronym in this context, put there to confuse you because it looks similar to OCSP. In other areas of IT, OCR stands for Optical Character Recognition (like scanning a document into text), which has nothing to do with certificates.
- **C. SSL (Secure Sockets Layer):** This is the older, obsolete predecessor to TLS. Just like TLS, it is an encryption protocol, not a method for checking if a certificate has been revoked.

--------------------------------------------------------------------------------

29. Brian's organization uses a process where a secure module boots systems, then monitors them as each boot stage proceeds. It validates each signed boot stage and reports on whether the boot process was correct or not when complete. What is the secure module used to verify these stages called?

A. A secure initiation manager
B. A root of trust
C. A boot hash
D. A cryptographic boot manager

**1. The Domain:** Domain 3: Security Architecture

**2. The Answer:** B. A root of trust

**3. Why that answer is correct:**
A "Root of Trust" (RoT) is the foundational security component within a computer system (often embedded inside the TPM hardware chip we discussed earlier). Because the computer has to trust *something* from the very moment it powers on, the Root of Trust serves as that absolute, unquestionable starting point. During the boot process (often called Secure Boot or Measured Boot), the Root of Trust acts like a strict security guard, checking the digital signatures of every piece of software trying to load. If it verifies everything is correct and unaltered, the computer finishes booting.

**4. Why the other answers are incorrect:**
- **A. A secure initiation manager:** This is a completely fabricated term designed to sound highly technical and trick you on the exam. 
- **C. A boot hash:** A hash is a mathematical fingerprint of data used to prove that a file hasn't been tampered with. While the Root of Trust might *read* or *check* a hash during the boot process to verify a file's integrity, a hash itself is just a piece of data, not the active "secure module" doing the monitoring.
- **D. A cryptographic boot manager:** Like option A, this is another fabricated term that doesn't exist in standard cybersecurity frameworks.

**Notes: Secure Boot vs. Measured Boot (Handling Infections)**
*   **Secure Boot (The Strict Bouncer):** If the Root of Trust detects that boot files (like the OS) have been infected or altered, it **halts the boot process completely**. The computer will refuse to start and will display a security error.
*   **Measured Boot (The Tattletale):** The computer **will still boot up**, even if infected. However, the Root of Trust takes notes (measures hashes) of everything that loads. Once booted, it sends these notes to a central server (Remote Attestation). If the server detects an infection from these notes, it immediately blocks the computer from the corporate network.

--------------------------------------------------------------------------------

30. A vulnerability scan shows that an embedded device that Alice is responsible for has a vulnerability. She knows the vendor is no longer in business and that there is no updated firmware or software update for the device. To resolve the issue, Alice places a firewall between the device and the rest of the network and creates rules that prevent the vulnerable service from being available to other devices. What type of control has Alice deployed?

A. A directive control
B. A compensating control
C. A detective control
D. A procedural control

**1. The Domain:** Domain 1: General Security Concepts

**2. The Answer:** B. A compensating control

**3. Why that answer is correct:**
A compensating control is a "Plan B" security measure that you use when the primary or ideal security control is impossible or too expensive to implement. In this scenario, the ideal primary control is obvious: patch the vulnerability by updating the device's firmware. However, since the vendor is out of business, patching is impossible. By putting a firewall in front of the device instead, Alice mitigated the risk using an alternative method. This is the textbook definition of a compensating control.

**4. Why the other answers are incorrect:**
- **A. A directive control:** This type of control uses rules and regulations to dictate user behavior (like an Acceptable Use Policy or a "No Tailgating" sign). A firewall is a technical piece of software/hardware, not a set of written directions for humans.
- **C. A detective control:** Detective controls are designed to identify and record an incident *as* or *after* it occurs (like security cameras, audit logs, or intrusion detection alerts). By actively blocking the vulnerable traffic with rules, Alice's firewall is acting as a preventative measure, not just watching and detecting.
- **D. A procedural control:** Procedural controls (often grouped under administrative controls) involve standard operating procedures, business processes, and employee training. Installing and configuring a firewall is a technical control, not a procedural one.

--------------------------------------------------------------------------------

### Question:
37. Renee wants to ensure that her logs support nonrepudiation. What should she do to ensure this?
A. Encrypt, then hash the logs.
B. Hash the logs and then digitally sign them.
C. Digitally sign the log file, then encrypt it.
D. Hash, then encrypt the logs.

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.2: Compare and contrast fundamental security concepts / Cryptography).

**2. The Answer and Explanation:**
**B. Hash the logs and then digitally sign them.**
Nonrepudiation guarantees that the sender or creator of a file cannot deny their action. This is achieved using digital signatures. The actual process of creating a digital signature involves two steps: first, you hash the file (to ensure integrity), and then you encrypt that hash using the sender's private key. This proves the file hasn't changed and that only the owner of the private key could have signed it.

**3. Incorrect Answers:**
- **A. Encrypt, then hash the logs:** Encryption provides confidentiality (privacy), not nonrepudiation. 
- **C. Digitally sign the log file, then encrypt it:** Renee only needs nonrepudiation. Encrypting it adds an unnecessary layer of confidentiality that wasn't requested. Option B is the better answer because it describes the actual mechanical steps of the signing process.
- **D. Hash, then encrypt the logs:** Hashing provides integrity, and general encryption provides confidentiality. Neither provides nonrepudiation unless the encryption is specifically done on a hash using a private key (which is what a digital signature is).

**4. Study Tips:**
- **Keyword Association:** Whenever you see "Nonrepudiation", immediately look for "Digital Signatures" or "Private Keys". 
- **The Formula:** Digital Signature = Hash the data + Encrypt the hash with a Private Key.

--------------------------------------------------------------------------------

### Question:
38. Isaac wants to deploy sensors to detect intruders in a facility, but he is concerned about the sensors being overly sensitive. What type of sensor is best suited to detecting intruders in an open office environment without significant expense or issues with sensitivity?
A. Infrared
B. Pressure
C. Microwave
D. Ultrasonic

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (specifically relating to Physical Security Controls and Sensors).

**2. The Answer and Explanation:**
**A. Infrared**
Infrared (specifically Passive Infrared or PIR) sensors detect changes in thermal radiation (body heat) moving across their field of view. They are very common, inexpensive, and generally less prone to false alarms from things like air currents or small, non-heat-producing movements. This makes them the best choice for an open office environment where cost and over-sensitivity are concerns.

**3. Incorrect Answers:**
- **B. Pressure:** Pressure sensors (like mats placed under carpets) are expensive to deploy across a large open office environment and are difficult to hide effectively over a large area.
- **C. Microwave:** Microwave sensors emit microwave pulses and measure their reflection. They can penetrate walls and are highly sensitive, which can lead to false alarms from movement *outside* the intended area (e.g., people walking in a hallway outside the office).
- **D. Ultrasonic:** Ultrasonic sensors emit high-frequency sound waves and measure the reflection. They are highly sensitive to air movement (like HVAC systems turning on or off) and can easily cause false alarms in a typical office environment.

**4. Study Tips:**
- **Infrared (PIR) = Body Heat**. They are cheap, reliable, and ignore the wind/AC.
- **Ultrasonic = Sound Waves**. Highly sensitive to air movement (HVAC).
- **Microwave = Penetrates Walls**. Too sensitive for open offices next to busy hallways.

--------------------------------------------------------------------------------

**Question:** Which of the answers listed below refers to a Zero Trust Control Plane security approach that takes into account user identity, device security, network conditions, and other contextual information to enable dynamic access decisions?
- Implicit trust
- Monitoring and logging
- Adaptive identity
- Microsegmentation

**1. Domain and Objective Category:**
Domain 3: Security Architecture (Objective 3.1: Compare and contrast security architecture models)

**2. The Answer and Explanation:**
The correct answer is **Adaptive identity**.
Adaptive identity leverages real-time contextual information (like user behavior, location, device health, and network conditions) to continuously assess risk and dynamically adjust access privileges. This is a foundational concept in the Zero Trust Control Plane, ensuring that trust is never implicit and is always evaluated based on the current context.

**3. Incorrect Answers:**
- **Implicit trust:** This is the traditional perimeter-based security model (trusting everything inside the network) that Zero Trust actively seeks to eliminate.
- **Monitoring and logging:** While crucial for visibility and auditing in a Zero Trust environment, these are reactive and operational capabilities, not the mechanism that makes dynamic access control decisions.
- **Microsegmentation:** This is an implementation technique used in the Zero Trust *Data Plane* to divide networks into smaller, isolated zones to prevent lateral movement. It does not refer to the identity or context-based decision-making aspect.

**4. Study Tips:**
Remember that "adaptive" means adjusting on the fly. Whenever you see a question about evaluating "context," "device security," or "network conditions" to make "dynamic decisions," think of **Adaptive identity**. Microsegmentation is for "stopping lateral movement" by chopping up the network.

--------------------------------------------------------------------------------

**Question:** What are the key components of the Zero Trust Control Plane's Policy Decision Point (PDP)? (Select 2 answers)
- Policy Engine (PE)
- Monitoring and logging
- Policy Enforcement Point (PEP)
- Microsegmentation
- Policy Administrator (PA)

**1. Domain and Objective Category:**
Domain 3: Security Architecture (Objective 3.1: Compare and contrast security architecture models)

**2. The Answer and Explanation:**
The correct answers are **Policy Engine (PE)** and **Policy Administrator (PA)**.
According to the NIST Zero Trust Architecture (NIST SP 800-207), the Control Plane contains the Policy Decision Point (PDP). The PDP is logically composed of two key components:
- **Policy Engine (PE):** This is the ultimate decision-maker. It analyzes enterprise policy, user identity, device health, and other context to decide whether to grant access.
- **Policy Administrator (PA):** This component is responsible for executing the decision made by the Policy Engine. It generates any necessary authentication tokens or credentials and communicates with the Policy Enforcement Point (PEP) to allow or deny the session.

**3. Incorrect Answers:**
- **Policy Enforcement Point (PEP):** This is part of the Zero Trust *Data Plane*, not the Control Plane's PDP. The PEP acts as the "bouncer," enforcing the access decisions made by the PDP.
- **Monitoring and logging:** While data from monitoring feeds into the Policy Engine to help it make decisions, logging itself is an operational capability, not a structural component of the PDP.
- **Microsegmentation:** This is a network security technique used in the Data Plane to divide networks into smaller zones to stop lateral movement; it is not a component of the Control Plane.

**4. Study Tips:**
Think of the PDP (Policy Decision Point) as the "brains" of Zero Trust. It consists of the **Engine** (which thinks and decides) and the **Administrator** (which gives the order). The PEP (Policy Enforcement Point) is the "muscle" or "bouncer" in the Data Plane that physically blocks or allows traffic based on those orders.

--------------------------------------------------------------------------------

**Question:** A process used by organizations to assess and evaluate the potential impact of disruptive incidents or disasters on their critical business functions and operations is referred to as:
- BPA
- BIA
- SLE
- BCP

**1. Domain and Objective Category:**
Domain 5: Security Program Management and Oversight (Objective 5.2: Explain elements of the risk management process)

**2. The Answer and Explanation:**
The correct answer is **BIA** (Business Impact Analysis).
A Business Impact Analysis (BIA) is a systematic process used to determine and evaluate the potential effects of an interruption to critical business operations as a result of a disaster, accident, or emergency. It helps an organization identify its most crucial systems and functions, and quantifies the impact if they were to go down.

**3. Incorrect Answers:**
- **BPA (Business Partnership Agreement):** A legal agreement between partners detailing the relationship and their contributions, not a process for assessing the impact of disasters.
- **SLE (Single Loss Expectancy):** A monetary value that represents how much money an organization expects to lose in a single occurrence of a specific risk. It is a metric used in risk assessment, not the holistic process of evaluating business functions.
- **BCP (Business Continuity Plan):** This is the actual comprehensive plan that contains the instructions and procedures on how to keep the business running during a disaster. The BCP is created *using* the results of the BIA, but it isn't the assessment process itself.

**4. Study Tips:**
Think of the **BIA** as the "Analysis" where you figure out what hurts the most if it goes down (finding the critical pieces). Think of the **BCP** as the "Plan" or "Playbook" on how you actually survive the disaster. (BIA = the diagnosis, BCP = the treatment plan).

--------------------------------------------------------------------------------

**Question:** A hierarchical system for the creation, management, storage, distribution, and revocation of digital certificates is known as:
- PKI
- RA
- PKCS
- CA

**1. Domain and Objective Category:**
Domain 3: Security Architecture (Public Key Infrastructure concepts)

**2. The Answer and Explanation:**
The correct answer is **PKI** (Public Key Infrastructure).
PKI is the comprehensive hierarchical system (including the hardware, software, policies, roles, and procedures) used for the creation, management, storage, distribution, and revocation of digital certificates and public-key encryption. 

**3. Incorrect Answers:**
- **CA (Certificate Authority):** This is a specific server or entity *within* the PKI that actually issues and manages the digital certificates. The CA is a component of the system, not the entire system itself.
- **RA (Registration Authority):** This is another component *within* the PKI. Its job is to verify the identity of the user requesting a certificate before the CA is allowed to issue it.
- **PKCS (Public Key Cryptography Standards):** These are a set of widely accepted standards (devised originally by RSA Security) that define how public key cryptography should be implemented. They are standards, not a management system.

**4. Study Tips:**
When you see words like "entire system", "framework", or "infrastructure" regarding digital certificates, think of **PKI** (Infrastructure). If the question asks for the "entity that issues or signs" the certificate, the answer is **CA** (Authority).

--------------------------------------------------------------------------------

**Question:** Key escrow is a cryptographic technique that enables storing copies of encryption keys with a trusted third party. A Recovery Agent (RA) is a trusted third party (an individual, entity, or system) who is authorized to assist in the retrieval of encryption keys and data on behalf of the data owner. Key escrow and RA are both used to ensure that encrypted data can be decrypted even if the data owner loses access to their encryption key. Since key escrow and RAs are both components of a single security solution, the only way to implement key escrow systems is with the use of RAs.
- True
- False

**1. Domain and Objective Category:**
Domain 3: Security Architecture (Public Key Infrastructure concepts)

**2. The Answer and Explanation:**
The correct answer is **False**.
While both Key Escrow and Recovery Agents (RAs) provide a way to recover encrypted data, they are distinct concepts and mechanisms. Key Escrow involves securely storing a direct copy of the user's private encryption key with a trusted third party. A Recovery Agent (often called a Data Recovery Agent, or DRA), on the other hand, is an authorized entity that typically possesses a separate, special "master" certificate/key that is mathematically authorized to decrypt the users' files directly. You can implement Key Escrow without a Recovery Agent, and you can implement a Recovery Agent without Key Escrow.

**3. Incorrect Answers:**
- **True:** This is incorrect because Key Escrow and Recovery Agents are independent mechanisms. They are not intrinsically bound together as a single solution, and one does not require the use of the other.

**4. Study Tips:**
To keep them straight, use this analogy: 
- **Key Escrow** is like giving a physical spare copy of your house key to a trusted neighbor to lock in their safe. 
- A **Recovery Agent (RA)** is like the apartment building manager who has their own universal "master key" that can open your door if you get locked out.
They solve the same problem, but they do it in completely different ways.

--------------------------------------------------------------------------------

**Question:** Which of the answers listed below refers to software technology designed to provide confidentiality for an entire data storage device?
- TPM
- FDE
- EFS
- HSM

**1. Domain and Objective Category:**
Domain 3: Security Architecture (Data Protection and Cryptography concepts)

**2. The Answer and Explanation:**
The correct answer is **FDE** (Full Disk Encryption).
FDE is a technology that encrypts every single bit of data on a storage device (such as a hard drive, SSD, or USB drive). By encrypting the entire drive, it provides complete confidentiality for all data at rest on that device, ensuring that if the device is lost or stolen, the data cannot be read without the correct authentication.

**3. Incorrect Answers:**
- **TPM (Trusted Platform Module):** A dedicated hardware chip found on most modern motherboards that securely stores cryptographic keys (and is often used *by* FDE software like BitLocker). However, the TPM itself is the hardware key-storage, not the encryption technology that encrypts the entire device.
- **EFS (Encrypting File System):** A feature of the Windows operating system that provides *file-level* or *folder-level* encryption. It only encrypts specific files you choose, rather than the *entire* storage device.
- **HSM (Hardware Security Module):** A physical, external computing device or server appliance that safeguards and manages digital keys and provides heavy-duty cryptoprocessing. It is enterprise hardware, not the technology that encrypts a local storage device.

**4. Study Tips:**
If a question asks about encrypting an *entire* drive or device, the answer is **FDE** (Full Disk Encryption). If it asks about encrypting specific *files* or *folders*, the answer is **EFS** (Encrypting File System). Think of TPM and HSM as the physical hardware "safes" where the encryption keys are securely kept.

--------------------------------------------------------------------------------

**Question:** Which of the following software application tools are specifically designed for implementing encryption algorithms to secure data communication and storage? (Select 2 answers)
- VPN
- GPG
- SSH
- IPsec
- PGP

**1. Domain and Objective Category:**
Domain 3: Security Architecture (Cryptographic tools and implementations)

**2. The Answer and Explanation:**
The correct answers are **GPG** and **PGP**.
PGP (Pretty Good Privacy) is a software application used for encrypting, decrypting, and digitally signing files, emails, and data storage. GPG (GNU Privacy Guard) is a free, open-source software application that is a complete replacement for PGP. Both are specific software tools designed precisely for implementing encryption for secure communication (like email) and secure storage (encrypting files at rest).

**3. Incorrect Answers:**
- **VPN (Virtual Private Network):** This is a network technology used to create a secure, encrypted tunnel over an unsecured network (like the internet). It secures data in transit, but it is not a software tool used for securing data storage.
- **SSH (Secure Shell):** This is a cryptographic network protocol used primarily for secure remote administration and file transfers. It secures data in transit, not data at rest (storage).
- **IPsec:** This is a protocol suite used to encrypt and authenticate IP packets at the network layer. Like VPNs (which often use IPsec), it secures data in transit, not data in storage.

**4. Study Tips:**
When you see a question asking for tools that secure BOTH communication (transit) AND storage (at rest), think of **PGP** and **GPG** (used heavily for files and emails). Network protocols like VPN, SSH, and IPsec are only used for protecting data *in transit*.

--------------------------------------------------------------------------------

**Question:** What is the name of a network protocol that secures web traffic via SSL/TLS encryption?
- SFTP
- HTTPS
- FTPS
- SNMP

**1. Domain and Objective Category:**
Domain 2: Architecture and Design (Secure Protocols)

**2. The Answer and Explanation:**
The correct answer is **HTTPS** (Hypertext Transfer Protocol Secure).
HTTPS is the standard protocol used to secure web traffic on the Internet. It protects the communication between a user's web browser and a website by encrypting the data using SSL (Secure Sockets Layer) or its modern successor, TLS (Transport Layer Security).

**3. Incorrect Answers:**
- **SFTP (SSH File Transfer Protocol):** While it is a secure protocol, it secures file transfers using SSH (Secure Shell), not SSL/TLS, and it is not used for web traffic.
- **FTPS (File Transfer Protocol Secure):** This protocol does use SSL/TLS encryption, but it is specifically used for file transfers, not general web traffic.
- **SNMP (Simple Network Management Protocol):** This is a protocol used for managing and monitoring network devices (like routers and switches). While SNMPv3 can be encrypted, it is not used for securing web traffic.

**4. Study Tips:**
Whenever you see the phrase "web traffic", immediately look for HTTP or HTTPS. If it specifically asks for "secure web traffic" or mentions "SSL/TLS", the answer is **HTTPS**. 
*Bonus tip:* To keep the secure file protocols straight: FTPS uses SSL/TLS. SFTP uses SSH.

--------------------------------------------------------------------------------

**Question:** Which of the answers listed below refers to a deprecated TLS-based method for secure transmission of email messages?
- S/MIME
- STARTTLS
- DKIM
- SMTPS

**1. Domain and Objective Category:**
Domain 2: Architecture and Design (Secure Email Protocols)

**2. The Answer and Explanation:**
The correct answer is **SMTPS** (Simple Mail Transfer Protocol Secure).
SMTPS was an early method for securing SMTP traffic using SSL/TLS encryption right from the start of the connection (known as implicit TLS, typically on port 465). It is now considered deprecated by the IETF (Internet Engineering Task Force) in favor of STARTTLS, though some legacy systems still use it.

**3. Incorrect Answers:**
- **STARTTLS:** This is the *current, modern* standard. Instead of requiring a separate, dedicated secure port like SMTPS, STARTTLS takes an existing insecure email connection on a standard port (like port 587) and explicitly upgrades it to a secure TLS connection.
- **S/MIME (Secure/Multipurpose Internet Mail Extensions):** This is a standard used to encrypt and digitally sign the actual email *content and attachments*, not a network protocol for the transmission of the email over the wire.
- **DKIM (DomainKeys Identified Mail):** This is an email authentication method that uses cryptographic signatures to verify the sender's domain and detect forged sender addresses (spoofing). It is not a TLS-based transmission method.

**4. Study Tips:**
If an email protocol ends in an "S" (like SMTPS), it usually refers to older "implicit" SSL/TLS connections on a dedicated port, which are mostly deprecated. **STARTTLS** is the modern way: it *starts* insecure on a normal port and explicitly upgrades the connection to TLS. 
- SMTPS = Deprecated
- STARTTLS = Modern

--------------------------------------------------------------------------------

**Question:** Which of the following answers refers to an obsolete protocol used for secure data transfer over the web?
- SMTPS
- SRTP
- SHTTP
- S/MIME

**1. Domain and Objective Category:**
Domain 2: Architecture and Design (Secure Protocols)

**2. The Answer and Explanation:**
The correct answer is **SHTTP** (Secure Hypertext Transfer Protocol).
SHTTP was an early protocol developed in the 1990s for secure data transfer over the web, competing directly with SSL (which later evolved into TLS and HTTPS). While HTTPS encrypts the entire communication session, SHTTP encrypted individual messages. SHTTP ultimately lost the standards battle to HTTPS and is now entirely obsolete.

**3. Incorrect Answers:**
- **SMTPS (Simple Mail Transfer Protocol Secure):** This is a deprecated protocol for securing *email* transmission, not for general data transfer over the web.
- **SRTP (Secure Real-Time Transport Protocol):** This is an active, modern protocol used for securing voice and video traffic (like VoIP and video calls), not general web traffic. It is not obsolete.
- **S/MIME (Secure/Multipurpose Internet Mail Extensions):** This is a standard used to encrypt and digitally sign *email contents*. It is used for email, not web data transfer, and is still widely used today.

**4. Study Tips:**
Don't confuse **SHTTP** (Secure HTTP, which is obsolete) with **HTTPS** (HTTP Secure, which is the modern standard). Notice the position of the 'S'. If the 'S' is at the front (SHTTP), it's the old, dead one. If the 'S' is at the end (HTTPS), it's the modern, alive one!

--------------------------------------------------------------------------------

### Question:
Which part of IPsec provides authentication, integrity, and confidentiality?
- SPD
- PFS
- AH
- ESP

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Secure Protocols / IPsec)

**2. The Answer and Explanation:**
**ESP (Encapsulating Security Payload)**
ESP is the protocol within the IPsec suite that provides **confidentiality** (encryption) for the data payload, in addition to optional authentication and data integrity. Because it encrypts the actual data being sent across the network, it is the component that keeps the contents secret from eavesdroppers.

**3. Incorrect Answers:**
- **AH (Authentication Header):** A protocol within the IPsec suite that provides strong authentication and data integrity, but it does *not* provide confidentiality (meaning, it does not encrypt the data payload).
- **SPD (Security Policy Database):** A configuration database used by an IPsec endpoint to determine what rules to apply to traffic (e.g., whether to encrypt it, bypass it, or drop it). It is a configuration component, not the protocol providing the cryptographic security.
- **PFS (Perfect Forward Secrecy):** A cryptographic property where temporary session keys are used to protect past sessions from future compromises. It is not a structural component or protocol within the IPsec suite itself.

**4. Study Tips:**
When dealing with IPsec on the exam, remember these two primary protocols:
- **ESP** = **E**ncryption (Confidentiality).
- **AH** = **A**uthentication only (No Encryption).
If the question specifically asks what provides *confidentiality/encryption*, the answer must be **ESP**.

--------------------------------------------------------------------------------

### Question:
Which cryptographic solution would be best suited for low-power devices, such as IoT devices, embedded systems, and mobile devices?
- ECC
- DES
- RSA
- AES

**1. Domain and Objective Category:**
Domain 1.0: General Security Concepts (Objective 1.2: Cryptography / Public-Key Algorithms)

**2. The Answer and Explanation:**
**ECC (Elliptic-Curve Cryptography)**
ECC is an asymmetric (public-key) encryption algorithm that provides the exact same level of cryptographic security as older algorithms (like RSA), but uses significantly smaller key sizes to do so. Because the keys are much smaller, ECC requires far less computational processing power, memory, and battery life. This makes it the absolute ideal choice for low-power devices like smartphones, IoT (Internet of Things) devices, and smart cards.

**3. Incorrect Answers:**
- **RSA:** While RSA is a highly secure asymmetric algorithm, it requires massive key sizes (e.g., 2048 or 4096-bit) to remain secure. Processing these massive keys heavily drains battery and processing power, making it poorly suited for small IoT devices.
- **AES (Advanced Encryption Standard):** While AES is highly efficient and frequently used on mobile devices as a *symmetric* cipher, the exam specifically tests ECC as the correct answer when looking for the most efficient *asymmetric* cryptosystem tailored for low-power environments.
- **DES (Data Encryption Standard):** An old, deprecated, and highly insecure symmetric block cipher. It should not be used on any modern device.

**4. Study Tips:**
Whenever you see the keywords **"low-power devices"**, **"IoT"**, **"smart cards"**, or **"mobile devices"** paired with a cryptography question on the exam, immediately look for **ECC (Elliptic-Curve Cryptography)**.

--------------------------------------------------------------------------------

### Question:
Which of the following answers refers to a public-key cryptosystem used for digital signatures, secure key exchange, and encryption?
- ECC
- RSA
- PKI
- DSA

**1. Domain and Objective Category:**
Domain 1.0: General Security Concepts (Objective 1.2: Cryptography / Public-Key Algorithms)

**2. The Answer and Explanation:**
**RSA (Rivest-Shamir-Adleman)**
RSA is one of the oldest and most widely used asymmetric (public-key) cryptosystems. It is a highly versatile algorithm because its underlying mathematical structure (based on the difficulty of factoring incredibly large prime numbers) allows it to natively perform all three major functions: it can be used to **encrypt data**, **exchange keys** securely, and generate **digital signatures**.

**3. Incorrect Answers:**
- **DSA (Digital Signature Algorithm):** As the name strictly implies, DSA is designed and used *only* for creating digital signatures. It cannot be used for general data encryption or key exchange.
- **ECC (Elliptic-Curve Cryptography):** While ECC is a powerful category of public-key cryptography (often used for key exchange via ECDHE and signatures via ECDSA), standard textbook definitions usually point to RSA as the classic, all-in-one algorithm that historically handled all three capabilities directly in its base form.
- **PKI (Public Key Infrastructure):** This is not a cryptosystem or algorithm itself. Rather, it is the entire overarching framework (the servers, Certificate Authorities, policies, and software) used to manage, create, store, and distribute digital certificates and public keys.

**4. Study Tips:**
- **RSA** = The "all-rounder." It does Encryption, Key Exchange, AND Digital Signatures.
- **DSA** = Digital Signatures **ONLY**.
- **PKI** = The *management system/infrastructure* for keys, not the math algorithm itself.

--------------------------------------------------------------------------------

### Question:
Which of the answers listed below refers to a solution designed to strengthen the security of session keys?
- ECB
- PFS
- EFS
- PFX

**1. Domain and Objective Category:**
Domain 1.0: General Security Concepts (Objective 1.2: Cryptography / Session Keys)

**2. The Answer and Explanation:**
**PFS (Perfect Forward Secrecy)**
PFS is a cryptographic property designed to strengthen the security of session keys by ensuring that a new, random session key is generated for every single session. Because these session keys are temporary (ephemeral) and are not mathematically derived from a long-term private key, a compromise of the server's long-term private key in the future will not allow an attacker to decrypt any past recorded sessions.

**3. Incorrect Answers:**
- **ECB (Electronic Codebook):** A very basic, legacy, and highly insecure mode of operation for block ciphers. It is known for leaving visible patterns in encrypted data and is definitely not a solution for strengthening session keys.
- **EFS (Encrypting File System):** A feature built directly into the Microsoft Windows operating system used for encrypting individual files or folders on a hard drive. It is a file-level encryption tool, not a session key security feature.
- **PFX (Personal Information Exchange):** A file format (also known as PKCS #12) used to securely store and transfer cryptographic objects, like certificates and private keys, in a single password-protected file. It is a file format, not a cryptographic property.

**4. Study Tips:**
- When you see **"strengthen the security of session keys"** or **"protecting past communications"**, immediately think of **PFS (Perfect Forward Secrecy)**.
- PFS is achieved by using **Ephemeral** keys (like DHE or ECDHE)!

--------------------------------------------------------------------------------

### Question:
Which of the following answers refers to a protocol used to set up secure connections and exchange of cryptographic keys in IPsec VPNs?
- SSL
- IKE
- ESP
- DHE

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Secure Protocols / IPsec)

**2. The Answer and Explanation:**
**IKE (Internet Key Exchange)**
IKE is the protocol used within the IPsec suite to set up a secure, authenticated communications channel (known as a Security Association, or SA) between two parties. It is responsible for the initial negotiation and exchange of cryptographic keys required to establish the IPsec VPN tunnel.

**3. Incorrect Answers:**
- **SSL (Secure Sockets Layer):** An older, deprecated protocol used to secure web traffic over the Internet. It is not used to set up IPsec VPNs.
- **ESP (Encapsulating Security Payload):** A core protocol within the IPsec suite, but its job is to provide the actual encryption and confidentiality of the data payload being transmitted, *after* the connection is established. It does not handle the initial setup and key exchange.
- **DHE (Diffie-Hellman Ephemeral):** A cryptographic algorithm used to generate temporary session keys. While IKE uses Diffie-Hellman mathematics behind the scenes to securely trade keys, DHE itself is just the math algorithm, not the overarching protocol (IKE) that manages the IPsec VPN setup.

**4. Study Tips:**
- **IKE = Internet Key Exchange.** If a question mentions exchanging keys specifically for **IPsec**, the answer is almost always **IKE**.
- Think of **IKE** as the handshake that agrees on the rules, and **ESP** as the armored truck that actually carries the encrypted data based on those rules.

--------------------------------------------------------------------------------

### Question:
Which of the answers listed below refers to a key exchange protocol that generates temporary keys for each session, providing forward secrecy to protect past and future communications?
- PFS
- SHA
- PGP
- DHE

**1. Domain and Objective Category:**
Domain 1.0: General Security Concepts (Objective 1.2: Cryptography / Key Exchange)

**2. The Answer and Explanation:**
**DHE (Diffie-Hellman Ephemeral)**
DHE is a key exchange protocol that creates a temporary, short-lived (ephemeral) key for each session. Because a brand new, unique key is used for every single session, it provides Perfect Forward Secrecy (PFS). This means that if an attacker records your encrypted traffic today and manages to compromise your server's long-term private key next year, they *still* cannot decrypt the recorded traffic because the temporary session keys were thrown away.

**3. Incorrect Answers:**
- **PFS (Perfect Forward Secrecy):** This is the tricky distractor! PFS is a cryptographic *property* or *feature* provided by certain protocols (like DHE). However, PFS is not the name of the key exchange protocol itself.
- **SHA (Secure Hash Algorithm):** A family of cryptographic hashing algorithms used for data integrity (creating digital fingerprints), not for key exchange.
- **PGP (Pretty Good Privacy):** A data encryption and decryption software/protocol used primarily for securing files and email. It is not an ephemeral session key exchange protocol.

**4. Study Tips:**
- The **"E"** in DHE and ECDHE stands for **"Ephemeral"**, which means "temporary" or "short-lived."
- **Ephemeral keys** are the magic ingredient that provides **Perfect Forward Secrecy (PFS)**!

--------------------------------------------------------------------------------

### Question:
Which of the answers listed below refers to a shared secret authentication method used in WPA, WPA2, and EAP?
- PSK
- 802.1X
- SAE
- TKIP

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Wireless Security Settings / Authentication Methods)

**2. The Answer and Explanation:**
**PSK (Pre-Shared Key)**
A Pre-Shared Key (PSK) is a shared secret (a password or passphrase) that is previously shared between the two communicating parties using some secure channel before it needs to be used. In WPA and WPA2 "Personal" modes, this is the standard Wi-Fi password that everyone types in to connect to the network.

**3. Incorrect Answers:**
- **802.1X:** An IEEE standard for port-based network access control (PNAC). It provides an authentication mechanism to devices wishing to attach to a LAN or WLAN. It is used in WPA "Enterprise" mode and relies on a central authentication server (like RADIUS), rather than a single shared secret password for everyone.
- **SAE (Simultaneous Authentication of Equals):** A highly secure key exchange protocol used in WPA3. It replaces the older PSK method to provide much stronger protection against offline dictionary attacks.
- **TKIP (Temporal Key Integrity Protocol):** This is an older *encryption* protocol used primarily with the original WPA standard. It encrypts the traffic, but it is not the *authentication* method itself.

**4. Study Tips:**
- **PSK (Pre-Shared Key):** Think of this as your normal home Wi-Fi password. Everyone "shares" the same "key" before they can connect.
- **802.1X (Enterprise):** Think of this as corporate Wi-Fi. You don't use a shared password; you log in using your own unique username and password that gets verified by a central server.
- **SAE:** The new, better version of PSK used in WPA3.

--------------------------------------------------------------------------------

### Question:
The term "KEK" refers to a type of cryptographic key often used in key management systems to add an additional layer of security when encrypting and decrypting other cryptographic keys.
- True
- False

**1. Domain and Objective Category:**
Domain 1.0: General Security Concepts (Objective 1.2: Cryptography / Key Management)

**2. The Answer and Explanation:**
**True**
KEK stands for **Key Encryption Key**. In cryptography and key management systems, it is extremely dangerous to leave your standard data keys lying around in plaintext. Therefore, a KEK is a specialized key whose sole purpose is to encrypt and decrypt *other* cryptographic keys (typically called DEKs, or Data Encryption Keys) to protect them while they are stored or being transmitted.

**3. Incorrect Answers:**
- **False:** The statement is completely accurate in describing the purpose of a Key Encryption Key.

**4. Study Tips:**
Think of a **KEK (Key Encryption Key)** as the heavily guarded "master key" for a security guard's lockbox. You use the master KEK to unlock the box, which then gives you access to all the smaller **DEKs (Data Encryption Keys)** that are used to actually unlock the individual doors/data.

--------------------------------------------------------------------------------

### Question:
Which of the algorithms listed below are not symmetric ciphers? (Select 3 answers)
- AES
- DES
- DHE
- ECC
- IDEA
- RC4
- RSA

**1. Domain and Objective Category:**
Domain 1.0: General Security Concepts (Objective 1.2: Cryptography / Symmetric vs. Asymmetric)

**2. The Answer and Explanation:**
**DHE, ECC, RSA**
These three algorithms are NOT symmetric ciphers; they are **asymmetric (public-key)** algorithms or key-exchange protocols:
- **DHE (Diffie-Hellman Ephemeral):** A cryptographic protocol that allows two parties to securely establish a shared secret key over an insecure network without ever sending the actual key.
- **ECC (Elliptic-Curve Cryptography):** A highly efficient asymmetric (public-key) encryption algorithm that uses the algebraic structure of elliptic curves to provide strong security with very small key sizes.
- **RSA (Rivest-Shamir-Adleman):** The most common asymmetric (public-key) algorithm used globally for secure data transmission and digital signatures. It relies on the mathematical difficulty of factoring large prime numbers.

**3. Incorrect Answers:**
The remaining choices are all **symmetric** ciphers (they use a single shared key for both encryption and decryption):
- **AES (Advanced Encryption Standard):** The current gold standard for symmetric encryption worldwide.
- **DES (Data Encryption Standard):** An old, deprecated symmetric block cipher.
- **IDEA (International Data Encryption Algorithm):** A symmetric block cipher developed in the 90s as a replacement for DES.
- **RC4 (Rivest Cipher 4):** An old, deprecated symmetric stream cipher.

**4. Study Tips:**
For the exam, it is much easier to just memorize the **asymmetric** algorithms because there are fewer of them. 
If it is **RSA**, **ECC**, **DSA**, or anything related to **Diffie-Hellman (DH, DHE, ECDHE)**, it is **Asymmetric**. 
Almost everything else (AES, DES, 3DES, RC4, Twofish, Blowfish, IDEA) is Symmetric!

--------------------------------------------------------------------------------

### Question:
Which of the following answers refer(s) to deprecated/insecure encryption protocols and cryptographic hash functions? (Select all that apply)
- DES
- AES-256
- MD5
- ECC
- SHA-1
- SSL
- RC4

**1. Domain and Objective Category:**
Domain 1.0: General Security Concepts (Objective 1.2: Cryptography)

**2. The Answer and Explanation:**
**DES, MD5, SHA-1, SSL, RC4**
These five algorithms and protocols are considered deprecated (obsolete) and insecure:
- **DES (Data Encryption Standard):** An old symmetric encryption algorithm that uses a tiny 56-bit key, which can easily be cracked via brute force by modern computers in minutes.
- **MD5 (Message Digest 5):** An old hashing algorithm that suffers from severe collision vulnerabilities (hackers can create two different files that produce the exact same hash).
- **SHA-1 (Secure Hash Algorithm 1):** An older hashing algorithm that is also deprecated due to collision vulnerabilities, much like MD5.
- **SSL (Secure Sockets Layer):** An obsolete cryptographic protocol for web traffic that suffers from numerous flaws (like the POODLE vulnerability). It has been completely replaced by TLS.
- **RC4 (Rivest Cipher 4):** A stream cipher that was heavily used in old protocols like WEP, but is now deprecated due to multiple severe cryptographic vulnerabilities.

**3. Incorrect Answers:**
- **AES-256 (Advanced Encryption Standard):** This is the current, modern, gold-standard symmetric encryption algorithm. It is highly secure and widely used around the world.
- **ECC (Elliptic-Curve Cryptography):** A modern, highly secure and efficient form of public-key (asymmetric) cryptography. It provides incredibly strong security with very small key sizes, making it perfect for mobile devices.

**4. Study Tips:**
For the exam, immediately flag these terms as "BAD" or "INSECURE":
- Hashes: **MD5, SHA-1**
- Encryption: **DES, 3DES, RC4**
- Web/Wireless Protocols: **SSL, WEP, TKIP**

--------------------------------------------------------------------------------

### Question:
An encryption protocol primarily used in Wi-Fi networks implementing the WPA2 security standard is called:
- TKIP
- CCMP
- SSL
- IPsec

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Wireless Security Settings / Secure Protocols)

**2. The Answer and Explanation:**
**CCMP (Counter Mode with Cipher Block Chaining Message Authentication Code Protocol)**
CCMP is the standard encryption protocol used in the WPA2 (Wi-Fi Protected Access 2) security standard. It utilizes the highly secure AES (Advanced Encryption Standard) cipher to provide strong data confidentiality, authentication, and access control for wireless networks, replacing the older and much weaker TKIP protocol.

**3. Incorrect Answers:**
- **TKIP (Temporal Key Integrity Protocol):** The older encryption protocol used primarily with the original WPA (not WPA2) security standard. It was a stopgap measure designed to replace the highly vulnerable WEP protocol on old hardware, but TKIP itself is now considered deprecated and insecure.
- **SSL (Secure Sockets Layer):** An obsolete cryptographic protocol designed for secure web traffic over the Internet (replaced by TLS), not for encrypting local Wi-Fi airwaves.
- **IPsec (Internet Protocol Security):** A suite of protocols used to secure IP communications (like VPNs) over a network, not the layer 2 protocol used to encrypt local Wi-Fi signals in WPA2.

**4. Study Tips:**
Memorize these Wi-Fi security pairings for the exam:
- **WPA** uses **TKIP** (Old and insecure).
- **WPA2** uses **CCMP** and **AES** (Strong standard).
- **WPA3** uses **SAE** (Simultaneous Authentication of Equals).

--------------------------------------------------------------------------------

### Question:
Which protocol enables secure, real-time delivery of audio and video over an IP network?
- S/MIME
- RTP
- SIP
- SRTP

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Secure Protocols)

**2. The Answer and Explanation:**
**SRTP (Secure Real-Time Transport Protocol)**
SRTP is an extension of the RTP (Real-Time Transport Protocol) that adds security features such as encryption, message authentication, and integrity. It is specifically designed to ensure that real-time audio and video communications (such as VoIP calls or video conferencing) are secure and protected against interception and tampering.

**3. Incorrect Answers:**
- **S/MIME (Secure/Multipurpose Internet Mail Extensions):** A protocol used for encrypting and digitally signing email messages, not for securing real-time audio or video streams.
- **RTP (Real-Time Transport Protocol):** The standard protocol for delivering audio and video over IP networks, but it does *not* natively include security features (it transmits unencrypted data). 
- **SIP (Session Initiation Protocol):** A signaling protocol used to initiate, maintain, and terminate real-time sessions (like VoIP calls). While essential for setting up the call, SIP only handles the call setup and signaling, not the secure delivery of the actual audio/video media stream itself.

**4. Study Tips:**
When you see a question about the **"real-time delivery of audio and video"**, think **RTP**.
When the question asks for the **"secure"** version of that delivery, simply add an 'S' to the front: **Secure + RTP = SRTP**.

--------------------------------------------------------------------------------

### Question:
A system that uses public network (such as the Internet) as a means for creating private encrypted connections between remote locations is referred to as:
- WWAN
- VPN
- PAN
- VLAN

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Architecture Models / Secure Protocols)

**2. The Answer and Explanation:**
**VPN (Virtual Private Network)**
A Virtual Private Network (VPN) uses a public network (like the Internet) to create a secure, private, encrypted "tunnel" between remote locations or between a remote user and a corporate network. This effectively extends a private corporate network across a public one, ensuring that intercepted traffic cannot be easily read.

**3. Incorrect Answers:**
- **WWAN (Wireless Wide Area Network):** A wireless network that covers a large geographic area (such as mobile/cellular networks like 4G or 5G). While it provides broad connectivity, it is not inherently defined as a system for creating private encrypted connections between remote locations.
- **PAN (Personal Area Network):** A small, very short-range network used for data transmission among personal devices (for example, Bluetooth connecting a smartphone to wireless headphones).
- **VLAN (Virtual Local Area Network):** A logical grouping of devices on the same local network (LAN) to segment traffic, regardless of physical location within that LAN. It operates locally within a switch/network, not over a public internet connection to remote locations.

**4. Study Tips:**
- **VPN** = **Virtual** Private Network (it acts like a private network, but uses public wires).
- Whenever a question mentions creating an **encrypted connection/tunnel over a public network (the Internet)**, the answer is almost always a VPN.

--------------------------------------------------------------------------------

### Question:
Which of the answers listed below refers to a suite of protocols and technologies providing encryption, authentication, and data integrity for network traffic?
- TLS
- SSH
- IPsec
- VPN

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Secure Protocols)

**2. The Answer and Explanation:**
**IPsec (Internet Protocol Security)**
IPsec is not a single protocol, but rather a comprehensive **suite of protocols** used to protect data and secure IP communications at the network layer. It accomplishes this by authenticating and encrypting each IP packet of a communication session. It primarily relies on two core protocols: Authentication Header (AH) for data integrity/authentication, and Encapsulating Security Payload (ESP) for encryption/confidentiality.

**3. Incorrect Answers:**
- **TLS (Transport Layer Security):** A cryptographic protocol designed to provide communications security over a computer network (typically used to secure web browsing via HTTPS). It operates at the transport layer, and while it provides encryption, it is generally considered a single protocol rather than a broad "suite of protocols" for general network traffic like IPsec.
- **SSH (Secure Shell):** A specific protocol used primarily for secure command-line access and remote administration, not a suite of protocols for general network traffic.
- **VPN (Virtual Private Network):** A technology or concept that extends a private network across a public network. A VPN is the overarching connection type, not the protocol suite itself. (Note: VPNs very frequently *use* the IPsec protocol suite to create that secure connection).

**4. Study Tips:**
When you see the keywords **"suite of protocols"** used for securing network traffic, immediately look for **IPsec**.
Remember its two main components:
- **AH (Authentication Header)** = Authentication & Integrity.
- **ESP (Encapsulating Security Payload)** = Encryption & Confidentiality.

--------------------------------------------------------------------------------

### Question:
A type of cryptographic network protocol for secure data communication, remote command-line login, remote command execution, and other secure network services between two networked computers is known as:
- RDP
- SSH
- Telnet
- SCP

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Secure Protocols)

**2. The Answer and Explanation:**
**SSH (Secure Shell)**
SSH is a cryptographic network protocol used to secure data communication, provide remote command-line login, and execute remote commands over an unsecured network. It typically operates on port 22 and provides strong encryption and authentication, replacing older, insecure protocols.

**3. Incorrect Answers:**
- **RDP (Remote Desktop Protocol):** A proprietary protocol developed by Microsoft that provides a user with a graphical interface (GUI) to connect to another computer. It is not primarily for command-line login.
- **Telnet:** An older network protocol used for remote command-line login, but it transmits all data in cleartext (unencrypted), so it provides no security or cryptographic protections.
- **SCP (Secure Copy Protocol):** A network protocol that supports file transfers between hosts on a network. While it uses SSH for data transfer and authentication (and thus is secure), it is specifically designed for copying and transferring files, not as a general protocol for remote command-line login.

**4. Study Tips:**
- **SSH** = Secure Shell (Secure command-line access).
- **Telnet** = Telecommunications Network (Insecure, cleartext command-line access).
- **RDP** = Remote Desktop Protocol (Graphical UI access).
- **SCP** = Secure Copy Protocol (Securely copying files).

--------------------------------------------------------------------------------

### Question:
What is a honeytoken?
- A decoy file that is designed to attract attackers
- A unique identifier assigned to a honeyfile
- A decoy system that is designed to lure potential attackers
- A unique identifier that is designed to track attackers

**1. Domain and Objective Category:**
Domain 4.0: Security Operations (Deception and disruption technology)

**2. The Answer and Explanation:**
**A unique identifier that is designed to track attackers**
A honeytoken is a specific piece of fabricated data—such as a fake credit card number, a dummy database record, or a fake API key/unique identifier—that is intentionally left within a system. If this data is ever accessed, used, or moved, it acts as a digital tripwire, alerting defenders and allowing them to track the unauthorized user's actions.

**3. Incorrect Answers:**
- **A decoy file that is designed to attract attackers:** This describes a **honeyfile**, which is an entire file (like a word document) used as a decoy, not just a specific piece of data or token.
- **A unique identifier assigned to a honeyfile:** Honeytokens are their own standalone pieces of decoy data; they are not inherently just ID numbers attached to honeyfiles.
- **A decoy system that is designed to lure potential attackers:** This describes a **honeypot**, which is an entire system or server designed as a decoy, not a single token of data.

**4. Study Tips:**
Match the terms to their scale:
- **Honeypot** = A whole fake *system/server*.
- **Honeyfile** = A whole fake *file*.
- **Honeytoken** = A small piece of fake *data* (like a token or identifier).

--------------------------------------------------------------------------------

### Question:
A honeyfile can be any type of file (e.g., a document, email message, image, or video file) containing real user data intentionally placed within a network or system to attract potential attackers or unauthorized users.
- True
- False

**1. Domain and Objective Category:**
Domain 4.0: Security Operations (Deception and disruption technology)

**2. The Answer and Explanation:**
**False**
While a honeyfile is indeed an intentionally placed file meant to attract and detect attackers, it must **never contain real user data**. A honeyfile contains fake, fabricated, or decoy data (such as fake passwords, fake financial records, or fake PII). Placing real, sensitive user data in a decoy file would put actual data at risk and cause a severe security and privacy violation.

**3. Incorrect Answers:**
- **True:** The statement is false purely because of the phrase "containing real user data."

**4. Study Tips:**
Honey = Fake/Decoy. Never use real data in a honeypot, honeyfile, honeynet, or honeytoken!

--------------------------------------------------------------------------------

### Question:
The term "Zero Trust security" refers to a cybersecurity model that eliminates implicit trust from networks and requires all users and devices to be continuously verified before being granted access to resources. The implementation of the Zero Trust security involves two distinct components: a Data Plane, responsible for defining and managing security policies, and a Control Plane, responsible for enforcing the security policies established by the Data Plane.
- True
- False

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Zero Trust Architecture)

**2. The Answer and Explanation:**
**False**
The definitions of the Data Plane and Control Plane are backward in the question. According to the NIST Zero Trust Architecture, the **Control Plane** is the "brains" of the operation—it is responsible for defining, managing, and deciding the security policies (Policy Decision Point). The **Data Plane** is the "muscle"—it is responsible for actually enforcing those policies and handling the network traffic (Policy Enforcement Point). 

**3. Incorrect Answers:**
- **True:** The statement is false because it swaps the roles of the Control Plane and Data Plane.

**4. Study Tips:**
Think of the Zero Trust planes like a human body:
- **Control Plane** = The Brains (Defines rules, makes decisions).
- **Data Plane** = The Muscle/Bouncer (Enforces the rules, moves the data).

--------------------------------------------------------------------------------

### Question:
What is the name of a network protocol that enables secure file transfer over SSH?
- TFTP
- SFTP
- Telnet
- FTPS

**1. Domain and Objective Category:**
Domain 3.0: Security Architecture (Secure Protocols)

**2. The Answer and Explanation:**
**SFTP** (SSH File Transfer Protocol / Secure File Transfer Protocol)
SFTP is a network protocol that provides file access, file transfer, and file management capabilities. It runs over the Secure Shell (SSH) protocol, which ensures that both the commands (like authentication) and the actual data being transferred are encrypted and secure from interception.

**3. Incorrect Answers:**
- **TFTP (Trivial File Transfer Protocol):** A very simple file transfer protocol that transmits data in cleartext (unencrypted) and does not require any authentication. It provides no security.
- **Telnet:** A legacy network protocol used for remote terminal access, not file transfer. It transmits all data, including usernames and passwords, in cleartext, making it highly insecure.
- **FTPS (File Transfer Protocol Secure):** An extension to the standard FTP protocol that adds encryption. However, FTPS uses SSL/TLS for encryption, whereas SFTP uses SSH. 

**4. Study Tips:**
To easily remember the difference between the two secure file transfer protocols:
- **SFTP** starts with **S**, just like **SSH**.
- **FTPS** ends with **S**, just like **TLS/SSL**.

--------------------------------------------------------------------------------

**Question:** Which of the following answers refers to a data storage device equipped with hardware-level encryption functionality?
- HSM
- TPM
- EFS
- SED

**1. Domain and Objective Category:**
Domain 3: Security Architecture (Hardware and Data Protection)

**2. The Answer and Explanation:**
The correct answer is **SED** (Self-Encrypting Drive).
An SED is a hard disk drive (HDD) or solid-state drive (SSD) that has an encryption circuit built directly into the drive's controller. This means the *storage device itself* transparently handles all the encryption and decryption at the hardware level, taking the processing load off the computer's main CPU.

**3. Incorrect Answers:**
- **HSM (Hardware Security Module):** This is a dedicated hardware appliance or server card that manages digital keys and performs heavy-duty cryptographic operations. It is not a general data storage device for user files.
- **TPM (Trusted Platform Module):** A dedicated hardware chip on a computer's motherboard that securely stores cryptographic keys. Like the HSM, it is a key vault, not a data storage device (like a hard drive).
- **EFS (Encrypting File System):** This is a *software*-level encryption feature built into the Windows operating system for encrypting individual files or folders. It is software, not a piece of hardware.

**4. Study Tips:**
If the question asks for a *storage device* (like a hard drive) with built-in *hardware encryption*, the answer is **SED** (Self-Encrypting Drive). If it asks about a chip on the motherboard that *stores keys* for encryption, it's **TPM**. If it asks for an external enterprise server/appliance that manages keys, it's **HSM**.

--------------------------------------------------------------------------------

**Question:** Which of the following answers refers to an obsolete protocol used for secure data transfer over the web?
- SMTPS
- SRTP
- SHTTP
- S/MIME

**1. Domain and Objective Category:**
Domain 2: Architecture and Design (Secure Protocols)

**2. The Answer and Explanation:**
The correct answer is **SHTTP** (Secure Hypertext Transfer Protocol).
SHTTP was an early protocol developed in the 1990s for secure data transfer over the web, competing directly with SSL (which later evolved into TLS and HTTPS). While HTTPS encrypts the entire communication session, SHTTP encrypted individual messages. SHTTP ultimately lost the standards battle to HTTPS and is now entirely obsolete.

**3. Incorrect Answers:**
- **SMTPS (Simple Mail Transfer Protocol Secure):** This is a deprecated protocol for securing *email* transmission, not for general data transfer over the web.
- **SRTP (Secure Real-Time Transport Protocol):** This is an active, modern protocol used for securing voice and video traffic (like VoIP and video calls), not general web traffic. It is not obsolete.
- **S/MIME (Secure/Multipurpose Internet Mail Extensions):** This is a standard used to encrypt and digitally sign *email contents*. It is used for email, not web data transfer, and is still widely used today.

**4. Study Tips:**
Don't confuse **SHTTP** (Secure HTTP, which is obsolete) with **HTTPS** (HTTP Secure, which is the modern standard). Notice the position of the 'S'. If the 'S' is at the front (SHTTP), it's the old, dead one. If the 'S' is at the end (HTTPS), it's the modern, alive one!

--------------------------------------------------------------------------------
**Question:**
Which of the following answers refers to a family of cryptographic hash functions designed for various security-related applications, including digital signatures, password storage, secure communications, and data integrity verification?
- RSA
- AES
- PKCS
- SHA

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography)

**2. The Answer and Explanation:**
**SHA (Secure Hash Algorithm)**
SHA is a family of cryptographic hash functions (such as SHA-1, SHA-2, and SHA-3) published by the National Institute of Standards and Technology (NIST). Hash functions take input data of any size and produce a fixed-size output (a hash value or digest). They are primarily used to ensure data integrity, securely store passwords, and support digital signatures.

**3. Incorrect Answers:**
- **RSA (Rivest-Shamir-Adleman):** This is an asymmetric encryption algorithm that uses a pair of keys (public and private). It is used for securing data transmission and digital signatures, but it is an encryption algorithm, not a hash function.
- **AES (Advanced Encryption Standard):** This is a symmetric encryption algorithm widely used to encrypt and decrypt data to keep it confidential. It is not a hash function.
- **PKCS (Public-Key Cryptography Standards):** This refers to a family of standards created by RSA Security to promote the use of public-key cryptography techniques, not a specific algorithm itself.

**4. Study Tips:**
An easy way to remember this is to look at the name! The **"H"** in S**H**A stands for **H**ash. 
- **SHA** = **H**ash (Used for Data Integrity)
- **AES** = Symmetric Encryption (Used for Data Confidentiality)
- **RSA** = Asymmetric Encryption (Used for Key Exchange/Digital Signatures)

--------------------------------------------------------------------------------

**Question:**
Which of the hash functions listed below offers the highest level of security?
- MD5
- SHA-3
- RIPEMD-160
- HMAC

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography)

**2. The Answer and Explanation:**
**SHA-3**
SHA-3 (Secure Hash Algorithm 3) is the newest member of the Secure Hash Algorithm family standard published by NIST. It uses a completely different internal structure compared to older algorithms, making it highly secure and resistant to collision attacks.

**3. Incorrect Answers:**
- **MD5 (Message Digest 5):** This algorithm is considered obsolete and cryptographically broken. It is highly vulnerable to collision attacks (where two different inputs produce the same hash) and should never be used for high-security applications.
- **RIPEMD-160:** While more secure than MD5, this is an older 160-bit hash function. It is generally considered less secure and is less widely adopted than the modern SHA-2 or SHA-3 families.
- **HMAC (Hash-based Message Authentication Code):** HMAC is not a standalone hashing algorithm. It is a technique that combines a cryptographic hash function (like SHA-256 or MD5) with a secret cryptographic key. Its security entirely depends on the underlying hash function it is paired with.

**4. Study Tips:**
When you see numbers after algorithms like SHA, bigger usually means better/newer! 
- **MD5** = Old and broken (avoid for security).
- **HMAC** = Needs a secret key + a hash function (it's a process/framework, not a standalone hash algorithm).
- **SHA-3** = The newest and strongest hash family tested on the exam.

--------------------------------------------------------------------------------

**Question:**
Which of the following combines a cryptographic hash function with a secret key to provide a means of verifying both the authenticity and integrity of a message or data?
- MD5
- DSA
- HMAC
- DES

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography)

**2. The Answer and Explanation:**
**HMAC (Hash-based Message Authentication Code)**
HMAC is a specific type of message authentication code that combines a standard cryptographic hash function (such as SHA-256 or MD5) with a secret cryptographic key. Because it requires a secret key that is only known by the sender and receiver, it verifies the *authenticity* of the sender, while the hash function verifies the *integrity* of the data.

**3. Incorrect Answers:**
- **MD5 (Message Digest 5):** This is a standalone hashing algorithm. While it verifies data integrity, it does not use a secret key on its own, so it cannot verify authenticity.
- **DSA (Digital Signature Algorithm):** This is a federal standard for digital signatures. While it verifies both integrity and authenticity, it uses *asymmetric* cryptography (public/private key pairs), not a hash combined with a single secret key.
- **DES (Data Encryption Standard):** This is a very old, symmetric encryption algorithm used to provide confidentiality, not a hashing algorithm or message authentication code. 

**4. Study Tips:**
The answer is right in the acronym! 
- **H** = **H**ash-based (Uses a hash function)
- **MAC** = **M**essage **A**uthentication **C**ode (Uses a secret key to authenticate)
If the exam mentions combining a hash and a secret key, **HMAC** is your answer.

--------------------------------------------------------------------------------

**Question:**
Which of the answers listed below refers to a non-cryptographic hash function often used for error-checking purposes?
- MD5
- CRC
- SHA
- RIPEMD

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography)

**2. The Answer and Explanation:**
**CRC (Cyclic Redundancy Check)**
A CRC is an error-detecting code (a non-cryptographic hash function) commonly used in digital networks and storage devices to detect accidental changes to raw data. For example, it checks if a file got corrupted while downloading or transferring to a USB drive. Because it is non-cryptographic, it provides no real security against a malicious attacker who intentionally tampers with the data.

**3. Incorrect Answers:**
- **MD5 (Message Digest 5):** This is a cryptographic hash function. Even though it is considered obsolete and vulnerable today, it was designed for security, not just simple error-checking.
- **SHA (Secure Hash Algorithm):** This is a highly secure family of cryptographic hash functions designed for digital signatures, password storage, and data integrity verification.
- **RIPEMD:** This is also a cryptographic hash function designed specifically for security purposes.

**4. Study Tips:**
Think of **CRC** like a simple spell-check for computers. It catches accidental typos (errors during transfer), but it won't stop a hacker who is actively trying to trick it. 
- **CRC** = Accidental Error Checking
- **MD5 / SHA / RIPEMD** = Cryptographic Security

--------------------------------------------------------------------------------

**Question:**
Which of the following answers refers to a type of additional input that increases password complexity and provides better protection against brute-force, dictionary, and rainbow table attacks?
- Seed
- IV
- Salt
- Shim

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography)

**2. The Answer and Explanation:**
**Salt**
A salt is a string of random data that is added to a password before it goes through a hashing algorithm. By adding this random data, it ensures that the resulting hash is completely unique, even if two users happen to choose the exact same password. This completely neutralizes rainbow table attacks (pre-computed lists of password hashes) and makes dictionary and brute-force attacks significantly harder.

**3. Incorrect Answers:**
- **Seed:** A seed is a starting number used by algorithms that generate pseudo-random numbers. While it involves randomness, it is not the specific security control used to protect password hashes.
- **IV (Initialization Vector):** An IV is a random or pseudo-random value used in symmetric encryption algorithms (block ciphers) to ensure that the same plaintext encrypted multiple times results in different ciphertexts. It is used for *encryption*, whereas a salt is used for *hashing*.
- **Shim:** A shim is a piece of software code that sits between two components and intercepts API calls, often used for maintaining backwards compatibility with older software or, maliciously, by malware to intercept data. It has nothing to do with cryptography.

**4. Study Tips:**
Just like we discussed earlier, think of a **Salt** as adding a unique "flavor" to every single password in a database. If a hacker brings their pre-cooked cheat sheet (a Rainbow Table), it won't work because every password has been uniquely salted!

--------------------------------------------------------------------------------

**Question:**
Which of the following answers refer to algorithms used for generating and verifying digital signatures? (Select 3 answers)
- ECDSA
- RSA
- ECDHE
- DSA
- GPG/PGP

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography)

**2. The Answer and Explanation:**
**ECDSA, RSA, and DSA**
- **ECDSA (Elliptic Curve Digital Signature Algorithm):** This is a highly efficient algorithm that uses elliptic curve cryptography to create digital signatures using much smaller key sizes than traditional methods.
- **RSA (Rivest-Shamir-Adleman):** This is a widely used, highly versatile asymmetric algorithm that can be used for both encrypting data *and* generating digital signatures.
- **DSA (Digital Signature Algorithm):** This is a federal standard designed specifically for generating and verifying digital signatures. 

**3. Incorrect Answers:**
- **ECDHE (Elliptic Curve Diffie-Hellman Ephemeral):** This is a *key exchange* algorithm, not a signature algorithm. It is used to securely swap encryption keys over the internet while providing perfect forward secrecy.
- **GPG/PGP (GNU Privacy Guard / Pretty Good Privacy):** These are software suites/protocols that *use* digital signature algorithms (like RSA) to secure emails and files, but they are not the mathematical algorithms themselves.

**4. Study Tips:**
When you see **DSA**, think **D**igital **S**ignature **A**lgorithm! Both **DSA** and **ECDSA** give away the answer right in their names. Also, remember that **RSA** is the "Jack of all trades" that can do both encryption and signatures. 

--------------------------------------------------------------------------------

**Question:**
Which of the following answers refer to the characteristic features of RSA? (Select 3 answers)
- Asymmetric encryption algorithm
- A public key used for encryption and a private key used for decryption
- Suitable for bulk data encryption
- Used for secure communications, digital signatures, and key exchange
- Symmetric encryption algorithm
- A single key used for both encryption and decryption

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography)

**2. The Answer and Explanation:**
**Asymmetric encryption algorithm; A public key used for encryption and a private key used for decryption; Used for secure communications, digital signatures, and key exchange.**
RSA is a classic, highly versatile asymmetric algorithm. Because it is asymmetric, it inherently uses a mathematical pair of keys: a Public Key for encryption and a Private Key for decryption. It is essentially the "Swiss Army Knife" of cryptography, as it can be used for securely exchanging symmetric keys, establishing secure communication channels, and creating digital signatures.

**3. Incorrect Answers:**
- **Suitable for bulk data encryption:** Asymmetric algorithms like RSA are incredibly slow and resource-heavy. They should never be used to encrypt large amounts of data (bulk data). Fast, symmetric algorithms like AES handle bulk data. 
- **Symmetric encryption algorithm:** RSA uses two different keys, so it is asymmetric.
- **A single key used for both encryption and decryption:** This is the definition of symmetric encryption (like AES), not asymmetric encryption like RSA.

**4. Study Tips:**
Think of RSA as the ultimate multitasker: it's **Asymmetric** and does almost everything (encryption, key exchange, signatures). But remember the golden rule of asymmetric math: it is **very slow**. Therefore, you never use it for bulk data!

--------------------------------------------------------------------------------

**Question:**
Key stretching is a cryptographic technique that enhances the security of sensitive data, such as cryptographic keys and passwords. It works by repeatedly applying a resource-intensive function or algorithm to the input data, thus increasing the computational effort required to derive the original key or password, which makes the data more resistant to brute-force, dictionary, or rainbow table attacks.
- True
- False

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography)

**2. The Answer and Explanation:**
**True**
The statement is completely accurate. Key stretching algorithms (like PBKDF2, Bcrypt, or Argon2) intentionally make the hashing process slow and resource-heavy. They usually do this by running the hash algorithm thousands of times in a loop. By forcing the computer to do massive amounts of math for every single password attempt, it severely limits how many guesses a hacker can make per second.

**3. Incorrect Answers:**
- **False:** This is incorrect because the provided definition perfectly describes the concept and purpose of key stretching. 

**4. Study Tips:**
Think of key stretching like forcing a hacker to run a marathon through thick mud. Normally, a powerful computer can guess billions of passwords a second. Key stretching slows the computer down so much that a brute-force attack could take centuries instead of hours!

--------------------------------------------------------------------------------

**Question:**
The term "Open public ledger" is used to describe a distributed database stored across multiple computers in a P2P network.
- True
- False

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography - Blockchain)

**2. The Answer and Explanation:**
**True**
The statement accurately defines an open public ledger. More commonly known as a **Blockchain**, an open public ledger is a decentralized, distributed database that is shared among the nodes (computers) of a peer-to-peer (P2P) network. Everyone on the network holds a copy of this ledger, ensuring transparency and making it extremely difficult for any single person to alter or forge transaction records.

**3. Incorrect Answers:**
- **False:** This is incorrect because the definition perfectly describes the core concept behind blockchain and distributed ledger technology.

**4. Study Tips:**
Whenever you see the phrase "open public ledger" or "distributed ledger," immediately think of **Blockchain** (like the technology behind Bitcoin). The entire point of a blockchain is that the record book (the ledger) is public and shared across thousands of computers, so nobody can secretly cheat the system!

--------------------------------------------------------------------------------

**Question:**
Which of the answers listed below refers to a set of standards and specifications that define various cryptographic techniques, including formats for public keys, private keys, digital signatures, and digital certificates?
- ITIL
- RFC
- PKCS
- ISO/IEC

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography - PKI)

**2. The Answer and Explanation:**
**PKCS (Public-Key Cryptography Standards)**
PKCS is a group of technical standards originally created by RSA Security. These standards essentially act as the "rulebook" for public-key cryptography, ensuring that different software programs and hardware devices can securely exchange keys, certificates, and digital signatures in a language they all understand (such as the popular PKCS #12 format used to store server certificates and private keys).

**3. Incorrect Answers:**
- **ITIL (Information Technology Infrastructure Library):** This is a set of best practices for managing IT services and aligning them with business needs (like helpdesk ticketing processes). It has nothing to do with cryptography.
- **RFC (Request for Comments):** This is a formal document created by the Internet Engineering Task Force (IETF) to define how internet protocols work. While there are RFCs *about* cryptography, RFC is a general publishing format, not a specific set of cryptographic standards.
- **ISO/IEC:** These are massive international organizations that publish standards for almost everything in the world (from cybersecurity frameworks to the exact dimensions of credit cards). It is far too broad to be the specific answer here.

**4. Study Tips:**
This is an easy one if you know what the acronym stands for! When the question asks about **Public Key** and **Standards**, look for the answer that literally means **P**ublic-**K**ey **C**ryptography **S**tandards (**PKCS**).

--------------------------------------------------------------------------------

**Question:**
Which of the following defines a file format for storing and exchanging personal identity information, including private keys and digital certificates?
- P10
- P11
- P12
- P13

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography - PKI)

**2. The Answer and Explanation:**
**P12**
P12 (short for PKCS #12) is a highly secure, password-protected file format. It is specifically designed to bundle a digital certificate (which contains the public key) together with its matching private key. Because it holds both halves of the key pair, it is commonly used by administrators to transfer and install identity information onto web servers or user devices.

**3. Incorrect Answers:**
- **P10 (PKCS #10):** This is the format for a Certificate Signing Request (CSR). It is the file you send to a Certificate Authority when you are *asking* them to create a certificate for you. It does not store your private key.
- **P11 (PKCS #11):** This is not a file format at all. It is a programming interface (API) that allows software to talk to cryptographic hardware, like smart cards or Hardware Security Modules (HSMs).
- **P13 (PKCS #13):** This standard relates to Elliptic Curve Cryptography, but it is not a file format used for bundling certificates and private keys.

**4. Study Tips:**
Think of **P12** like a securely locked briefcase. It is the only format on the exam that carries a **bundle** of both your digital certificate AND your highly sensitive private key! (Note: You may also see P12 files referred to as **.PFX** files; they are essentially the same thing).

--------------------------------------------------------------------------------

**Question:**
What is the role of Registration Authority (RA) in PKI? (Select 2 answers)
- Accepting requests for digital certificates
- Validating digital certificates
- Authenticating the entity making the request
- Providing backup source for cryptographic keys
- Issuing digital certificates

**1. Domain and Objective Category:**
Domain 1: General Security Concepts (Objective 1.4: Explain the concepts of cryptography - PKI)

**2. The Answer and Explanation:**
**Accepting requests for digital certificates; Authenticating the entity making the request**
In a Public Key Infrastructure (PKI), the Registration Authority (RA) acts as the "front desk." When a user or device needs a new certificate, they send their request (a CSR) to the RA. The RA is responsible for accepting that request and rigorously verifying the identity of whoever is asking for it. Once the RA is satisfied that the user is who they claim to be, it forwards the approved request to the Certificate Authority (CA). 

**3. Incorrect Answers:**
- **Issuing digital certificates:** This is the most common trap! The RA *never* issues the certificate. Only the **Certificate Authority (CA)** actually generates and issues the certificate.
- **Validating digital certificates:** Checking if a certificate is currently valid or revoked is done by checking a CRL (Certificate Revocation List) or using OCSP (Online Certificate Status Protocol), not by the RA.
- **Providing backup source for cryptographic keys:** Backing up and storing private keys securely is handled by a Key Escrow system, not the RA.

**4. Study Tips:**
Think of getting a passport! 
- The **RA (Registration Authority)** is like your local Post Office. You hand them your application (accepting the request), and they check your driver's license to make sure you are who you say you are (**authenticating** the entity). 
- The **CA (Certificate Authority)** is the Federal Government. The Post Office sends them your approved application, and the Government is the one that actually **issues** (prints) the passport. 

--------------------------------------------------------------------------------

