# OWASP Top Ten 2021 - Summary with Examples

## Introduction

The OWASP Top Ten represents the most critical web application security risks. Below is a summary of each category with practical examples to help identify and understand these vulnerabilities.

---

## OWASP Top Ten Categories

| Category | Description | Common Examples |
|----------|-------------|-----------------|
| **A01: Broken Access Control** | Failures that allow users to perform actions beyond their permissions. | - Accessing another user’s data via IDOR (Insecure Direct Object Reference).<br>- Bypassing admin-only pages by modifying URLs.<br>- Performing actions without proper authorization checks. |
| **A02: Cryptographic Failures** | Issues with improper use or absence of encryption. | - Storing passwords in plaintext or using weak hashes (MD5, SHA1).<br>- Missing TLS, leading to data interception.<br>- Hardcoded encryption keys in source code. |
| **A03: Injection** | Inserting untrusted data that is executed as code or commands. | - SQL Injection allowing database compromise.<br>- Command Injection enabling OS command execution.<br>- Cross-Site Scripting (XSS) injecting scripts into web pages. |
| **A04: Insecure Design** | Security issues stemming from poor architecture or missing controls. | - No rate limiting on login endpoints.<br>- Missing multi-factor authentication.<br>- Insufficient input validation by design. |
| **A05: Security Misconfiguration** | Incorrect or insecure default configurations. | - Default passwords left unchanged.<br>- Debugging information exposed in production.<br>- Open cloud storage buckets accessible publicly. |
| **A06: Vulnerable and Outdated Components** | Use of libraries or frameworks with known vulnerabilities. | - Using an old jQuery version with XSS bugs.<br>- Running software with unpatched security updates.<br>- Including dependencies with known CVEs in the project. |
| **A07: Identification and Authentication Failures** | Weaknesses in verifying user identity or managing sessions. | - Allowing weak or common passwords.<br>- Missing account lockout after failed attempts.<br>- Session tokens not invalidated on logout. |
| **A08: Software and Data Integrity Failures** | Lack of integrity checks for code and infrastructure. | - Accepting unsigned updates.<br>- Using compromised third-party packages.<br>- Not verifying CI/CD pipeline security. |
| **A09: Security Logging and Monitoring Failures** | Lack of logs or monitoring that delays breach detection. | - No logging of failed login attempts.<br>- Alerts not configured for suspicious behavior.<br>- Logs stored without integrity protection. |
| **A10: Server-Side Request Forgery (SSRF)** | Server is tricked into sending unauthorized requests. | - Attacker makes server access internal-only APIs.<br>- Access to cloud metadata service via SSRF.<br>- Proxying requests to internal networks. |

---

## Usage

When assessing security, use these categories as a checklist to systematically identify vulnerabilities, understand their impact, and plan mitigations.

---

## Conclusion

Applying the OWASP Top Ten framework strengthens your security posture by focusing on the most widespread and impactful vulnerabilities.

---

