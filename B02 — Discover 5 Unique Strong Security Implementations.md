# B2 — Discover 5 Unique Strong Security Implementations

This portfolio entry documents five different examples of strong security implementations. Each example explains what the implementation is, why it is effective, what security principles it supports, and how evidence can be collected for a portfolio submission.

---

## 1. Multi-Factor Authentication for User Accounts

### Security implementation

Multi-factor authentication requires users to provide more than one form of proof before gaining access to an account. A strong implementation usually combines something the user knows, such as a password, with something the user has, such as an authenticator app, hardware security key, or passkey.

### Why this is strong

Passwords are often exposed through phishing, credential reuse, malware, or database breaches. Multi-factor authentication reduces the risk that a stolen password alone can be used to access an account. Stronger options such as FIDO2 security keys and passkeys are especially effective because they are resistant to common phishing techniques.

### Security principles demonstrated

- Defence in depth
- Strong authentication
- Reduced reliance on passwords
- Protection against credential theft

### Example evidence to collect

- Screenshot of MFA being enabled on a test account
- Screenshot of available authentication methods, such as authenticator app or security key
- Notes explaining why SMS-based MFA is weaker than authenticator apps or hardware-backed options

### Defensive value

This implementation reduces account takeover risk and is one of the most effective protections for email, cloud platforms, source code repositories, learning management systems, and administrative dashboards.

---

## 2. Role-Based Access Control with Least Privilege

### Security implementation

Role-based access control assigns permissions according to a user’s role rather than giving all users the same level of access. A strong access control design only gives users the permissions they need to perform their tasks.

For example, a student user may only be able to view and submit work, while a tutor can mark submissions, and an administrator can manage user accounts and system settings.

### Why this is strong

Least privilege limits the damage that can occur if an account is misused or compromised. It also reduces accidental changes, unauthorised data access, and privilege abuse. A strong implementation separates normal user permissions from administrative permissions.

### Security principles demonstrated

- Least privilege
- Separation of duties
- Access control enforcement
- Reduced blast radius

### Example evidence to collect

- Table showing different roles and permissions
- Screenshot of a test user being denied access to an admin-only function
- Screenshot of an administrator account with additional permissions
- Short explanation of how permissions are checked before sensitive actions are allowed

### Defensive value

This implementation protects sensitive data and system functions by ensuring that users cannot access features outside their authorised role.

---

## 3. Secure Password Storage Using Salted Hashing

### Security implementation

Secure password storage means passwords are not stored in plain text. Instead, each password is processed through a slow password hashing algorithm with a unique salt. Strong examples include Argon2, bcrypt, scrypt, or PBKDF2 with appropriate parameters.

### Why this is strong

If a database is leaked, salted password hashes are much harder to use than plain-text passwords. A unique salt prevents attackers from using precomputed rainbow tables effectively. Slow hashing algorithms also make large-scale password guessing more expensive.

### Security principles demonstrated

- Secure data storage
- Protection of credentials at rest
- Resistance to offline brute-force attacks
- Secure cryptographic practice

### Example evidence to collect

- Code snippet showing bcrypt, Argon2, scrypt, or PBKDF2 being used
- Screenshot showing that stored password values are hashes rather than plain text
- Explanation that passwords should be verified by comparing hashes, not decrypted
- Notes confirming that each password has a unique salt

### Defensive value

This implementation protects users after a database compromise by preventing immediate exposure of their actual passwords.

---

## 4. HTTPS with Valid TLS Configuration

### Security implementation

HTTPS protects communication between a user’s browser and a website by using TLS encryption. A strong implementation uses a valid certificate, redirects HTTP traffic to HTTPS, avoids obsolete TLS versions, and applies secure headers such as HTTP Strict Transport Security.

### Why this is strong

Without HTTPS, attackers on the same network may be able to view or modify traffic. HTTPS protects usernames, passwords, session cookies, payment details, and other sensitive information while in transit.

### Security principles demonstrated

- Confidentiality
- Integrity
- Secure communication
- Protection against network interception

### Example evidence to collect

- Browser screenshot showing the secure connection indicator
- TLS scan result from an approved test website or personal domain
- Screenshot showing HTTP requests redirecting to HTTPS
- Header output showing Strict-Transport-Security where appropriate

### Defensive value

This implementation helps prevent eavesdropping, session hijacking, credential theft, and content tampering during transmission.

---

## 5. Input Validation and Output Encoding Against Injection Attacks

### Security implementation

A secure application validates input before processing it and encodes output before displaying it. For database queries, strong implementations use parameterised queries or prepared statements rather than directly joining user input into SQL commands. For web pages, output encoding reduces the risk of cross-site scripting.

### Why this is strong

Many serious vulnerabilities occur when applications trust user input. Parameterised queries prevent user input from being interpreted as SQL code. Output encoding prevents user-supplied content from being interpreted as executable script in a browser.

### Security principles demonstrated

- Secure input handling
- Safe data processing
- Injection prevention
- Secure coding practice

### Example evidence to collect

- Code snippet showing a parameterised query
- Test case showing that special characters are handled safely
- Screenshot showing that script-like input is displayed as text rather than executed
- Notes explaining the difference between validation, sanitisation, and output encoding

### Defensive value

This implementation reduces the risk of SQL injection, cross-site scripting, broken data handling, account compromise, and unauthorised data access.

---

# Summary Table

| No. | Strong security implementation | Main threat reduced | Security principle |
|---:|---|---|---|
| 1 | Multi-factor authentication | Account takeover | Defence in depth |
| 2 | Role-based access control | Unauthorised access | Least privilege |
| 3 | Salted password hashing | Password exposure after breach | Secure storage |
| 4 | HTTPS with valid TLS | Traffic interception | Confidentiality and integrity |
| 5 | Input validation and output encoding | Injection attacks | Secure coding |

---

# Reflection

These five implementations show that strong security is usually built from multiple layers rather than a single control. Authentication protects accounts, access control limits what users can do, password hashing protects stored credentials, HTTPS protects data in transit, and secure input handling reduces application-level attacks. Together, these examples demonstrate practical defensive cybersecurity principles that can be applied to web applications, cloud systems, coursework projects, and real organisational environments.
