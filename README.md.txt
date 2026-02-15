# Cyber Security Task 1 – Vulnerability Assessment Report

## Internship

Future Interns – Cyber Security Track

---

## Target Website

http://demo.testfire.net

---

## Scope of Assessment

This assessment was conducted using a **read-only and passive approach**.
No exploitation, brute force, or harmful activity was performed.

The analysis included:

* Public pages only
* Port exposure analysis
* Security header inspection
* Information disclosure review

---

## Tools Used

* Nmap (Port Scanning)
* Browser Developer Tools (Header Inspection)

---

## Findings

### 1. Open HTTP Port (80) – High Risk

The website allows unencrypted communication over HTTP.
Sensitive data may be intercepted by attackers.

**Recommendation:** Redirect all traffic to HTTPS and disable HTTP access.

---

### 2. Missing Security Headers – Medium Risk

Important browser security protections are not configured.

**Recommendation:** Implement headers such as:

* Content-Security-Policy
* X-Frame-Options
* Strict-Transport-Security
* X-Content-Type-Options

---

### 3. Server Information Disclosure – Low Risk

The server reveals software details in response headers.

**Recommendation:** Hide server version information.

---

## Conclusion

The website contains security misconfigurations that could expose users to risk.
Implementing HTTPS and proper security headers will significantly improve security posture.

---

## Ethical Statement

This assessment followed responsible disclosure practices and respected the defined scope.
No active attacks or exploitation were performed.

---

## Repository Contents

* Report.pdf → Final vulnerability assessment report
* Evidence/ → Screenshots of findings
