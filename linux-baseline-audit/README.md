# Linux Baseline Compliance Audit (AWS EC2 Lab)

## 📌 Overview
This project simulates a baseline compliance audit on a cloud-hosted Ubuntu server.  
It demonstrates technical hardening, patch management, and audit evidence collection as part of GRC engineering.

The goal: connect **hands-on system administration** with **governance, risk, and compliance (GRC) controls**.

---

## 🛠️ Tools & Skills
- **AWS EC2** (Ubuntu 22.04 LTS Free Tier)
- **SSH Key Authentication** (secure remote login)
- **Patch Management** (`apt update/upgrade`, `autoremove`, kernel reboot)
- **Baseline Audit** (Lynis security scanner)
- **Evidence Collection** (`scp`, audit logs, structured documentation)
- **Audit Reporting** (interpreting technical findings in plain English)

---

## 📂 Project Structure

<pre><code>linux-baseline-audit/
├── README.md
├── evidence/
│   ├── autoremove-log.txt
│   ├── kernel-version-log.txt
│   └── lynis-report.txt
└── docs/
    └── findings.md
</code></pre>
---

## 🔎 Key Findings
- **Root login permitted via SSH** → Increases chance of brute-force or unauthorized access.  
- **Weak password policy** → Allows short/simple passwords, easier to crack.  
- **Firewall not configured** → All ports potentially exposed to the internet.  

---

## 🎯 GRC Relevance
This lab connects **technical actions** (patching, hardening, auditing) with **governance controls** such as:  
- Patch Management  
- Identity & Access Management (IAM)  
- Configuration Baseline Testing  
- Audit Evidence Handling  

It demonstrates how auditors gather, interpret, and preserve evidence securely — skills that bridge IT operations with GRC engineering.

---

## ✅ Next Steps
- Apply recommended hardening changes (disable root login, enforce stronger password policy, configure firewall).  
- Re-run Lynis and compare the hardening index for improvement.  
- Extend this workflow to additional projects (SSH hardening lab, firewall configuration lab, IAM controls lab).

