# Configuration Drift Report

This report compares two servers (server1, server2) against the baseline security policy.

---

## Server1 (mostly compliant)
- Password length: **PASS** (12 ≥ 12)  
- Root login: **PASS** (NO)  
- Logs: **FAIL** (21 < 30) → Medium risk  

**Summary:** Server1 is largely compliant with baseline standards. The only gap is log retention (21 days vs 30). This reduces ability to investigate security incidents fully.  

**Recommendation:** Increase log retention to at least 30 days.  

---

## Server2 (non-compliant)
- Password length: **FAIL** (8 < 12) → Medium risk  
- Root login: **FAIL** (YES) → High risk  
- Logs: **FAIL** (0 < 30) → High risk  

**Summary:** Server2 fails across all critical areas. Short passwords increase likelihood of compromise, root login creates a direct path to full system control with no accountability, and no logs means incidents cannot be investigated.  

**Recommendations:**  
1. Enforce 12+ character password policy.  
2. Disable root login and require named accounts + sudo.  
3. Configure log retention for 30+ days.  

---

## Overall Assessment
- Server1: Medium risk finding  
- Server2: Multiple High risk findings  

**Conclusion:** Immediate remediation is required on Server2 to reduce exposure to unauthorized access and data loss. Server1 needs log retention adjusted to meet baseline.  
