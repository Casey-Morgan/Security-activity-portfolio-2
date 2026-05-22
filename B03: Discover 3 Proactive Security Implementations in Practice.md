# B03: Discover 3 Proactive Security Implementations in Practice

## Overview

This portfolio activity identifies three proactive security implementations that are commonly used in real-world environments to reduce risk before an incident occurs. Each example focuses on prevention, early detection, resilience, and security-by-design rather than reacting only after a compromise.

---

## 1. Multi-Factor Authentication for Account Protection

### Implementation

Multi-factor authentication is a proactive control that requires users to provide more than one form of verification before accessing an account. For example, a university, workplace, or cloud service may require a password plus a one-time code, authenticator app approval, hardware security key, or biometric verification.

### How It Works in Practice

A user first enters their username and password. The system then asks for a second factor, such as a push notification from an authenticator app or a code generated on a trusted device. Access is only granted when both factors are successfully verified.

### Why It Is Proactive

MFA reduces the chance that a stolen password alone can be used to access an account. This is proactive because it protects the account before an attacker can successfully use compromised credentials.

### Security Benefits

- Reduces the impact of password theft and credential stuffing.
- Makes phishing attacks less effective when phishing-resistant MFA is used.
- Adds protection for remote access, email, cloud storage, and administrative accounts.
- Helps organisations enforce stronger identity and access management.

<img width="1320" height="1710" alt="Screenshot 2026-05-22 at 13 13 22" src="https://github.com/user-attachments/assets/758366e3-d07c-4cee-8e67-94ce6ca21be8" />


### Limitations

MFA is not perfect. SMS-based codes can be vulnerable to SIM-swap attacks, and push notifications can be abused through MFA fatigue attacks. Stronger options such as authenticator apps, number matching, passkeys, or hardware security keys provide better protection.

---

## 2. Automated Vulnerability Scanning in a Development Workflow

### Implementation

Automated vulnerability scanning is a proactive security practice where tools check code, dependencies, containers, or infrastructure for known weaknesses before software is deployed. Examples include GitHub Dependabot, Snyk, npm audit, Trivy, OWASP Dependency-Check, and GitHub CodeQL.

### How It Works in Practice

When code is pushed to a repository, a scanning tool checks the project for insecure dependencies, outdated packages, exposed secrets, or risky code patterns. If a problem is found, the tool creates an alert or pull request recommending an update or fix.

### Why It Is Proactive

The weakness is identified before an attacker can exploit it in production. Instead of waiting for a breach, the development team receives early warnings during coding, testing, or continuous integration.

### Security Benefits

- Identifies vulnerable dependencies early.
- Encourages regular patching and secure software maintenance.
- Reduces the risk of deploying known vulnerabilities.
- Helps developers learn secure coding practices through direct feedback.
- Supports DevSecOps by integrating security into the development lifecycle.

<img width="1600" height="853" alt="697fce83773590c9d36195fb_834eef65" src="https://github.com/user-attachments/assets/577eb005-0420-4ec9-87e8-33b231be4062" />


### Limitations

Automated scanners can produce false positives or miss business logic flaws. They are most effective when combined with manual code review, secure design practices, penetration testing in authorised environments, and regular patch management.

---

## 3. Network Segmentation to Limit Attack Movement

### Implementation

Network segmentation separates systems into different network zones based on trust level, function, or sensitivity. For example, guest Wi-Fi can be separated from internal staff systems, production servers can be separated from development systems, and administrative interfaces can be restricted to a management network.

### How It Works in Practice

Firewall rules, VLANs, access control lists, or cloud security groups are used to control which devices and services can communicate. A user on a guest network may be allowed to access the internet but blocked from reaching internal file servers, databases, or administrative dashboards.

### Why It Is Proactive

Segmentation reduces the damage an attacker can cause if one device or account is compromised. It limits lateral movement and makes it harder for an attacker to reach sensitive systems.

### Security Benefits

- Reduces the blast radius of a compromised endpoint.
- Protects critical systems from unnecessary exposure.
- Supports least privilege at the network level.
- Makes monitoring easier by separating normal and suspicious traffic patterns.
- Helps meet security and compliance requirements for sensitive environments.

<img width="1150" height="823" alt="microsoft-entra-global-secure-access-health-check-success" src="https://github.com/user-attachments/assets/ede9b4c1-08a4-4a51-bd15-6560eaf79d31" />


### Limitations

Network segmentation must be designed carefully. Overly permissive rules, poor documentation, flat internal networks, or unmanaged exceptions can weaken the control. Segmentation should be reviewed regularly as systems and business needs change.

---

## Comparison Table

| Proactive implementation | Main purpose | Example environment | Primary security value |
|---|---|---|---|
| Multi-factor authentication | Strengthen account login security | Email, cloud services, VPN, admin portals | Prevents password-only compromise |
| Automated vulnerability scanning | Detect weaknesses before deployment | GitHub repository, CI/CD pipeline, container images | Finds known vulnerabilities early |
| Network segmentation | Restrict unnecessary communication | Campus network, office network, cloud environment | Limits lateral movement and damage |

---

## Reflection

These three implementations demonstrate proactive cybersecurity because they reduce risk before an incident becomes serious. MFA protects identities before stolen passwords are misused, automated scanning identifies weaknesses before deployment, and network segmentation limits the impact of compromise before an attacker can move freely across systems.

The strongest security outcome comes from combining these controls. For example, an organisation could require MFA for developers, scan code before deployment, and host production systems in segmented networks. Together, these practices support defence-in-depth and reduce reliance on a single security control.
