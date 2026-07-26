# Security+ SY0-701 Practice Questions

### Question 1
An attacker uses a 50 dollar device to copy the data from a high-level executive’s badge while standing near them in a crouded elevator. Which of the following best describes this attack type?

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

### Question 2
An organization is migrating its security stack to a cloud-native model to ensure mobile users receive the same security policy enforcement as office users. Which of the following would be the best choice for this requirement?

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

### Question 3
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

### Question 4
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

### Question 5
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

### Question 6
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

### Question 7
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

### Question 8
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
