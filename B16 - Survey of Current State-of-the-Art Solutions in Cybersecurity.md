# B16 - Survey of Current State-of-the-Art Solutions in Cybersecurity

## Overview

This activity surveys current state-of-the-art solutions in cybersecurity. The purpose is to understand modern defensive technologies, how they are used in practice, and what limitations they still have.

Cybersecurity has moved beyond relying only on firewalls and antivirus software. Modern security uses layered defence, identity protection, behavioural monitoring, automation, and continuous risk management.

---

## 1. Zero Trust Architecture

### Description

Zero Trust Architecture is a security model based on the idea of **never trust, always verify**. Instead of assuming users or devices inside a network are safe, every access request is checked continuously.
<img width="1075" height="605" alt="Zero-Trust-framework" src="https://github.com/user-attachments/assets/c5e8b9d9-83f1-482b-8363-3a7a18ff356a" />

### Key Features

- Strong identity verification
- Multi-factor authentication
- Least privilege access
- Device health checks
- Continuous monitoring
- Network segmentation

### Example Use Case

A university or company may use Zero Trust so that students or staff can only access systems they are authorised to use. Even if a user logs in successfully, access may still be limited based on device status, location, and risk level.

<img width="1000" height="640" alt="What-is-Zero-Trust-Architecture-_1" src="https://github.com/user-attachments/assets/e466ea48-d687-4a3c-a611-9cb9f633e4a2" />

### Benefits

- Reduces damage if an account is compromised
- Limits unnecessary access
- Works well with cloud and remote work environments
- Improves visibility over users and devices

### Limitations

- Can be complex to implement
- Requires good identity and access management
- May affect user experience if controls are poorly configured
- Needs continuous maintenance
<img width="1042" height="745" alt="Steps-to-Design-a-Zero-Trust-System" src="https://github.com/user-attachments/assets/d66ae173-0dbc-4eee-925b-5ef90618a452" />
---

## 2. Extended Detection and Response (XDR)

### Description

Extended Detection and Response combines security data from multiple sources, such as endpoints, cloud services, email, identity systems, and networks. It helps security teams detect and respond to attacks more quickly.

### Key Features

- Centralised threat detection
- Automated correlation of alerts
- Endpoint and network visibility
- Incident investigation support
- Response automation

### Example Use Case

If a phishing email leads to a suspicious login and then unusual file activity on a laptop, XDR can connect these events together and show them as one incident.

### Benefits

- Reduces alert fatigue
- Gives a wider view of attacks
- Helps security teams respond faster
- Improves incident investigation

### Limitations

- Can be expensive
- Requires skilled security staff
- May produce false positives
- Depends on good data collection from many systems

---

## 3. Security Information and Event Management with AI Analytics

### Description

Security Information and Event Management, known as SIEM, collects logs from different systems and helps detect suspicious activity. Modern SIEM platforms often use artificial intelligence and machine learning to identify unusual behaviour.

### Key Features

- Log collection and analysis
- Threat detection rules
- Behaviour analytics
- Alert generation
- Compliance reporting
- Integration with response tools

### Example Use Case

A SIEM can detect when a user logs in from two countries within a short time or when an administrator account performs unusual actions late at night.

### Benefits

- Improves visibility across systems
- Supports compliance and auditing
- Helps detect insider threats
- Allows investigation using historical logs

### Limitations

- Requires correct log sources
- Poorly configured SIEMs can create too many alerts
- AI-based detection may not always explain its reasoning clearly
- Needs tuning and maintenance

---

## 4. Cloud Security Posture Management (CSPM)
<img width="1024" height="521" alt="cspm-diagram" src="https://github.com/user-attachments/assets/0e011b52-8302-4b7e-b559-34c15e64507d" />

### Description

Cloud Security Posture Management tools monitor cloud environments for misconfigurations and risky settings. This is important because many cloud security incidents happen due to incorrect permissions or exposed storage.

### Key Features

- Cloud configuration scanning
- Misconfiguration detection
- Compliance checks
- Risk scoring
- Automated remediation suggestions
- Visibility across cloud accounts

### Example Use Case

A CSPM tool can detect if a cloud storage bucket is publicly accessible or if an identity has excessive permissions.

### Benefits

- Helps prevent cloud data leaks
- Improves cloud compliance
- Detects risky configurations quickly
- Supports large and complex cloud environments

### Limitations

- Does not replace secure cloud design
- May require cloud-specific expertise
- False positives can occur
- Automated fixes may cause issues if not reviewed

---

## 5. Passwordless Authentication and Passkeys

### Description

Passwordless authentication reduces or removes the need for traditional passwords. Passkeys are a modern approach that use public-key cryptography and device-based authentication, such as biometrics or PINs.

### Key Features

- No reusable password shared with websites
- Resistant to phishing
- Uses cryptographic key pairs
- Can work with fingerprint, face recognition, or device PIN
- Easier user experience than complex passwords

### Example Use Case

A student can sign in to an account using a passkey stored on their phone or laptop. A phishing website cannot easily steal the passkey because the private key does not leave the device.

### Benefits

- Strong protection against phishing
- Reduces password reuse
- Improves login experience
- Lowers risk from password database breaches

### Limitations

- Adoption is still growing
- Account recovery must be designed carefully
- Users may be confused during transition
- Device loss needs secure recovery options

---

## 6. Secure Access Service Edge (SASE)

### Description

Secure Access Service Edge combines networking and security functions into a cloud-delivered model. It is designed for organisations with remote users, cloud applications, and distributed offices.

### Key Features

- Secure web gateway
- Cloud access security broker
- Zero Trust network access
- Firewall as a service
- Data loss prevention
- Central policy management

### Example Use Case

A company with remote employees can use SASE to securely connect users to cloud applications without relying only on a traditional office network.

### Benefits

- Supports remote and hybrid work
- Centralises security policies
- Reduces reliance on legacy VPNs
- Improves visibility into cloud access

### Limitations

- Migration can be difficult
- Depends on reliable internet connectivity
- Vendor lock-in may be a concern
- Requires careful policy design

---

## 7. Threat Intelligence Platforms

### Description

Threat intelligence platforms collect, organise, and analyse information about cyber threats. This may include malicious IP addresses, domains, malware indicators, attacker tactics, and vulnerability information.

### Key Features

- Indicator collection
- Threat feed integration
- Attack pattern mapping
- Risk scoring
- Sharing of intelligence
- Integration with SIEM, firewall, and detection tools

### Example Use Case

A security team can use threat intelligence to block known malicious domains or prioritise patching when a vulnerability is actively exploited.

### Benefits

- Helps organisations understand current threats
- Supports faster detection and response
- Improves prioritisation of security work
- Can enrich alerts with extra context

### Limitations

- Intelligence quality varies
- Too many indicators can create noise
- Requires analysis to be useful
- Outdated indicators may cause false confidence

---

## 8. Deception Technology

### Description

Deception technology creates fake but realistic systems, files, credentials, or network resources to detect attackers. Legitimate users should not interact with these decoys, so interaction may indicate suspicious activity.

### Key Features

- Honeypots and decoy systems
- Fake credentials
- Fake network shares
- Early attacker detection
- Alert generation when decoys are touched

### Example Use Case

A company may place fake administrator credentials on a monitored system. If an attacker tries to use them, the security team receives an alert.

### Benefits

- Detects attackers inside the network
- Can reveal attacker behaviour
- Produces high-quality alerts
- Helps slow or mislead attackers

### Limitations

- Requires careful deployment
- Decoys must look realistic
- Does not stop attacks by itself
- Skilled attackers may avoid obvious traps

---

## Comparison Table

| Solution | Main Purpose | Strength | Limitation |
|---|---|---|---|
| Zero Trust Architecture | Control access continuously | Limits unauthorised access | Complex implementation |
| XDR | Detect and respond across systems | Connects related alerts | Needs skilled staff |
| AI-enabled SIEM | Analyse logs and detect anomalies | Strong visibility and auditing | Requires tuning |
| CSPM | Detect cloud misconfigurations | Reduces cloud exposure risk | Needs cloud expertise |
| Passkeys | Replace weak passwords | Strong phishing resistance | Adoption and recovery challenges |
| SASE | Secure remote and cloud access | Good for hybrid work | Migration complexity |
| Threat Intelligence Platforms | Understand and use threat data | Improves prioritisation | Data quality varies |
| Deception Technology | Detect intruders using decoys | High-quality alerts | Must be realistic |

---

## Discussion

Modern cybersecurity solutions are increasingly based on continuous monitoring, identity verification, automation, and risk-based decision-making. A common theme is that security is no longer limited to a network boundary. Users, devices, applications, and data may be spread across cloud services and remote locations.

The most useful approach is layered defence. For example, an organisation may use Zero Trust for access control, XDR for detection and response, SIEM for log analysis, CSPM for cloud security, and passkeys for phishing-resistant authentication.

However, state-of-the-art tools do not remove the need for good security management. Tools must be configured correctly, monitored regularly, and supported by trained people and clear processes.

---

## Reflection

This activity helped me understand that modern cybersecurity is not based on one single product. Effective defence requires a combination of technology, policy, monitoring, and user education.

The most interesting solution was passkey-based authentication because it directly addresses one of the most common causes of account compromise: weak or stolen passwords. I also found XDR important because attacks often involve multiple steps across email, identity, endpoint, and cloud systems.

A key lesson is that advanced tools can still fail if they are poorly implemented. Strong cybersecurity depends on both technical controls and responsible operational practice.

---

## Portfolio Claim

This activity satisfies **B16: Survey the current state-of-the-art solutions in cybersecurity**.

The survey covered the following current cybersecurity solution areas:

1. Zero Trust Architecture
2. Extended Detection and Response
3. AI-enabled SIEM
4. Cloud Security Posture Management
5. Passwordless authentication and passkeys
6. Secure Access Service Edge
7. Threat intelligence platforms
8. Deception technology
