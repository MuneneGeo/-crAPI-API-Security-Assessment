Security assessment of OWASP crAPI (Completely Ridiculous API) — a deliberately vulnerable REST API application designed to demonstrate real-world API security weaknesses. Conducted by Squad 4 as part of the AfricaHackon Cybersecurity Program.

## 🎯 Assessment Objective
Identify and document security weaknesses in REST API endpoints using manual and automated testing techniques.

## 🔴 Key Vulnerabilities Found
- IDOR (API1) — Accessing other users' orders by modifying object IDs in GET requests
- Broken Authentication — Unauthenticated access to protected API endpoints
- Excessive Data Exposure — API responses returning sensitive fields not required by the client
- Business Logic Flaws — Abusing application functionality to perform unauthorised actions
- Missing Rate Limiting — Enumeration and scraping of user data at scale
- Mass Assignment — Setting unauthorised fields through API request body manipulation
- JWT Vulnerabilities — Token validation weaknesses enabling privilege escalation

## 🛠️ Tools Used
Burp Suite | Postman | Browser DevTools | Docker | OWASP API Top 10 Framework

## 📄 Full Report
See `reports/crAPI_API_Security_Report.pdf` for all findings with proof-of-concept requests, responses, and remediation recommendations.

## ⚠️ Disclaimer
Testing was conducted solely against the OWASP crAPI lab environment for educational purposes. No real systems were targeted.
