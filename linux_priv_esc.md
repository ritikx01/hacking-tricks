1. `sudo -l` to check for binaries we can run. Search for that binary in gtfobins.
2. Find files with SUID bits set `find / -perm -u=s 2>/dev/null`.
