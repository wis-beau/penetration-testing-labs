# Discovered Ports & Services (from `-sV`)

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
| 445/tcp | microsoft-ds   | Samba smbd 3.X–4.X (WORKGROUP)                         | SMB file sharing |
| 512/tcp | exec           | netkit-rsh rexecd                                      | Legacy r-services |
| 513/tcp | login          | rlogind                                                | Legacy r-services |
| 514/tcp | shell          | rshd                                                   | Legacy r-services |
| 1099/tcp| java-rmi       | GNU Classpath rmiregistry                              | Java RMI registry |
| 1524/tcp| bindshell      | Metasploitable root shell                              | Intentional backdoor (lab) |
| 2049/tcp| nfs            | NFS v2–v4 (RPC #100003)                                | Network file system |
| 2121/tcp| ftp            | ProFTPD 1.3.1                                          | Additional FTP service |
| 3306/tcp| mysql          | MySQL 5.0.51a-3ubuntu5                                 | Outdated DB |
| 3632/tcp| distccd        | distccd v1 (GNU 4.2.4)                                 | RCE risk, see CVE-2004-2687 |
| 5432/tcp| postgresql     | PostgreSQL 8.3.0–8.3.7                                 | Outdated DB |
| 5900/tcp| vnc            | VNC (protocol 3.3)                                     | Remote desktop exposed |
| 6000/tcp| X11            | access denied                                          | X server exposed |
| 6667/tcp| irc            | UnrealIRCd                                             | Backdoored build existed, CVE-2010-2075 |
| 6697/tcp| ircs-u         | UnrealIRCd (SSL)                                       | Backdoored build existed, CVE-2010-2075 |
| 8009/tcp| ajp13          | Apache JServ Protocol (AJP13)                          | Tomcat connector |
| 8180/tcp| http?          | unknown                                                | Secondary web interface (validate) |
| 8787/tcp| drb            | Ruby DRb RMI (Ruby 1.8)                                | Ruby Distributed Ruby |
| 34723/tcp| rpc.mountd    | mountd (RPC #100005)                                   | Dynamic RPC (example) |
| 35131/tcp| rpc.status    | status (RPC #100024)                                   | Dynamic RPC (example) |
| 36401/tcp| rpc.nlockmgr  | nlockmgr (RPC #100021)                                 | Dynamic RPC (example) |
| 57323/tcp| rpc.*         | additional RPC                                         | Dynamic RPC (example) |

> Note: Exact ports/services may vary slightly between boots; verify against your saved `nmap-scan-full.txt`.