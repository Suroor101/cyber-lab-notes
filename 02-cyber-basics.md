# 02 - Cybersecurity Basics

---

## Types of Threats

Cyber threats are methods attackers use to harm systems or steal data. Below is each threat with a clear definition:

- **Malware**  
  **Definition:** Software designed to infiltrate, damage, or control devices without the user’s consent.  
  **Examples:**  
  - **Virus:** Attaches to files and spreads when executed.  
  - **Worm:** Self‑replicates across networks without user action.  
  - **Ransomware:** Encrypts files and demands payment.  
  - **Spyware:** Monitors user activity and steals information.
  - **Adware:** Displays Unwanted advertisements, some are malicious

- **Phishing**  
  **Definition:** Social‑engineering attack where fraudsters send deceptive messages to trick users into revealing credentials or clicking malicious links.  
  **Characteristics:**  
  - Often mimics trusted brands (banks, services)  
  - May include urgent “account locked” or “payment required” warnings  
  - Can deliver malware or harvest login details

- **Denial of Service (DoS/DDoS)**  
  **Definition:** Overwhelming a target system with traffic or requests to make it unavailable to legitimate users.  
  **Variants:**  
  - **DoS:** Single source flood.  
  - **DDoS:** Multiple compromised systems (botnets) launch a coordinated flood.

- **Man-in-the-Middle (MitM)**  
  **Definition:** Attacker secretly intercepts and possibly alters communication between two parties without their knowledge.  
  **Scenarios:**  
  - Public Wi‑Fi eavesdropping  
  - HTTPS downgrade attacks  
  - Session hijacking

- **SQL Injection**  
  **Definition:** Inserting malicious SQL statements into input fields to manipulate a web application’s database.  
  **Risks:**  
  - Data extraction (user lists, financial records)  
  - Data modification or deletion  
  - Full system compromise if stacked with other flaws

- **Zero-Day Exploits**  
  **Definition:** Attacks that target software vulnerabilities unknown to developers and unpatched at the time of exploit.  
  **Implications:**  
  - No immediate defense available  
  - High value on black markets  
  - Often used in targeted espionage

- **Insider Threats**  
  **Definition:** Risks posed by trusted individuals within an organization (employees, contractors) who misuse access, either intentionally or by accident.  
  **Examples:**  
  - Exfiltration of sensitive data  
  - Accidental data leaks via misconfiguration  
  - Sabotage of systems

---

## CIA Triad (from GeeksforGeeks)

The **CIA Triad** outlines the three fundamental goals of information security. Every control or policy should support one or more of these:

1. **Confidentiality**  
   - **Definition:** Ensuring that sensitive information is accessed only by authorized individuals.  
   - **Controls:** Encryption (AES, TLS), strong authentication (MFA), strict access permissions.

2. **Integrity**  
   - **Definition:** Guaranteeing that data remains accurate, complete, and unaltered unless by authorized actions.  
   - **Controls:** Cryptographic hashes (SHA‑256), digital signatures, version control, checksums.

3. **Availability**  
   - **Definition:** Making sure systems and data are accessible to authorized users when needed.  
   - **Controls:** Redundant servers, load balancers, regular backups, DDoS mitigation services.

> A breach of any one of these pillars constitutes a security incident.  

---

## Real-World Breaches

### 1. Equifax Data Breach (2017)

- **What happened:**  
  Attackers exploited a known vulnerability in Apache Struts (CVE‑2017‑5638) that Equifax failed to patch.

- **Impact:**  
  Personal data of 147 million people was stolen, including names, Social Security numbers, birth dates, and addresses.

- **Cause:**  
  The vulnerability had a patch available months before the attack, but Equifax’s systems remained unpatched.

- **Lessons learned:**  
  - Patch management is critical — delays can be catastrophic.  
  - Inventory and monitor all internet-facing applications.  
  - Regular vulnerability scans could have caught this earlier.

---

### 2. WannaCry Ransomware Attack (2017)

- **What happened:**  
  WannaCry ransomware used the EternalBlue exploit (originally developed by the NSA) to target a flaw in Windows SMBv1 protocol.

- **Impact:**  
  Over 200,000 computers were affected in 150+ countries. Systems were locked and ransom demanded in Bitcoin.

- **Major victims:**  
  UK’s National Health Service (NHS), FedEx, Telefonica, Renault, and others.

- **Cause:**  
  Organizations failed to apply Microsoft’s critical SMB patch (MS17-010) released two months earlier.

- **Lessons learned:**  
  - Keep systems up-to-date with security patches.  
  - Disable outdated protocols like SMBv1.  
  - Offline backups are essential to recover from ransomware.

---

### 3. Facebook – Cambridge Analytica Scandal (2018)

- **What happened:**  
  A quiz app collected user data and also harvested data from friends of users via Facebook's API without proper consent.

- **Impact:**  
  Data from ~87 million users was collected and used for targeted political advertising and profiling.

- **Cause:**  
  Facebook failed to enforce strict data privacy policies for third-party apps and did not audit data use effectively.

- **Lessons learned:**  
  - Even without a breach, poor data governance can cause massive harm.  
  - Third-party access must be limited and audited.  
  - User consent and transparency are crucial for privacy.

