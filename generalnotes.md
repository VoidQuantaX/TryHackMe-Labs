# 📝 General Notes

This file collects *general cybersecurity concepts, commands, and best practices* that I learned during my TryHackMe journey and beyond.  
It acts as a quick reference and highlights my ability to connect theory with practical offensive security skills.

---

## 🔍 Enumeration & Recon
- Importance of *enumeration before exploitation*  
- Common tools: nmap, gobuster, dirb, nikto, whatweb  
- OSINT basics: whois, nslookup, dig, Shodan, DNSDumpster  

---

## ⚡ Exploitation Concepts
- SQL Injection (manual + automated)  
- Command Injection  
- File Upload Bypass  
- XSS (Reflected, Stored, DOM-based)  
- SSRF & LFI/RFI  

---

## 🛡️ Privilege Escalation Basics
- Kernel exploits  
- Sudo misconfigurations  
- PATH hijacking  
- SUID/SGID binaries  
- Windows: Registry, Weak Services, Token Impersonation  

---

## 🧰 Handy Linux Commands
- find / -perm -4000 2>/dev/null → Find SUID binaries  
- netstat -tulnp → Check listening ports  
- strings filename → Analyze binaries  
- ps aux → Check running processes  

---

## 🌐 Networking Concepts
- TCP 3-way handshake  
- Difference between TCP and UDP in exploitation  
- Common ports and services (22, 80, 443, 3306, 8080, etc.)  

---

## 📌 Key Takeaway
This section shows I not only practiced labs but also built a strong foundation of *general security concepts*, making me effective in adapting to new environments quickly.
