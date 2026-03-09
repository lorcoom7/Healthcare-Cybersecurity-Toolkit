# Password Policy

## Healthcare Organization: _____________________________

---

## 1. Purpose

This Password Policy establishes requirements for creating, managing, and protecting passwords to secure access to information systems and Protected Health Information (PHI) in compliance with HIPAA Security Rule.

## 2. Scope

This policy applies to:
- All employees, contractors, and workforce members
- All systems accessing organizational data
- All password-protected resources

---

## 3. Password Requirements

### 3.1 Password Complexity

| Requirement | Standard |
|-------------|----------|
| Minimum Length | 12 characters |
| Complexity | Must include 3 of 4: uppercase, lowercase, numbers, special characters |
| History | Cannot reuse last 12 passwords |
| Maximum Age | 90 days |

### 3.2 Prohibited Passwords

- ☐ Employee name or username
- ☐ Company name
- ☐ Dictionary words
- ☐ Personal information (birthdays, addresses)
- ☐ Sequential characters (123456, qwerty)
- ☐ Previously compromised passwords

---

## 4. Account Lockout

| Parameter | Setting |
|-----------|---------|
| Failed attempts | 5 attempts |
| Lockout duration | 30 minutes |
| Admin unlock | Required after 3 lockouts |

---

## 5. Multi-Factor Authentication (MFA)

### 5.1 MFA Required For

| System/Access | MFA Required |
|---------------|--------------|
| VPN access | ☐ Yes ☐ No |
| Remote desktop | ☐ Yes ☐ No |
| Email (external) | ☐ Yes ☐ No |
| EHR systems | ☐ Yes ☐ No |
| Administrative accounts | ☐ Yes ☐ No |
| Cloud services | ☐ Yes ☐ No |

### 5.2 Approved MFA Methods

- [ ] Authenticator app (Microsoft, Google, Duo)
- [ ] Hardware token (YubiKey, RSA)
- [ ] SMS/Voice (backup only)
- [ ] Biometric + PIN

---

## 6. Password Change Schedule

| Account Type | Change Frequency |
|--------------|------------------|
| Standard users | Every 90 days |
| Privileged accounts | Every 60 days |
| Service accounts | Every 180 days |
| After security incident | Immediately |

---

## 7. Password Storage & Transmission

| Requirement | Standard |
|-------------|----------|
| Storage | Hash + salt only |
| Transmission | TLS/SSL required |
| Display | Masked by default |
| Sharing | Prohibited |

---

## 8. Service Account Management

| # | Requirement | Compliant |
|---|-------------|-----------|
| 1 | Unique service accounts per application | ☐ Yes ☐ No |
| 2 | Complex passwords (25+ chars) | ☐ Yes ☐ No |
| 3 | Documented in password vault | ☐ Yes ☐ No |
| 4 | Regular rotation schedule | ☐ Yes ☐ No |
| 5 | Access limited to required personnel | ☐ Yes ☐ No |

---

## 9. Password Vault

### 9.1 Password Vault Requirements

| Feature | Required |
|---------|----------|
| Encrypted storage | ☐ Yes |
| MFA for access | ☐ Yes |
| Audit logging | ☐ Yes |
| Share access feature | ☐ Yes |
| Auto-generate passwords | ☐ Yes |

---

## 10. Password Construction Guide

### Recommended Methods

| Method | Example |
|--------|---------|
| Passphrase (3 random words) | Correct-Horse-Battery-Staple |
| Abbreviated sentence | ILuP@S2day! |
| Password generator | Xk9#mP2$vL8qN |

### Creating a Strong Password Steps:
1. Choose 3 random words (at least 6 letters each)
2. Add uppercase to first letter
3. Add a special character
4. Add a number
5. Example: 🌵Banana🎸Pizza🌟 → BananaPizza2024!

---

## 11. Prohibited Practices

- ☐ Writing passwords on paper
- ☐ Sharing passwords with anyone
- ☐ Storing passwords in plain text
- ☐ Sending passwords via email/chat
- ☐ Using same password across systems
- ☐ Storing in browser (except with master password)
- ☐ Using personal information in passwords

---

## 12. Incident Response

### Compromised Password Response

| # | Action | Completed |
|---|--------|-----------|
| 1 | Force password change | ☐ |
| 2 | Review account activity | ☐ |
| 3 | Check for unauthorized access | ☐ |
| 4 | Enable MFA if not active | ☐ |
| 5 | Document incident | ☐ |
| 6 | Report to security team | ☐ |

---

## 13. Compliance Checklist

| Requirement | Implemented | Date |
|-------------|-------------|------|
| Password complexity enabled | ☐ | _________ |
| Account lockout configured | ☐ | _________ |
| MFA for privileged accounts | ☐ | _________ |
| Password vault deployed | ☐ | _________ |
| User training completed | ☐ | _________ |
| Password policy communicated | ☐ | _________ |

---

## Policy Acknowledgment

| Employee Name | Signature | Date |
|---------------|-----------|------|
| _________________ | _____________ | ________ |
| _________________ | _____________ | ________ |
| _________________ | _____________ | ________ |
| _________________ | _____________ | ________ |

---

**Version:** _________________ | **Effective Date:** _________________ | **Review Date:** _________________

*This template is for educational purposes.*
