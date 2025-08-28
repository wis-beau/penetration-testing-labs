# 🛡️ Penetration Testing Lab — Learning Log (Metasploitable 2)

This repository documents a hands-on **penetration testing lab** performed against **Metasploitable 2** from a Kali Linux attacker VM on an isolated Host‑Only network. The focus is on the early lifecycle stages: **reconnaissance → scanning → service enumeration → analysis**. Evidence and outputs are kept in plain text for transparency and easy review.

> **Scope & Ethics**: This lab ran entirely in a closed, local environment on intentionally vulnerable targets. Do **not** use these techniques on systems you do not own or have explicit authorization to test.

---

## 📂 Repository Layout

```
penetration-testing-labs/
├── README.md
├── 01-open-port-scanning/
│   ├── README.md
│   ├── nmap-scan-full.txt
│   ├── nmap-scan-detailed.txt
│   └── summary-table.md
├── 02-service-enumeration/
│   ├── README.md
│   ├── netcat-banners.txt
│   ├── telnet-banners.txt
│   └── vsftpd-version.txt
├── 03-analysis-findings/
│   ├── README.md
│   ├── vulnerabilities.md
│   └── remediation-ideas.md
└── references/
    ├── README.md
    ├── assignment-brief.md
    └── bibliography.md
```

---

## 🎯 Objectives

- Identify **open ports** and **running services** on Metasploitable 2.
- Enumerate **service versions** to map potential vulnerabilities.
- Capture **banner evidence** (e.g., `vsftpd 2.3.4`) for verification.
- Summarize **initial risks** and propose **remediation ideas**.

## 🛠️ Tools

- `nmap` for host discovery, full‑port scans and service detection.
- `netcat` & `telnet` for manual banner grabbing / verification.

---

## 🔗 Where to Look

- **Scanning commands & raw outputs** → [`01-open-port-scanning/`]([./01-open-port-scanning](https://github.com/wis-beau/penetration-testing-labs/tree/main/penetration-testing-labs/01-open-port-scanning))
- **Banner grabs & version notes** → [`02-service-enumeration/`](./02-service-enumeration)
- **Findings & mitigations** → [`03-analysis-findings/`](./03-analysis-findings)
- **Assignment brief + references** → [`references/`](./references)

---

## ⚠️ Disclaimer

Content here is for **education** and **portfolio** purposes. Vulnerability references (e.g., CVEs) are provided in `references/bibliography.md`. Keep your environments patched and isolated.
