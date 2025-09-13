# Findings from Baseline Audit

## 1. Root login permitted via SSH
- **Risk**: Increases chance of brute-force or unauthorized access.
- **Recommendation**: Set `PermitRootLogin no` in `/etc/ssh/sshd_config`.

## 2. Weak password policy
- **Risk**: Allows short/simple passwords, easier to crack.
- **Recommendation**: Enforce 12+ character minimum using PAM.

## 3. Firewall not configured
- **Risk**: All ports potentially exposed to the internet.
- **Recommendation**: Enable and configure `ufw` or iptables.

---

**Next Steps**: Address findings, re-run Lynis, compare hardening index improvements.

