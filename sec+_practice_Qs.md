# Security+ SY0-701 Practice Questions

### Question 1
An attacker uses a 50 dollar device to copy the data from a high-level executive’s badge while standing near them in a crouded elevator. Which of the following best describes this attack type?

A. Biometric Spoofing
B. Brute force
C. Denial of Service
D. FRID Cloning
E. On path attack

**1. The Answer:**
D. FRID Cloning (Note: This is likely a typo for "RFID Cloning").

**2. Why that answer is correct:**
RFID (Radio Frequency Identification) cloning involves using a specialized, often inexpensive device to read and copy the information stored on a physical RFID card or badge. Because RFID technology uses radio waves to transmit data, an attacker simply needs to be in close physical proximity to the victim to secretly scan and steal the badge's credentials—perfectly describing the crowded elevator scenario.

**3. Why the other answers are incorrect:**
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

**1. The Answer:**
B. Secure Access Service Edge (SASE)

**2. Why that answer is correct:**
Secure Access Service Edge (SASE) is a cloud-native architecture that combines network security functions (like secure web gateways, cloud access security brokers, firewalls, and zero-trust network access) with wide area networking (WAN) capabilities. Because it is delivered as a cloud service, it ensures that all users—whether they are sitting in a corporate office or working from a mobile device at a coffee shop—are routed through the same security policies and protections before accessing the internet or corporate resources.

**3. Why the other answers are incorrect:**
- **A. Software-defined networking (SDN):** SDN separates the network's control logic from its forwarding hardware to make networks more agile and easier to manage, typically within a data center or campus. While modern, it is primarily a networking architecture, not a cloud-native security model for remote mobile users.
- **C. Site-to-site IPsec tunneling:** This creates a secure, encrypted connection between two fixed geographic locations (like a branch office and a main headquarters). It doesn't solve the problem of mobile, roaming users needing consistent security enforcement from anywhere.
- **D. Next-Generation Firewall (NGFW):** While an NGFW provides deep packet inspection and advanced security policies, traditional NGFWs are typically physical or virtual appliances deployed at a specific location's perimeter. It doesn't inherently push a cloud-native security model to remote mobile users.
- **E. Virtual Private Network Concentrator:** A VPN concentrator handles incoming remote access VPN connections, bringing remote users onto the corporate network. It forces all traffic to "trombone" or backhaul through the central data center to get security enforcement, which is exactly the non-cloud-native, legacy model organizations try to move away from with SASE.

--------------------------------------------------------------------------------

