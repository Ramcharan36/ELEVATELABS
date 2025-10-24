# Task 3: Basic Vulnerability Scan on PC

## Objective
Perform a basic vulnerability assessment on a personal computer using free vulnerability scanning tools to identify common security risks and understand mitigation steps.

---

## Tool Used
- **Nessus Essentials** (Free version)  
- Version: 10.8.x  
- Scan Type: **Basic Network Scan**

---

## Scan Configuration
- **Scan Name:** PC Vulnerability Scan  
- **Target:** `localhost` or `<Your PC IP>`  
- **Scan Type:** Full system scan  
- **Credentialed Scan:** No (optional: Yes, for patch auditing)  
- **Duration:** ~30–60 minutes  

---

## Scan Results
### Vulnerabilities Summary
| Severity       | Count |
|----------------|-------|
| Critical       |       |
| High           |       |
| Medium         |       |
| Low            |       |

> Add a screenshot of the overall summary here  
`![Scan Summary](screenshots/summary.png)`

### Critical / High Vulnerabilities
| Vulnerability Name | Severity | Description | Recommended Fix | Screenshot |
|-------------------|---------|-------------|----------------|-----------|
|                   |         |             |                | ![vuln1](screenshots/critical1.png) |
|                   |         |             |                | ![vuln2](screenshots/critical2.png) |
|                   |         |             |                | ![vuln3](screenshots/critical3.png) |

---

## Mitigation Steps
- Apply software patches and updates for all identified vulnerabilities.  
- Disable unnecessary services or open ports.  
- Update antivirus and system security settings.  
- Follow Nessus recommendations for each critical/high vulnerability.

---

## Conclusion
- Completed a full vulnerability scan on the local PC.  
- Identified critical, high, medium, and low-severity vulnerabilities.  
- Documented mitigation steps for critical issues.  
- Gained introductory experience in vulnerability assessment and risk prioritization.

---

## Notes
- **Frequency of scans:** Monthly or after major updates.  
- **CVSS (Common Vulnerability Scoring System)** used for severity assessment.  
- **False Positives:** Some reported vulnerabilities may not be applicable; verify before remediation.

---

## Screenshots
Place all scan result screenshots in a folder called `screenshots` in the repo.  
Example: `screenshots/summary.png`, `screenshots/critical1.png`

---
