# VAPT – Web Security & Vulnerability Testing (DVWA)

Vulnerability Assessment & Penetration Testing project completed as part of the
**Cybersecurity Internship at DG Interns Hub**.

**Intern:** Avisha Masih  
**SIN:** DG/AUGUST/CYBER/098  
**Duration:** Aug 2026 – Nov 2026  
**Target Application:** DVWA (Damn Vulnerable Web Application)  
**Tools Used:** Burp Suite (Community Edition), OWASP ZAP, Kali Linux

---

## 📌 Objective
To understand and practically demonstrate common web application vulnerabilities
from the OWASP Top 10 by performing manual and automated security testing on
DVWA in an isolated lab environment.

## 🛠️ Tools Used
- **DVWA** – Intentionally vulnerable target application
- **Burp Suite Community Edition** – Manual request interception & exploitation
- **OWASP ZAP** – Automated vulnerability scanning
- **Kali Linux** – Isolated testing environment (VirtualBox)

## 🔍 Vulnerabilities Tested
| Vulnerability | Method | Risk Level |
|---|---|---|
| SQL Injection | Manual (Burp Suite) | Critical |
| XSS – Reflected | Manual (Burp Suite) | High |
| XSS – Stored | Manual (Burp Suite) | High |
| Missing Security Headers (CSP, X-Frame-Options, etc.) | Automated (OWASP ZAP) | Medium/Low |

## 📂 Repository Contents
- `VAPT_Project_Report_Avisha_Masih.pdf` – Full 15+ page project report
- `OWASP_Top10_Notes_Avisha_Masih.pdf` – Study notes on SQLi, XSS, Broken Auth, Security Misconfiguration
- `VAPT_Presentation_Avisha_Masih.pptx` – Project presentation (10 slides)
- `screenshots/` – Evidence screenshots (Burp Suite, DVWA, OWASP ZAP)

## ✅ Key Findings
- SQL Injection allowed full user-table disclosure with no authentication.
- Both Reflected and Stored XSS were successfully exploited using DVWA's XSS modules.
- OWASP ZAP's automated scan identified 9 alerts, including missing CSP and
  anti-clickjacking headers.

## 🔒 Mitigation Highlights
- Use parameterised queries to prevent SQL Injection.
- Apply output encoding and a strong Content-Security-Policy to prevent XSS.
- Configure security headers (X-Frame-Options, X-Content-Type-Options) correctly.

## ⚠️ Disclaimer
All testing was performed exclusively on a local, intentionally vulnerable
DVWA instance for educational purposes as part of an internship program.
No external or production systems were tested.
