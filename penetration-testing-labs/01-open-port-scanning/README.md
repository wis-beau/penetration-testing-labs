# 01 · Open Port Scanning

This folder contains the **Nmap scanning workflow** and raw outputs used to enumerate open TCP ports and detect service versions on the Metasploitable 2 target.

## Commands Used

> Replace `TARGET` with your Metasploitable IP (e.g., `192.168.56.102`).

```bash
# 1) Full TCP port sweep (65,535 ports) + service detection
nmap -sV -p- TARGET

# 2) Detailed fingerprinting (aggressive detection/scripts)
nmap -A TARGET
```

> Tip: Save outputs to files using `-oN` or redirect, e.g. `nmap -sV -p- TARGET -oN nmap-scan-full.txt`.

## Files

- `nmap-scan-full.txt` — output from the full‑port + service scan.
- `nmap-scan-detailed.txt` — output from the `-A` (aggressive) scan.
- `summary-table.md` — human‑readable table of discovered ports & services.

## Notes

- Always validate service versions with **manual banner grabbing** to avoid false positives (see `../02-service-enumeration`).