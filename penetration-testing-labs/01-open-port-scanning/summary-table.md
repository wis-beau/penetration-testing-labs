# Discovered Ports & Services (from `-sV`) Output (sanitized)

| Port | Service        | Version / Banner                                        | Notes |
|-----:|----------------|---------------------------------------------------------|-------|
| 21/tcp  | ftp            | vsftpd 2.3.4                                           | Known backdoor, see CVE-2011-2523 |
| 22/tcp  | ssh            | OpenSSH 4.7p1 Debian 8ubuntu1 (protocol 2.0)          | Legacy SSH |
| 23/tcp  | telnet         | Linux telnetd                                          | Insecure plaintext protocol |
| 25/tcp  | smtp           | Postfix smtpd                                          | Mail transfer agent exposed |
| 53/tcp  | domain         | ISC BIND 9.4.2                                         | DNS server |
| 80/tcp  | http           | Apache httpd 2.2.8 (Ubuntu) DAV/2                      | Outdated Apache |
| 111/tcp | rpcbind        | RPC #100000 v2                                         | RPC endpoint mapper |
| 139/tcp | netbios-ssn    | Samba smbd 3.X–4.X (WORKGROUP)                         | Windows file sharing (NetBIOS) |

> Note: Exact ports/services may vary slightly between boots; verify against your saved `nmap-scan-full.txt`.
