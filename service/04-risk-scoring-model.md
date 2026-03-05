# Healthcare Cybersecurity Risk Scoring Model

---

## Overview

This model provides a consistent, quantifiable method for assessing and communicating cybersecurity risk in healthcare organizations. It aligns with HIPAA Security Rule requirements and industry-standard risk management practices.

---

## Risk Score Components

### Category Weights

| Category | Weight | Rationale |
|----------|--------|-----------|
| Technical Safeguards | 40% | Primary data protection layer |
| Administrative Safeguards | 30% | Process-driven risk |
| Physical Safeguards | 15% | Often overlooked but critical |
| HIPAA Compliance | 15% | Regulatory requirement |

---

## Scoring Methodology

### Control Scoring

| Status | Points | Percentage |
|--------|--------|------------|
| Compliant | 10 | 100% |
| Partially Compliant | 5 | 50% |
| Non-Compliant | 0 | 0% |
| Not Applicable | 10 | 100% (excluded from calc) |

### Section Score Calculation

```
Section Score = (Points Earned / Points Possible) × 100
```

### Category Score Calculation

```
Category Score = (Sum of Section Scores) / (Number of Sections)
```

### Overall Risk Score Calculation

```
Overall Score = (Technical × 0.40) + (Administrative × 0.30) + 
                (Physical × 0.15) + (Compliance × 0.15)
```

---

## Risk Level Definitions

| Score Range | Risk Level | Color | Action Required |
|-------------|------------|-------|-----------------|
| 80-100% | 🟢 LOW | Green | Annual review; maintain controls |
| 60-79% | 🟡 MODERATE | Yellow | Address findings within 90 days |
| 40-59% | 🟠 HIGH | Orange | Address findings within 30 days |
| 0-39% | 🔴 CRITICAL | Red | Immediate action required |

---

## Risk Severity Classification

### Individual Finding Severity

| Severity | Criteria | Response Time |
|----------|----------|---------------|
| **CRITICAL** | Active breach, imminent threat, major HIPAA violation | Immediate (24-48 hrs) |
| **HIGH** | Significant vulnerability, likely exploitation, compliance gap | 30 days |
| **MEDIUM** | Moderate risk, potential exploitation | 90 days |
| **LOW** | Minor issue, low exploitation probability | 180 days |

### Severity Assessment Matrix

| Impact / Likelihood | Low Likelihood | Medium Likelihood | High Likelihood |
|---------------------|----------------|-------------------|-----------------|
| **Critical Impact** | HIGH | HIGH | CRITICAL |
| **High Impact** | MEDIUM | HIGH | HIGH |
| **Medium Impact** | LOW | MEDIUM | HIGH |
| **Low Impact** | LOW | LOW | MEDIUM |

---

## Finding Priority Matrix

| Priority | Score Range | Description | Timeline |
|----------|-------------|-------------|----------|
| P1 - Critical | 0-39% | Immediate remediation needed | 0-7 days |
| P2 - High | 40-59% | Significant risk, prioritize fix | 7-30 days |
| P3 - Medium | 60-79% | Standard remediation | 30-90 days |
| P4 - Low | 80-100% | Improvement opportunity | 90-180 days |

---

## Sample Score Calculation

### Example Organization: "HealthClinic XYZ"

#### Section Scores
| Section | Earned | Possible | Score |
|---------|--------|----------|-------|
| B. Administrative | 180 | 250 | 72% |
| C. Technical | 200 | 280 | 71% |
| D. Physical | 80 | 110 | 73% |

#### Category Scores
| Category | Score | Weight | Weighted |
|----------|-------|--------|----------|
| Technical | 71% | 40% | 28.4% |
| Administrative | 72% | 30% | 21.6% |
| Physical | 73% | 15% | 10.95% |
| Compliance | 65% | 15% | 9.75% |
| **OVERALL** | | | **70.7%** |

#### Risk Level: **MODERATE** 🟡

---

## Compliance Scoring

### HIPAA Security Rule Mapping

| Rule Section | Requirement | Max Points | Weight |
|--------------|-------------|------------|--------|
| 164.308(a)(1) | Risk Analysis | 10 | 10% |
| 164.308(a)(1)(ii)(B) | Risk Management | 10 | 10% |
| 164.308(a)(3) | Workforce Security | 10 | 8% |
| 164.308(a)(4) | Information Access | 10 | 8% |
| 164.308(a)(5) | Security Awareness | 10 | 8% |
| 164.308(a)(6) | Security Incident | 10 | 8% |
| 164.308(a)(7) | Contingency Plan | 10 | 8% |
| 164.310(d)(1) | Device/Media | 10 | 8% |
| 164.312(a)(1) | Access Control | 10 | 10% |
| 164.312(b) | Audit Controls | 10 | 8% |
| 164.312(c)(1) | Integrity | 10 | 6% |
| 164.312(e)(1) | Transmission Security | 10 | 8% |
| **TOTAL** | | **120** | **100%** |

### Compliance Score Calculation

```
Compliance Score = (Requirements Met / Total Requirements) × 100
```

---

## Reporting Template

### Risk Scorecard

```
╔═══════════════════════════════════════════════════════════╗
║           HEALTHCARE CYBERSECURITY RISK SCORECARD        ║
╠═══════════════════════════════════════════════════════════╣
║ Organization: [Name]                                      ║
║ Assessment Date: [Date]                                   ║
╠═══════════════════════════════════════════════════════════╣
║ OVERALL RISK SCORE:        [XX]%  [LEVEL]                ║
╠═══════════════════════════════════════════════════════════╣
║ Category Scores:                                          ║
║   Technical Safeguards:    [XX]%  ████████░░░░░           ║
║   Administrative:         [XX]%  ████████░░░░░           ║
║   Physical Safeguards:    [XX]%  ████████░░░░░           ║
║   HIPAA Compliance:       [XX]%  ████████░░░░░           ║
╠═══════════════════════════════════════════════════════════╣
║ Findings by Severity:                                     ║
║   Critical:  [X]                                          ║
║   High:      [X]                                          ║
║   Medium:    [X]                                          ║
║   Low:       [X]                                          ║
╠═══════════════════════════════════════════════════════════╣
║ Priority Remediations:                                     ║
║   1. [Finding summary]                                    ║
║   2. [Finding summary]                                    ║
║   3. [Finding summary]                                    ║
╚═══════════════════════════════════════════════════════════╝
```

---

## Remediation Effort Estimation

| Finding Complexity | Description | Estimated Hours |
|-------------------|-------------|-----------------|
| **Low** | Policy update, configuration change | 1-4 hours |
| **Medium** | New tool implementation, process change | 8-40 hours |
| **High** | Infrastructure change, system overhaul | 40-160 hours |
| **Critical** | Emergency response, major redesign | 160+ hours |

---

## Re-Assessment Guidelines

| Risk Level | Re-Assessment Frequency |
|------------|----------------------|
| CRITICAL | 30 days |
| HIGH | 90 days |
| MODERATE | 180 days |
| LOW | 12 months |

---

## Alignment Notes

This scoring model aligns with:
- NIST Cybersecurity Framework (Protect, Detect, Respond)
- HIPAA Security Rule (45 CFR 164.308)
- ISO 27001 Risk Assessment methodology
- CIS Controls v8

---

*Model Version 1.0 | Healthcare Cybersecurity Risk Assessment Service*
