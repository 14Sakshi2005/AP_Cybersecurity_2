#  Vulnerability Assessment using GVM  

<p align="center">
  <img src="https://img.shields.io/badge/Tool-GVM%20(OpenVAS)-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Platform-Kali%20Linux-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Target-Metasploitable2-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge">
</p>


##  Overview  
This project demonstrates a **comprehensive vulnerability assessment** performed on an intentionally vulnerable system using **Greenbone Vulnerability Management (GVM / OpenVAS)**.  

It covers the complete workflow from **reconnaissance → scanning → vulnerability analysis → reporting**.


##  Objective  
- Identify security vulnerabilities in a target system  
- Analyze vulnerabilities using CVE data and severity levels  
- Document findings in a structured and professional format  


##  Tech Stack  

| Tool | Purpose |
|------|--------|
|  Kali Linux | Attacker Environment |
|  GVM (OpenVAS) | Vulnerability Scanning |
|  Nmap | Network Scanning & Enumeration |
|  Metasploitable2 | Vulnerable Target Machine |


##  Target Information  

- **IP Address:** `192.168.64.4`  
- **Environment:** Virtual Lab (UTM)  


##  Methodology  

### 1. Reconnaissance  
- Verified host availability using ping  
- Performed port scanning using Nmap  

```bash
ping 192.168.64.4
nmap -sS -sV 192.168.64.4
```

### 2. Vulnerability Scanning

      - Configured GVM (OpenVAS)
      - Created and launched scan task
      - Used Full and Fast Scan Profile
      - Targeted the system for vulnerability detection

### 3. Analysis

      - Reviewed scan results
      - Categorized vulnerabilities based on severity:
              🔴 Critical
              🟠 High
              🟡 Medium
              🔵 Low
      - Analyzed associated CVE IDs


### Results
✔ Multiple vulnerabilities detected
✔ Services exposed with known weaknesses
✔ Risks categorized based on severity levels

Report: gvm_scan_report.pdf

Note: Metasploitable2 is intentionally vulnerable, so high-severity issues are expected.

 screenshots/4.1 (open port details).png

 screenshots/7.png

 screenshots/8.png

