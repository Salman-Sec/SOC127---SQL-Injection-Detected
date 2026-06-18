# SOC127---SQL-Injection-Detected
detected sql injection and investigation
# Incident Investigation Report: Event 235

## 📋 Alert Overview
* **Incident ID / Event ID:** 235
* **Alert Name:** `SOC127 - SQL Injection Detected`
* **Alert Time:** Mar, 07, 2024, 12:51 PM
* **Severity Level:** High (Security Analyst Review Required)
* **Device Action:** Allowed

---

## 🌐 Network Traffic & Direction

| Field | Value |
| :--- | :--- |
| **Source Address** | `118.194.247.28` (External Public Internet - China Unicom) |
| **Destination Address** | `172.16.20.12` (Internal Company Network) |
| **Destination Hostname** | WebServer1000 |
| **Traffic Direction** | Internet ➔ Company Network |

---

## 🛡️ Payload & Artifact Analysis

|The attacker initiated an unauthenticated `GET` request containing a heavily nested, multi-vector malicious payload:```text|
|GET /?|douj=3034%20AND%201%3D1%20UNION%20ALL%20SELECT%201%2CNULL%2C%27%3Cscript%3Ealert%28%22XSS%22%29%3C%2Fscript%3E%27%2Ctable_name%20FROM%20information_schema.tables%20WHERE%202%3E1--%2F%2A%2A%2F%3B%20EXEC%20xp_cmdshell%28%27cat%20..%2F..%2F..%2Fetc%2Fpasswd%27%29%23 HTTP/1.1|

---
##  🔍 Playbook Question Answers
* **Incident ID / Event ID:** 235
* **Alert Name:** `SOC127 - SQL Injection Detected`
* **Alert Time:** Mar, 07, 2024, 12:51 PM
* **Severity Level:** High (Security Analyst Review Required)
* **Device Action:** Allowed
.
