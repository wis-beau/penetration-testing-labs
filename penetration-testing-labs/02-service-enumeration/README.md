# 02 · Service Enumeration (Banner Grabbing)

Manual verification of key services using `netcat` and `telnet` to confirm versions and capture banners.

## Commands Used

```bash
# FTP banner (port 21)
nc -nv 192.168.56.102 21

# Alternative FTP banner via telnet (often works similarly)
telnet 192.168.56.102 21

# HTTP banner (if needed)
telnet 192.168.56.102 80
# then type: HEAD / HTTP/1.0  (press Enter twice)
```

## Files

- `netcat-banners.txt` — raw output from `nc` sessions.
- `telnet-banners.txt` — raw output from `telnet` sessions.
- `vsftpd-version.txt` — extracted version note for vsftpd.