# Healthcare Cybersecurity Incident Response Plan Template

## Organization Information

| Field | Details |
|-------|---------|
| Organization Name | ________________________________ |
| Document Version | ________________________________ |
| Effective Date | ________________________________ |
| Review Date | ________________________________ |
| Document Owner | ________________________________ |

---

## 1. Purpose & Scope

### 1.1 Purpose
This Incident Response Plan establishes procedures for detecting, responding to, and recovering from cybersecurity incidents that affect the confidentiality, integrity, or availability of Protected Health Information (PHI) and organizational information systems.

### 1.2 Scope
This plan applies to:
- All employees, contractors, and workforce members
- All information systems that store, process, or transmit PHI
- All locations and facilities
- All devices including workstations, servers, mobile devices, and medical devices

### 1.3 Incident Types Covered
- ☐ Data breach / Unauthorized disclosure of PHI
- ☐ Ransomware or malware infection
- ☐ Phishing attack resulting in credential compromise
- ☐ Denial of Service (DoS/DDoS)
- ☐ Unauthorized access to systems or data
- ☐ Lost or stolen device
- ☐ Insider threat
- ☐ Physical security breach
- ☐ Medical device cybersecurity incident
- ☐ Other: _______________________

---

## 2. Incident Response Team

### 2.1 Core Team Members

| Role | Name | Contact (Primary) | Contact (Backup) |
|------|------|-------------------|------------------|
| Incident Response Manager | _________________ | _________________ | _________________ |
| IT Security Lead | _________________ | _________________ | _________________ |
| Privacy Officer | _________________ | _________________ | _________________ |
| Legal Counsel | _________________ | _________________ | _________________ |
| HR Representative | _________________ | _________________ | _________________ |
| Communications Lead | _________________ | _________________ | _________________ |
| Executive Sponsor | _________________ | _________________ | _________________ |

### 2.2 External Contacts

| Service | Provider | Contact Number | Account Info |
|---------|----------|----------------|--------------|
| Cybersecurity Insurance | _________________ | _________________ | _________________ |
| Incident Response Firm | _________________ | _________________ | _________________ |
| Legal Counsel | _________________ | _________________ | _________________ |
| Law Enforcement (FBI IC3) | _________________ | _________________ | N/A |
| HHS OCR | _________________ | 1-800-368-8001 | www.hhs.gov/breach |
| Media Contact | _________________ | _________________ | _________________ |

---

## 3. Incident Classification

### 3.1 Severity Levels

| Level | Description | Response Time | Examples |
|-------|-------------|---------------|----------|
| **Level 1 - Critical** | Confirmed breach of 500+ PHI records | Immediate | Ransomware, data exfiltration |
| **Level 2 - High** | Confirmed breach of <500 PHI records | Within 4 hours | Phishing with credentials, malware |
| **Level 3 - Medium** | Attempted attack, no PHI compromised | Within 24 hours | Blocked intrusion attempt |
| **Level 4 - Low** | Policy violation, no security impact | Within 72 hours | Failed login attempts, minor issues |

### 3.2 Incident Categories

| Category | Code | Description |
|----------|------|-------------|
| Confidentiality Breach | INC-CB | Unauthorized access/disclosure of PHI |
| Integrity Breach | INC-IB | Unauthorized modification of data |
| Availability Breach | INC-AB | System/service disruption |
| Malware | INC-MW | Malicious software infection |
| Phishing | INC-PH | Social engineering attack |
| Insider Threat | INC-IT | Malicious internal actor |
| Physical Security | INC-PS | Physical facility breach |
| Medical Device | INC-MD | Medical equipment compromise |

---

## 4. Incident Response Procedures

### Phase 1: DETECTION & IDENTIFICATION

#### 4.1 Detection Methods
- [ ] Intrusion Detection System (IDS) alert
- [ ] Security Information & Event Management (SIEM) alert
- [ ] Antivirus/EDR alert
- [ ] User report
- [ ] Third-party notification
- [ ] Log analysis
- [ ] Network monitoring
- [ ] Other: _______________________

#### 4.2 Initial Assessment Checklist

| # | Action | Completed | Notes |
|---|--------|-----------|-------|
| 1 | Document date/time of initial detection | ☐ | _________________ |
| 2 | Identify who detected the incident | ☐ | _________________ |
| 3 | Document initial indicators of compromise | ☐ | _________________ |
| 4 | Determine scope - systems/data affected | ☐ | _________________ |
| 5 | Assign preliminary severity level | ☐ | _________________ |
| 6 | Create incident case number | ☐ | Case #: ________ |
| 7 | Notify Incident Response Manager | ☐ | _________________ |
| 8 | Preserve evidence (screenshots, logs) | ☐ | _________________ |

#### 4.3 Initial Detection Form

```
INCIDENT DETECTION FORM
========================
Date/Time Detected: _______________
Detected By: _______________________
Detection Method: __________________
Systems Affected: __________________
Data Potentially Affected: _________
Estimated Records Affected: ________
Severity Level: ☐ Critical ☐ High ☐ Medium ☐ Low
Initial Description:
_________________________________________________
_________________________________________________
```

---

### Phase 2: CONTAINMENT

#### 4.4 Short-Term Containment (Immediate)

| # | Action | Completed | Performed By |
|---|--------|-----------|--------------|
| 1 | Isolate affected systems from network | ☐ | _________________ |
| 2 | Block malicious IP addresses/domains | ☐ | _________________ |
| 3 | Disable compromised accounts | ☐ | _________________ |
| 4 | Revoke access tokens/sessions | ☐ | _________________ |
| 5 | Preserve volatile evidence (memory) | ☐ | _________________ |
| 6 | Document all actions taken | ☐ | _________________ |

#### 4.5 Long-Term Containment

| # | Action | Completed | Performed By |
|---|--------|-----------|--------------|
| 1 | Analyze malware/vulnerabilities | ☐ | _________________ |
| 2 | Patch affected systems | ☐ | _________________ |
| 3 | Reset credentials for affected users | ☐ | _________________ |
| 4 | Implement additional monitoring | ☐ | _________________ |
| 5 | Review and strengthen access controls | ☐ | _________________ |
| 6 | Update firewall/IDS rules | ☐ | _________________ |

---

### Phase 3: INVESTIGATION & ANALYSIS

#### 4.6 Root Cause Analysis

| # | Question | Answer |
|---|----------|--------|
| 1 | How did the attacker gain initial access? | _____________________________ |
| 2 | What vulnerability was exploited? | _____________________________ |
| 3 | What systems were compromised? | _____________________________ |
| 4 | What data was accessed/exfiltrated? | _____________________________ |
| 5 | How long did the attacker have access? | _____________________________ |
| 6 | What was the attack vector? | _____________________________ |
| 7 | Were there any warning signs? | _____________________________ |
| 8 | Could this have been prevented? How? | _____________________________ |

#### 4.7 Evidence Log

| # | Evidence Type | Description | Collected By | Date/Time | Hash |
|---|---------------|-------------|--------------|-----------|-----|
| 1 | _________________ | _________________ | ____________ | _________ | ____ |
| 2 | _________________ | _________________ | ____________ | _________ | ____ |
| 3 | _________________ | _________________ | ____________ | _________ | ____ |
| 4 | _________________ | _________________ | ____________ | _________ | ____ |
| 5 | _________________ | _________________ | ____________ | _________ | ____ |

#### 4.8 Impact Assessment

| Assessment Area | Findings |
|-----------------|----------|
| Number of PHI records potentially affected | _________________ |
| Types of PHI involved | ☐ Demographic ☐ Medical ☐ Billing ☐ Insurance |
| Number of patients affected | _________________ |
| Geographic scope | ☐ Single facility ☐ Multiple facilities ☐ Regional |
| Regulatory implications | ☐ HIPAA ☐ State laws ☐ Contractual |
| Financial impact estimate | $ _________________ |

---

### Phase 4: NOTIFICATION & COMMUNICATION

#### 4.9 Internal Notification Checklist

| # | Stakeholder | Notified | Date/Time | Method | Contact |
|---|-------------|----------|-----------|--------|---------|
| 1 | Incident Response Team | ☐ | _________ | ________ | _______ |
| 2 | Executive Leadership | ☐ | _________ | ________ | _______ |
| 3 | Legal Counsel | ☐ | _________ | ________ | _______ |
| 4 | IT Department | ☐ | _________ | ________ | _______ |
| 5 | HR Department | ☐ | _________ | ________ | _______ |
| 6 | Privacy Officer | ☐ | _________ | ________ | _______ |
| 7 | Department Heads | ☐ | _________ | ________ | _______ |

#### 4.10 External Notification Requirements

| # | Entity | Required | Deadline | Notified | Date |
|---|--------|----------|----------|----------|------|
| 1 | HHS OCR (if >500 records) | ☐ Yes ☐ No | 60 days | ☐ | ________ |
| 2 | Affected Individuals | ☐ Yes ☐ No | Without unreasonable delay | ☐ | ________ |
| 3 | Media (if >500 records) | ☐ Yes ☐ No | Immediately | ☐ | ________ |
| 4 | State Attorney General | ☐ Yes ☐ No | Per state law | ☐ | ________ |
| 5 | Insurance Carrier | ☐ Yes ☐ No | Per policy | ☐ | ________ |
| 6 | Business Associates | ☐ Yes ☐ No | Per contract | ☐ | ________ |
| 7 | Law Enforcement | ☐ Yes ☐ No | As appropriate | ☐ | ________ |

#### 4.11 Sample Individual Notification Letter
*(Attach actual letter to this plan)*

---

### Phase 5: RECOVERY

#### 4.12 Recovery Checklist

| # | Action | Completed | Date | Performed By |
|---|--------|-----------|------|--------------|
| 1 | Verify threat has been eliminated | ☐ | _________ | _________________ |
| 2 | Restore systems from clean backups | ☐ | _________ | _________________ |
| 3 | Apply all security patches | ☐ | _________ | _________________ |
| 4 | Reset all credentials | ☐ | _________ | _________________ |
| 5 | Verify system functionality | ☐ | _________ | _________________ |
| 6 | Confirm security controls working | ☐ | _________ | _________________ |
| 7 | Monitor for repeat indicators | ☐ | _________ | _________________ |
| 8 | Resume normal operations | ☐ | _________ | _________________ |

#### 4.13 Post-Recovery Validation

| Test | Result | Date | Tester |
|------|--------|------|--------|
| Network connectivity | ☐ Pass ☐ Fail | _________ | _______ |
| User authentication | ☐ Pass ☐ Fail | _________ | _______ |
| Data integrity | ☐ Pass ☐ Fail | _________ | _______ |
| Application functionality | ☐ Pass ☐ Fail | _________ | _______ |
| Logging/alerting | ☐ Pass ☐ Fail | _________ | _______ |

---

### Phase 6: POST-INCIDENT REVIEW

#### 4.14 Lessons Learned Meeting

| Item | Details |
|------|---------|
| Meeting Date | _________________ |
| Attendees | _________________ |
| Incident Summary | ________________________________ |
| What went well | ________________________________ |
| What needs improvement | ________________________________ |
| Action items for future | ________________________________ |

#### 4.15 Improvement Action Items

| # | Improvement Area | Action Item | Owner | Due Date | Status |
|---|------------------|-------------|-------|----------|--------|
| 1 | _________________ | _________________ | _______ | _________ | ☐ Open ☐ Complete |
| 2 | _________________ | _________________ | _______ | _________ | ☐ Open ☐ Complete |
| 3 | _________________ | _________________ | _______ | _________ | ☐ Open ☐ Complete |
| 4 | _________________ | _________________ | _______ | _________ | ☐ Open ☐ Complete |
| 5 | _________________ | _________________ | _______ | _________ | ☐ Open ☐ Complete |

---

## 5. Incident Documentation Summary

### Complete this for each incident

```
INCIDENT SUMMARY
================
Incident #: _________
Date/Time Discovered: _____________
Date/Time Contained: ______________
Date/Time Resolved: ________________

Severity: ☐ Critical ☐ High ☐ Medium ☐ Low
Category: _________________________

Impact:
- Records affected: ________________
- Downtime: ________________________
- Financial impact: $ ______________

Root Cause: ________________________

Lessons Learned:
___________________________________
___________________________________

Recommendations:
___________________________________
___________________________________
```

---

## 6. Plan Maintenance

| Review Type | Frequency | Last Review | Next Review | Approved By |
|-------------|-----------|-------------|-------------|-------------|
| Full Plan Review | Annually | _____________ | _____________ | ____________ |
| Contact Update | Quarterly | _____________ | _____________ | ____________ |
| Tabletop Exercise | Bi-annually | _____________ | _____________ | ____________ |
| After Incident | As needed | N/A | N/A | N/A |

---

## 7. Sign-Off

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Incident Response Manager | _________________ | _____________ | ________ |
| IT Security Lead | _________________ | _____________ | ________ |
| Privacy Officer | _________________ | _____________ | ________ |
| Executive Sponsor | _________________ | _____________ | ________ |

---

**Document Control**
- Version: _________________
- Last Updated: _________________
- Next Review: _________________

*This template is for educational purposes. Consult with a qualified HIPAA compliance expert and legal counsel for full implementation.*

---
© 2026 Healthcare Cybersecurity Toolkit - For Educational Use Only
