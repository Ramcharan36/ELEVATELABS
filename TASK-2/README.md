# Task 2 — Phishing Email Analysis

**Student:** CHHILUMURI. SREE RAM SAI CHARAN  
**Date:** 20 Oct 2025  
**Tools:** Gmail (Show Original), MXToolbox Header Analyzer, VirusTotal (optional)

---

## 1. Sample Description
- **Source:** Public phishing sample (mock)  
- **Subject:** Urgent – Verify Your Account Now  
- **Sender Display Name:** Support Team  
- **Sender Email:** support@examp1e.com  
- **Recipient:** ramcharan@example.com  

---

## 2. Header Summary
| Field | Result |
|-------|--------|
| SPF | FAIL |
| DKIM | NONE |
| DMARC | FAIL |
| Source IP | 5.6.7.8 (Russia) |
| Return-Path Domain | examp1e.com (typo of example.com) |

---

## 3. Links and Attachments
- **Displayed Link:** https://bank.com/verify  
- **Actual URL:** http://bank-secure-verification.com/login  
- **Attachment:** None (link-based phish)

---

## 4. Phishing Indicators
| Indicator | Evidence | Risk |
|------------|-----------|------|
| Spoofed sender domain | support@examp1e.com → fake | High |
| SPF/DKIM fail | Authentication failed | High |
| Mismatched URL | Looks like bank.com → malicious domain | High |
| Urgent language | “Verify within 24 hours…” | Medium |
| Suspicious origin | IP 5.6.7.8 from RU | High |

---

## 5. Recommendations
1. Mark email as phishing and delete.  
2. Block sender domain and malicious IP.  
3. Do not click links or open attachments.  
4. Educate users about typo-domain spoofing.  
5. Enable SPF, DKIM, and DMARC for official domains.

---

## 6. Files Included
- `scan_results.txt` — full email text  
- `email_headers.txt` — raw headers  
- `header_analysis.txt` — analyzer output  
- `links.txt` — link comparison  
- `findings.csv` — structured summary  
- `screenshots/` — supporting images  

---

## 7. Conclusion
The analyzed message is a **credential-harvesting phishing email**.  
Authentication failures, spoofed domains, and urgent tone confirm malicious intent.  
Proper security controls (SPF/DKIM/DMARC, user training) can prevent similar attacks.
