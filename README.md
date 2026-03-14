# 🔐 OWASP Top 10:2025 — Complete Penetration Testing Checklist

[![OWASP](https://img.shields.io/badge/OWASP-Top%2010%3A2025-blue?style=flat-square&logo=owasp)](https://owasp.org/Top10/2025/)
[![CWEs](https://img.shields.io/badge/CWEs-249-red?style=flat-square)](https://cwe.mitre.org/)
[![Format](https://img.shields.io/badge/Format-Excel%20(.xlsx)-green?style=flat-square)](./OWASP_Top10_2025_Complete_249CWEs.xlsx)
[![License](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey?style=flat-square)](https://creativecommons.org/licenses/by/4.0/)

> **The missing OWASP Top 10:2025 Excel checklist.**  
> All 249 officially mapped CWEs across all 10 risk categories — each with a plain-English description, 3 real-world attack examples, actionable prevention guidance, and a ready-to-use pentest tracking layout.

---

## 📌 Why This Exists

The OWASP Top 10:2025 was released in late 2025. Unlike previous editions, the community had not yet produced a structured, CWE-complete Excel checklist for it. Most existing checklists either target the 2021 edition or are built around the OWASP Web Security Testing Guide (WSTG) test case IDs rather than CWE mappings.

This checklist fills that gap.

---

## 📊 What's Inside

The workbook contains **3 sheets**:

### 1. `OWASP Top 10 2025 Checklist` — 249 rows
The main working sheet. One row per CWE, covering all 10 categories.

| Column | Content |
|--------|---------|
| **#** | Sequential row number |
| **OWASP ID** | Category badge (A01–A10), colour-coded per category |
| **Category** | Full OWASP risk category name |
| **CWE ID** | MITRE CWE identifier |
| **CWE Name** | Official MITRE CWE weakness name |
| **Description** | Plain-English summary of the weakness and its impact |
| **Example 1** | Real-world attack scenario / proof-of-concept |
| **Example 2** | Second distinct attack variant |
| **Example 3** | Third scenario or tool-based example |
| **Prevention** | Actionable remediation and prevention guidance |
| **Status** | ☐ Not Tested / ✅ Pass / ❌ Fail / ➖ N/A |
| **Severity** | Critical / High / Medium / Low / Informational |
| **Tester Notes** | Free-text field for findings, CVEs, tool output |

### 2. `Category Summary`
Quick-reference overview of all 10 categories with CWE counts and notable CWEs.

### 3. `Legend & Instructions`
Status values, severity definitions, and reference links.

---

## 📋 Category Breakdown

| ID | Category | CWEs |
|----|----------|------|
| A01 | Broken Access Control | 40 |
| A02 | Security Misconfiguration | 16 |
| A03 | Software Supply Chain Failures | 6 |
| A04 | Cryptographic Failures | 32 |
| A05 | Injection | 37 |
| A06 | Insecure Design | 39 |
| A07 | Authentication Failures | 36 |
| A08 | Software or Data Integrity Failures | 14 |
| A09 | Security Logging and Alerting Failures | 5 |
| A10 | Mishandling of Exceptional Conditions | 24 |
| **Total** | | **249** |

---

## 🚀 How to Use

1. **Download** the `.xlsx` file from this repository
2. **Open** in Microsoft Excel, LibreOffice Calc, or Google Sheets
3. **Filter** by OWASP ID to focus on a specific category
4. **Update the Status column** as you test each item:
   - `☐ Not Tested` → starting state
   - `🔄 In Progress` → currently testing
   - `✅ Pass` → no vulnerability found
   - `❌ Fail` → vulnerability confirmed, needs remediation
   - `➖ N/A` → not applicable to the scope
5. **Add findings** in the Tester Notes column (CVE IDs, tool output, screenshots reference, remediation steps)
6. **Filter by Severity** to prioritise Critical and High findings for the report

---

## 🎯 Who This Is For

- **Penetration testers** running web application assessments
- **Security engineers** conducting internal security reviews
- **AppSec teams** performing threat modelling and design reviews
- **Bug bounty hunters** using a structured approach to coverage
- **Students and learners** studying the OWASP Top 10:2025

---

## ✅ Data Accuracy

All CWE mappings were verified directly from:
- [OWASP Top 10:2025 official category pages](https://owasp.org/Top10/2025/) — each A01–A10 page's "List of Mapped CWEs" section
- [MITRE CWE database](https://cwe.mitre.org/) — cross-referenced via the OWASP 2025 category entries (CWE-1440 through CWE-1449)

The CWE counts match the official score tables published by OWASP:

> A01:40 · A02:16 · A03:6 · A04:32 · A05:37 · A06:39 · A07:36 · A08:14 · A09:5 · A10:24 = **249 total**

---

## 📁 Repository Contents

```
├── OWASP_Top10_2025_Complete_249CWEs.xlsx   # Main checklist file
└── README.md                                 # This file
```

---

## 🤝 Contributing

Contributions are welcome. If you find a missing CWE, incorrect mapping, or want to improve the examples or prevention guidance, please:

1. Fork the repository
2. Make your changes
3. Open a Pull Request with a description of what was changed and why

For issues or suggestions, open a GitHub Issue.

---

## 📜 Attribution & License

This checklist is an independent community resource built on top of publicly available data.

- **OWASP Top 10:2025** content and category mappings are sourced from [owasp.org/Top10/2025](https://owasp.org/Top10/2025/) and are licensed under [Creative Commons Attribution 3.0 Unported](http://creativecommons.org/licenses/by/3.0/).
- **CWE names and identifiers** are sourced from [cwe.mitre.org](https://cwe.mitre.org/) and are copyright © The MITRE Corporation.
- **This checklist** (examples, descriptions, prevention guidance, formatting) is released under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to use, share, and adapt this checklist for commercial and non-commercial purposes, as long as you provide appropriate credit.

---

## ⭐ If This Helped You

If you found this useful, consider starring the repo — it helps others find it too.

---

*Data sourced from [owasp.org/Top10/2025](https://owasp.org/Top10/2025/) and [cwe.mitre.org](https://cwe.mitre.org/). This is a community resource and is not officially affiliated with OWASP or MITRE.*
