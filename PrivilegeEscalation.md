# 🔼 Privilege Escalation — Linux & Windows

> Documenting key privilege escalation techniques practiced in TryHackMe labs.  
> Privilege escalation transforms an initial foothold into full system compromise — a core penetration testing skill.

---

## 🐧 Linux Privilege Escalation

### 🔍 Common Techniques
- *Kernel Exploits* → outdated kernels (dirty cow, overlayfs)  
- *SUID Binaries* → abuse misconfigured executables (find / -perm -4000 -type f 2>/dev/null)  
- *Weak Permissions* → writable /etc/passwd, /etc/shadow  
- *Cron Jobs* → hijacking scheduled scripts  
- *PATH Hijacking* → replacing binaries in user PATH  
- *NFS Misconfigurations* → root squashing disabled  

### ⚡ Real-World Example
- Found python as SUID binary → escalated to root.  
- Abused writable cron script /etc/cron.d/backup.sh.  
- Exploited vulnerable kernel version with a local privilege escalation exploit.  

---

## 🪟 Windows Privilege Escalation

### 🔍 Common Techniques
- *Service Exploits* → misconfigured services with weak file permissions  
- *Unquoted Service Paths* → inject malicious executables  
- *Registry Escalation* → weak registry keys containing credentials  
- *Stored Credentials* → dumped from memory, SAM database, or config files  
- *Token Impersonation* → SeImpersonatePrivilege (Juicy Potato, PrintSpoofer)  
- *DLL Hijacking* → replacing DLLs loaded by privileged processes  

### ⚡ Real-World Example
- Found misconfigured service → replaced binary → SYSTEM access.  
- Used mimikatz to dump administrator credentials.  
- Exploited SeImpersonatePrivilege with Juicy Potato for escalation.  

---

## 🧑‍💻 Workflow Example
1. Run *LinPEAS / WinPEAS* to automate enumeration.  
2. Check for kernel exploits (Linux) or misconfigured services (Windows).  
3. Attempt manual exploitation → escalate privileges.  
4. Verify persistence and clean up traces.  

---

## 🔑 Key Skills Demonstrated
- Mastery of *post-exploitation privilege escalation* techniques.  
- Ability to escalate from *low-privilege shell → root/SYSTEM*.  
- Knowledge of *automated + manual enumeration tools*.  
- Real-world exploitation of *misconfigurations and kernel flaws*.  

---
