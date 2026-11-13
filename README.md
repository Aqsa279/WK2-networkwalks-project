🔐 WK2 – Footprinting, Reconnaissance & Network Scanning
Week 2 Cybersecurity Hands-on Project | OSINT | Footprinting | Network Reconnaissance
![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-404040?style=flat-square)
![OSINT](https://img.shields.io/badge/Focus-OSINT-0077B5?style=flat-square)
![Kali Linux](https://img.shields.io/badge/Platform-Kali%20Linux-557C94?style=flat-square)
![Nmap](https://img.shields.io/badge/Tool-Nmap-4682B4?style=flat-square)
![Maltego](https://img.shields.io/badge/Tool-Maltego-8A2BE2?style=flat-square)
![theHarvester](https://img.shields.io/badge/Tool-theHarvester-E87500?style=flat-square)

---
📌 Project Overview
---
This repository documents my Week 2 practical cybersecurity work focused on footprinting, reconnaissance, Open-Source Intelligence (OSINT), and network scanning. The exercises cover collecting publicly available domain information, identifying web technologies and DNS records, exploring Google Hacking Database (GHDB) search techniques, mapping domain-related entities with Maltego, gathering public email and subdomain information with theHarvester, and performing network discovery and scanning with Nmap/Zenmap.
The repository is organized by project module and task so that screenshots, notes, command outputs, and the final report can be reviewed easily. Only actual results from my own authorized lab work will be added; no findings or screenshots are fabricated.

---
🎯 Project Objectives
---
Understand the fundamentals of footprinting and reconnaissance.
Practice collecting and documenting publicly available domain information.
Use Kali Linux tools to inspect registration, web technology, DNS, HTTP headers, WAF presence, and DNS records.
Understand GHDB and Google search operators for security research.
Explore domain-related email information and entity relationships with Maltego, where authorized.
Use theHarvester to collect publicly available email addresses, hosts, and subdomains from selected sources.
Practice network discovery, live-host identification, and scanning with Nmap/Zenmap in an authorized environment.
Record observations, screenshots, and outputs in a structured technical report.
---
🛠️ Tools & Technologies
Tool	Purpose in this project
WHOIS	Review public domain registration information
WhatWeb	Identify technologies used by a website
Nslookup	Query DNS and resolve domain information
cURL	Inspect HTTP response headers (`curl -I`)
WAFW00F	Check for a web application firewall
DNSRecon	Enumerate DNS records
GHDB	Learn Google dorks and search for publicly indexed exposure
Maltego	Visualize relationships between domain entities and email-related data
theHarvester	Gather publicly available emails, hosts, and subdomains from data sources
Nmap / Zenmap	Network discovery, scanning, and topology visualization
	
---
📂 Repository Structure
```text
WK2-Cybersecurity-Project/
│
├── README.md
│
├── W2-PM1-Footprinting-Multiple-Kali-Tools/
│   ├── README.md
│   ├── Task-01-WHOIS/                 # Registration details
│   ├── Task-02-WhatWeb/               # Web technology fingerprinting
│   ├── Task-03-Nslookup/               # Domain-to-IP / DNS lookup
│   ├── Task-04-cURL-Headers/            # HTTP response headers
│   ├── Task-05-WAFW00F/                 # WAF detection
│   └── Task-06-DNSRecon/                # DNS record enumeration
│
├── W2-PM2-Footprinting-with-GHDB/
│   ├── README.md
│   ├── Task-01-GHDB-Camera-Search/      # Record authorized research only
│   └── Task-02-Mathematics-PDF-Listings/
│
├── W2-PM3-Footprinting-with-Maltego/
│   ├── README.md
│   ├── Task-01-Maltego-Installation/
│   └── Task-02-Domain-Email-Transforms/
│
├── W2-PM4-Footprinting-with-theHarvester/
│   ├── README.md
│   ├── Task-01-Baidu-Source/            # microsoft.com, limit 1000 (per lab brief)
│   └── Task-02-All-Sources/             # microsoft.com, limit 50 (per lab brief)
│
├── W2-PM5-Network-Scanning-Nmap-Zenmap/
│   ├── README.md
│   └── Task-Screenshots/                # Add task folders after confirming PM5 brief
│
└── Final-Project-Report/
    ├── README.md
    ├── Final-Report.pdf                 # Add your completed report
    └── Final-Report.docx                # Add your editable report
---
🔍 Summary
---
W2-PM1 – Footprinting & Reconnaissance with Multiple Kali Tools
---
The lab brief uses six Kali Linux tools against `networkwalks.com`:
`whois networkwalks.com` – review public domain registration details.
`whatweb networkwalks.com` – fingerprint website technologies.
`nslookup networkwalks.com` – query domain DNS information.
`curl -I https://networkwalks.com` – inspect HTTP response headers.
`wafw00f https://networkwalks.com` – check for WAF indicators.
`dnsrecon -d networkwalks.com` – enumerate DNS information.
Save each task's screenshot and, where applicable, terminal output in that task's folder. Use the exact command and target approved by the instructor; the commands above are examples aligned with the module brief.
---
W2-PM2 – Footprinting & Reconnaissance with GHDB
---
The module introduces GHDB dorks and asks learners to document relevant search queries and results for two exercises: security-camera-related search results and downloadable mathematics PDF listings.
For ethical practice, do not open, view, control, or attempt to access exposed camera feeds or private systems. Use only instructor-approved, explicitly authorized test resources, and redact sensitive URLs, credentials, personal information, and private data from public screenshots. The repository should document the search method and safe, non-sensitive evidence rather than publish access to exposed devices.
---
W2-PM3 – Footprinting with Maltego
---
The module tasks are to install and configure Maltego on Windows, then use a Domain entity and email-related transforms for `networkwalks.com` with due permission. Add screenshots of installation/configuration and the transform/results view, redacting personal or sensitive data.
---
W2-PM4 – Footprinting & Reconnaissance with theHarvester
---
The module brief specifies two searches for `microsoft.com` in Kali Linux:
```bash
theHarvester -d microsoft.com -l 1000 -b baidu
theHarvester -d microsoft.com -l 50 -b all
```
Here, `-d` specifies the domain, `-l` sets the result limit, and `-b` selects the source. Save the screenshots and text outputs in the matching task folders. Results may vary as public data sources change.
---
W2-PM5 – Network Scanning with Nmap / Zenmap
---
This section is reserved for the network-scanning tasks discussed during the training. Add the exact task brief, screenshots, scan outputs, and topology export after verifying the instructor's PM5 instructions. Scan only systems and networks that you own or have explicit permission to test.
---
📸 Screenshots & Evidence
---
<img width="665" height="419" alt="whois-ss-1" src="https://github.com/user-attachments/assets/8cfe4a2b-eecc-4598-b37c-4b53caa9b0ee" />
<img width="658" height="433" alt="whois-ss-3" src="https://github.com/user-attachments/assets/e5524fed-41a0-4414-b356-48ba5edf2a06" />
<img width="658" height="433" alt="whois-ss-3" src="https://github.com/user-attachments/assets/79b14866-b018-49ff-9ed4-6afbea888974" />
<img width="636" height="131" alt="whatweb networkwalks" src="https://github.com/user-attachments/assets/a9cf3094-7ca9-474c-95fc-f8e5abe18dad" />
<img width="706" height="320" alt="nslookup" src="https://github.com/user-attachments/assets/e044ea02-4a10-4c94-845a-317b244d0685" />
<img width="713" height="269" alt="curl-2-orignal" src="https://github.com/user-attachments/assets/f6ad0b43-297a-45c1-b5e2-4409d72c93d3" />
<img width="663" height="291" alt="wafw00f" src="https://github.com/user-attachments/assets/5db9b3bb-02eb-4afa-b294-0967e8a660a5" />
<img width="664" height="325" alt="dnsrecon" src="https://github.com/user-attachments/assets/9faa5cc2-2225-4839-8c3a-0fe1fdd5b4e5" />



<img width="959" height="489" alt="Screenshot 2026-11-13 105934" src="https://github.com/user-attachments/assets/5aed5477-01f9-4fdd-9c8c-064aec6ce278" />
<img width="956" height="496" alt="Screenshot 2026-11-13 110035" src="https://github.com/user-attachments/assets/c30ef0ff-1376-4cf7-846c-9b96cb808d0d" />



<img width="298" height="286" alt="Screenshot 2026-11-12 112540" src="https://github.com/user-attachments/assets/9f77208b-e497-40f5-b5ae-bfc1781eebcc" />
<img width="652" height="416" alt="Screenshot 2026-11-12 112559" src="https://github.com/user-attachments/assets/47299c74-4004-4577-8a62-cecf3bb7b045" />
<img width="659" height="416" alt="1" src="https://github.com/user-attachments/assets/859b44f6-5f52-4f42-9a60-fc090d071474" />



<img width="950" height="481" alt="Screenshot 2026-11-10 100617" src="https://github.com/user-attachments/assets/73868b51-07d2-490c-bd4f-94cfac3d1e80" />
<img width="954" height="464" alt="Screenshot 2026-11-12 185918" src="https://github.com/user-attachments/assets/58343a41-208b-4adf-89f2-5e5511e8c851" />


---
📄 Final Project Report
---
The `Final-Project-Report/` folder is reserved for the completed PDF and editable Word report. The report should accurately describe the scope, authorized methodology, tools, actual observations, evidence references, limitations, and recommendations. Do not claim a task was completed until you have performed it and saved its evidence.
---
⚖️ Ethical Use & Disclaimer
---
This repository is for educational and authorized cybersecurity learning. Perform testing only on systems you own, a lab environment, or systems for which you have documented permission and an agreed scope. Publicly indexed information is not permission to access a device or private data. Never publish credentials, private records, or links that enable access to exposed devices.
---
👩‍💻 Author
---
Aqsa Shafiq  
Cybersecurity Learner | Aspiring Android Pentester
GitHub: Aqsa279
LinkedIn: Aqsa Shafiq
---
Learning today, securing tomorrow! 🔐
```
