# Project 2 — Secure Configuration & Baseline Drift

**Goal:** Simulate an IT audit of Linux server configurations by checking actual settings against a defined security baseline.  
**Why it matters:** In real audits, we don’t just say “secure or insecure” — we measure systems against a **baseline policy** (the yardstick) and document gaps with risk ratings and remediation recommendations.

---

## 🎯 Objectives
- Define a **baseline security policy** (password rules, root login, log retention).
- Compare two sample servers (`server1.txt`, `server2.txt`) against this baseline.
- Identify **PASS/FAIL results** with **High/Medium risk ratings**.
- Produce an **audit-style findings report** with clear remediation steps.

---

## 🗂 Project Structure
- **baseline.txt** → Policy requirements (yardstick for compliance).  
- **server1.txt** → Mostly compliant server (1 medium risk gap).  
- **server2.txt** → Non-compliant server with multiple high risks.  
- **report.md** → Audit report with findings, risk ratings, and recommendations.  

---

## ✅ Key Learnings Demonstrated
- **Control Testing:** Measured actual settings against baseline requirements.  
- **Risk Assessment:** Rated findings (High/Medium) based on potential impact.  
- **Audit Reporting:** Documented results in a clear, actionable report.  
- **Communication:** Explained *why* each failed control matters in plain English.  

---

## 📋 Sample Findings (from report.md)

### Server1
- Password length: PASS  
- Root login: PASS  
- Logs: **FAIL** (21 < 30) → *Medium risk*  

> **Recommendation:** Increase log retention to 30 days.  

### Server2
- Password length: **FAIL** (8 < 12) → *Medium risk*  
- Root login: **FAIL** (enabled) → *High risk*  
- Logs: **FAIL** (0 < 30) → *High risk*  

> **Recommendation:** Disable root login, enforce stronger passwords, enable logging.  

---

## 📂 How to Navigate
- Start with `baseline.txt` to see the “policy.”  
- Review `server1.txt` and `server2.txt` to compare evidence.  
- Open `report.md` for the final audit findings and recommendations.  

---

*This project mirrors how IT auditors and GRC analysts test system configurations: define baseline → collect evidence → analyze gaps → communicate risks and fixes.*

