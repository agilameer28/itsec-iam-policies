# INTERNAL MEMO: Updated Enterprise Authentication Policy

**To:** All Employees
**From:** IT Security Operations 
**Subject:** Transition to NIST-Compliant IAM & Password Standards
**Effective Date:** Immediate

---

## 1. Overview and Purpose
To protect our corporate infrastructure against credential stuffing and brute-force attacks, we are updating our Identity and Access Management (IAM) policies to align with **NIST SP 800-63B** digital identity guidelines. 

## 2. Passphrase Requirements (Length Over Complexity)
Complex passwords (e.g., `Tr0ub4dor&3`) are difficult for humans to remember but easy for computers to crack. We are shifting to a **passphrase** model.
* **Minimum Length:** 15 characters.
* **Recommendation:** Use a sequence of 3-4 random, unrelated words (e.g., `battery-horse-staple-correct`).
* **Complexity:** We no longer mandate a mix of special characters, numbers, and uppercase letters, provided the length requirement is met.

## 3. Password Expiration 
* **Old Policy:** Mandatory password resets every 90 days.
* **New Policy:** **Abolished.** Passwords will only require changing if there is a suspected compromise or a known security breach. 

## 4. Compromised Credential Screening
All new passwords will be automatically screened against known databases of breached credentials (e.g., HaveIBeenPwned API). If your chosen passphrase has appeared in a past public data breach, the system will reject it.

## 5. Multi-Factor Authentication (MFA)
* **Mandatory:** MFA is now strictly enforced for all remote access, VPN connections, and cloud application logins (Microsoft 365 / Google Workspace). 
* **Approved Methods:** Authenticator Apps (TOTP) or Hardware Security Keys (FIDO2/WebAuthn). SMS-based 2FA is deprecated due to SIM-swapping vulnerabilities.
