# ⚡ Nmap — Network Scanning & Enumeration

> Documenting practical Nmap skills gained through TryHackMe labs and real-world recon workflows.  
> This section shows how I use Nmap not just for scanning, but to map an attack surface and guide exploitation.

---

## 📌 Key Techniques
- *Host Discovery* → nmap -sn 10.10.10.0/24  
- *Port Scanning* → nmap -p- -T4 target (full range, fast timing)  
- *Service Enumeration* → nmap -sV -sC -p 22,80 target  
- *OS Fingerprinting* → nmap -O target  
- *Aggressive Scan* → nmap -A target (version, scripts, traceroute)  

---

## 🔍 Real-World Scenarios
- Identified *open SSH & HTTP ports* → attempted brute force and web enumeration.  
- Used *version detection* to find outdated Apache server → led to exploit research.  
- Combined *Nmap scripts (NSE)* to check for vulnerabilities (e.g., SMB, FTP).  
- Prioritized *high-value ports (21,22,80,443,445,3389)* for deeper exploitation.  

---

## 🧑‍💻 Workflow Example
1. Run initial scan to map open ports.  
2. Enumerate services and versions.  
3. Cross-reference results with *Exploit DB / Metasploit modules*.  
4. Choose exploitation path (e.g., outdated SMB → EternalBlue).  

---

## 🔑 Key Skills Demonstrated
- Efficient scanning under stealth/timing constraints.  
- Translating scan results into actionable exploit paths.  
- Integration with *Gobuster, Hydra, and Burp Suite* for full kill-chain.  

---
