# 💥 Metasploit — Framework for Exploitation

> Documenting my practical use of Metasploit from TryHackMe labs and real-world attack workflows.  
> This section highlights how I leverage Metasploit for scanning, exploitation, post-exploitation, and privilege escalation.

---

## 📌 Key Techniques
- *Auxiliary Scans* → use auxiliary/scanner/portscan/tcp  
- *Exploitation* → use exploit/windows/smb/ms17_010_eternalblue  
- *Payload Selection* → set payload windows/meterpreter/reverse_tcp  
- *Sessions Handling* → interacting with multiple shells simultaneously  
- *Post-Exploitation Modules* → password dumping, keylogging, persistence  

---

## 🔍 Real-World Scenarios
- Exploited *SMB vulnerability (EternalBlue)* to gain system shell.  
- Used *FTP exploit* for misconfigured anonymous login.  
- Delivered a *reverse shell payload* and maintained persistence.  
- Extracted *Windows credentials* with Mimikatz module.  
- Combined Metasploit with *Nmap results* to identify exploitable services quickly.  

---

## 🧑‍💻 Workflow Example
1. Import Nmap results into Metasploit DB.  
2. Search for matching exploits using search <service/version>.  
3. Configure exploit & payload, launch attack.  
4. Post-exploitation → gather credentials, escalate privileges, pivot to new hosts.  

---

## 🔑 Key Skills Demonstrated
- Effective use of Metasploit for *rapid exploitation*.  
- Transition from automated to *manual exploitation* when needed.  
- Knowledge of *post-exploitation techniques* (persistence, data exfiltration).  
- Ability to integrate Metasploit into a *red team workflow*.  

---
