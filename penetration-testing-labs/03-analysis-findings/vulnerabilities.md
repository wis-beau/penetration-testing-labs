# Vulnerabilities & Potential Impact

> Map discovered services to well-known issues for Metasploitable 2. Validate against your own evidence.

| Service / Port | Version / Evidence | Risk Summary | Notable CVE / Ref |
|---|---|---|---|
| FTP (21/tcp) | `220 (vsFTPd 2.3.4)` | Backdoored build that opens shell on 6200/tcp | CVE-2011-2523 |
| IRC (6667/6697) | UnrealIRCd (per `-sV`) | Trojaned source backdoor allowing RCE | CVE-2010-2075 |
| distccd (3632/tcp) | `distccd v1` | Command execution if access not restricted | CVE-2004-2687 |
| Samba (139/445) | smbd 3.X–4.X | Auth/browse risks on legacy configs | Hardening guides |
| NFS (2049) | NFS v2–v4 | Data exposure via exports, weak perms | Hardening guides |
| VNC (5900) | VNC 3.3 | Remote desktop exposure, weak auth | Hardening guides |
| X11 (6000) | X server open | Local display exposure, potential snooping | Hardening guides |
| MySQL (3306) | 5.0.51a | Outdated DB server | Patch/upgrade |
| PostgreSQL (5432) | 8.3.x | Outdated DB server | Patch/upgrade |
| Apache (80) | 2.2.8 | Outdated HTTP server | Patch/upgrade |

**Note**: Metasploitable 2 is intentionally vulnerable; treat these as **training findings** and not representative of modern hardened systems.