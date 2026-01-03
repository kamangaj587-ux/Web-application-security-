# Web-application-security-
# Web Application Security Lab – OWASP ZAP Scan

## 🔎 Workflow
1. **Setup**
   - Installed and launched OWASP ZAP.
   - Configured browser proxy to route traffic through ZAP.
   - Selected target web application for testing.

2. **Scanning**
   - Ran the **Spider tool** to crawl the application.
   - Conducted an **Active Scan** to identify vulnerabilities.
   - Exported results into ZAP’s HTML report.

3. **Analysis**
   - Reviewed findings, categorized by severity (High, Medium, Low).
   - Verified potential false positives.

---

## 📝 Findings
- **Cross-Site Scripting (XSS)** – Input fields not properly sanitized.
- **SQL Injection (SQLi)** – Detected in login form query parameters.
- **Missing Security Headers** – No `Content-Security-Policy` or `X-Frame-Options`.
- **Insecure Cookies** – Session cookies missing `HttpOnly` and `Secure` flags.

---

## 🛠️ Remediation Notes
- **XSS** → Implement input validation and output encoding.
- **SQLi** → Use parameterized queries and ORM frameworks.
- **Headers** → Add CSP, X-Frame-Options, and Strict-Transport-Security.
- **Cookies** → Configure secure attributes to prevent hijacking.

---

## 📚 Lessons Learned
- Even simple applications can expose critical vulnerabilities.
- Automated scans are powerful but require manual verification.
- Security is a continuous process, not a one-time fix.

---

## 📌 Next Steps
- Apply fixes and re-run scans.
- Document improvements in follow-up commits.
- Share reflections on LinkedIn/Medium for professional growth.
