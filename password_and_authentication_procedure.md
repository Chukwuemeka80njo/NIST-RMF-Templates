# Password & Authentication Procedure  
**File:** password_and_authentication_procedure.md  
**Category:** Procedures  
**Related Policies:** Identification & Authentication Policy, Access Control Policy  
**Mapped NIST Controls:** IA-2, IA-4, IA-5, IA-8, AC-2, AC-17  

---

## 1. Purpose  
This procedure defines the required steps for secure password creation, authentication controls, credential lifecycle management, and multi-factor authentication (MFA). It ensures compliance with NIST 800-53 authentication expectations.

---

## 2. Scope  
This procedure applies to:  
- All employees, contractors, and third-party users  
- All systems, applications, and cloud platforms requiring authentication  
- Enterprise identity and access management (IAM) systems  
- Privileged accounts and administrative access  

---

## 3. Definitions  

**Password:** A confidential string used to authenticate a user.  
**Authentication:** Verification of identity using passwords, MFA, tokens, and other mechanisms.  
**MFA (Multi-Factor Authentication):** Authentication using two or more factors (knowledge, possession, inherence).  
**Credential:** Passwords, tokens, certificates, and authentication secrets.  

---

## 4. Procedure  

### 4.1 Password Creation Requirements  
1. Minimum length: **14 characters**  
2. Must include at least **three** of the following:  
   - Uppercase letter  
   - Lowercase letter  
   - Number  
   - Special character  
3. Passwords must NOT contain:  
   - Dictionary words  
   - Personal information  
   - Previously used passwords  
4. Default passwords must be changed immediately upon first login.

---

### 4.2 Multi-Factor Authentication (MFA)  
MFA is required for:  
- Remote access / VPN  
- Administrative access  
- Cloud platforms  
- Systems containing sensitive data (Finance, HR, PII, etc.)

Approved MFA methods:  
- Time-based one-time passwords (TOTP)  
- Hardware tokens  
- Mobile authenticator applications  
- Push authentication  

---

### 4.3 Password Storage & Transmission  
1. Passwords must never be stored or transmitted in cleartext.  
2. Systems must store passwords using:  
   - Salted hashing (PBKDF2, bcrypt, scrypt, Argon2)  
3. Password files and credential stores must be encrypted.  
4. Users may not share passwords under any circumstances.

---

### 4.4 Password Change & Reset  
1. Users must change passwords immediately if compromise is suspected.  
2. Password resets require identity verification through one of the following:  
   - In-person verification  
   - Ticket-based identity challenge  
   - MFA-based recovery  
3. Temporary reset passwords must expire within **24 hours**.  
4. Administrators may not reuse previously issued temporary passwords.

---

### 4.5 Account Lockout  
1. Accounts must lock after **10 invalid login attempts**.  
2. Locked accounts require administrative reset.  
3. Authentication events must be logged and monitored for anomalies.

---

### 4.6 Credential Protection Requirements  
- Users must not write passwords down or store them in unsecured locations.  
- Password vaults must be approved by the ISO.  
- API keys, service accounts, and certificates must be rotated regularly.

---

## 5. Responsibilities  

### Users  
- Maintain secure passwords  
- Protect authentication information  
- Report suspected compromise immediately  

### System Administrators  
- Enforce password policy settings  
- Configure MFA systems  
- Monitor authentication logs  

### Information Security Officer (ISO)  
- Review authentication controls annually  
- Approve exceptions or waivers  

---

## 6. Enforcement  
Failure to follow this procedure may result in disciplinary action and removal of system access.

---

## 7. Review  
This procedure must be reviewed **annually** or after major system or policy changes.

