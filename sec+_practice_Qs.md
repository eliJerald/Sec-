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
