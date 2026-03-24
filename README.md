<div align="center">

# Viktor Vas | Junior SOC Analyst & Blue Team Specialist

**`Defense & Incident Response · Threat Modeling · OSINT · Hardware Security`**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-viktor--vas-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/viktor-vas)
[![GitHub](https://img.shields.io/badge/GitHub-vasviktor--cyber-181717?style=flat&logo=github&logoColor=white)](https://github.com/vasviktor-cyber)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Pre_Security-88cc14?style=flat&logo=tryhackme&logoColor=white)](https://tryhackme.com)
[![Location](https://img.shields.io/badge/Location-Bad_Salzuflen,_Germany-blue?style=flat&logo=googlemaps&logoColor=white)](#)

</div>

---

## 🛡️ About Me

I'm a cybersecurity analyst in training with a sharp Blue Team focus, currently transitioning from **10+ years of hands-on heavy machinery troubleshooting** (Baumaschinenmechatroniker) into the world of IT security. Reading complex wiring diagrams, performing systematic fault diagnosis under pressure, and maintaining strict safety compliance (DGUV/TRBS) — this is the investigative, methodical mindset I now bring to SOC operations and incident response.

Before my civilian career, I served as a **commander in strategic air defense**, where I developed the kind of discipline, stress resistance, and responsibility for system integrity that directly translates to defending digital infrastructure.

> *"I don't wait for opportunities — I prepare for them."*

I completed the **Robot Dreams Cyber Security Fundamentals** academy with a score of **97% (193/200 points)**, ranking in the **Top 4 of 19 participants** across a 14-week intensive program. My portfolio is built on real-world incidents, not textbook exercises — including a full investigation of a Rhadamanthys Infostealer attack on my own workstation.

**Goal:** Junior SOC Analyst position in the DACH region (remote-friendly), with a long-term path toward CompTIA Security+ and ISO 27001 certification.

---

## 🔧 Core Competencies & Tools

### Blue Team & Defense
![Incident Response](https://img.shields.io/badge/Incident_Response-IR_Lifecycle-2C2D72?style=flat-square)
![Threat Modeling](https://img.shields.io/badge/Threat_Modeling-STRIDE-D32F2F?style=flat-square)
![Kill Chain](https://img.shields.io/badge/Cyber_Kill_Chain-Analysis-FF6F00?style=flat-square)
![Log Analysis](https://img.shields.io/badge/Log_Analysis-Triage-4CAF50?style=flat-square)
![OWASP](https://img.shields.io/badge/OWASP-Top_10-000000?style=flat-square&logo=owasp&logoColor=white)
![Defense in Depth](https://img.shields.io/badge/Defense_in_Depth-Strategy-1565C0?style=flat-square)

### OSINT & Threat Intelligence
![Maltego](https://img.shields.io/badge/Maltego-OSINT-2596BE?style=flat-square)
![Shodan](https://img.shields.io/badge/Shodan-Recon-D32F2F?style=flat-square)
![VirusTotal](https://img.shields.io/badge/VirusTotal-Analysis-394EFF?style=flat-square)
![AbuseIPDB](https://img.shields.io/badge/AbuseIPDB-Threat_Intel-1B5E20?style=flat-square)

### Network & System Analysis
![Nmap](https://img.shields.io/badge/Nmap-Port_Scanning-4682B4?style=flat-square)
![Wireshark](https://img.shields.io/badge/Wireshark-Traffic_Analysis-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-Security-0078D6?style=flat-square&logo=windows&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Fundamentals-FCC624?style=flat-square&logo=linux&logoColor=black)

### Hardware & Low-Level Security
![SPI Flash](https://img.shields.io/badge/SPI_Flash-CH341A-FF6F00?style=flat-square)
![UART](https://img.shields.io/badge/UART-Serial_Debug-607D8B?style=flat-square)
![BIOS/UEFI](https://img.shields.io/badge/BIOS%2FUEFI-Firmware_Config-333333?style=flat-square)
![Virtualization](https://img.shields.io/badge/Virtualization-VMs_%26_Sandbox-6A1B9A?style=flat-square)

---

## 📂 Featured Projects

### 1. 🔴 Rhadamanthys Infostealer — Real-World Incident Response

> Full investigation of a live malware attack on my own workstation (Oct 2025). Not a simulation — a real supply-chain infection with documented C2 infrastructure.

- **Scenario:** A compromised third-party driver installer (SignalRGB) delivered the Rhadamanthys Stealer malware via drive-by-download. Security protections (Secure Boot, Core Isolation) had been disabled following flawed AI-generated instructions.
- **Methodology:**
  - Complete **Cyber Kill Chain analysis**: initial access → process injection into `wmprph.exe` → credential theft via `LsaIso.exe` modification → C2 beaconing to `178.22.24.253:58888`
  - **OSINT tracking** of C2 server using Shodan, VirusTotal & AbuseIPDB → attributed to **Galeon LLC, Moscow**
  - Malware family identified: **Rhadamanthys Stealer** (11/93 VT detection rate)
  - Documented impacts: session hijacking, account takeover (Ubisoft, Microsoft, Instagram), crypto mining
- **Outcome:** Developed and executed a **"Scorched Earth" remediation protocol** — network isolation, full clean install, router factory reset, identity lockdown across all accounts, and hardware replacement (phone + SIM card).

---

### 2. 🟠 Collé Rental & Sales — Incident Response Plan

> Practical IR plan designed for a real employer: an international heavy equipment rental company with a Citrix-based infrastructure spanning the Netherlands and Germany.

- **Scenario:** Protect critical systems (Citrix environment, Track & Trace fleet monitoring, central Dutch database) from cybersecurity incidents, with a focus on phishing threats.
- **Methodology:**
  - Defined **roles & responsibilities** (Incident Commander, Network Admins, Data Analysts, 24/7 IT Emergency, On-Site Support)
  - Built a **3-tier incident classification system** (Critical / Medium / Low) with clear escalation criteria
  - Mapped the full **IR lifecycle**: Identification → Containment → Eradication → Recovery → Lessons Learned
  - Created the **"5555 Protocol"** — a dedicated internal emergency hotline for immediate incident reporting
  - Designed a **mandatory annual cybersecurity e-learning program** with 30-question exam (80% pass threshold) and certification-gated system access
- **Outcome:** Complete phishing attack simulation scenario with step-by-step containment, communication plan, and post-incident training integration.

---

### 3. 🟡 E-Commerce Threat Modeling (eBay Architecture)

> Systematic security analysis of an eBay-style e-commerce platform using the STRIDE methodology and Microsoft Threat Modeling Tool.

- **Scenario:** Model the full attack surface of an e-commerce platform including buyer/seller interactions, payment processing, API gateways, and database infrastructure.
- **Methodology:**
  - Built a complete **Data Flow Diagram (DFD)** with 6 core assets: user data, payment data, APIs, web servers, database, and listings
  - Defined **Trust Boundaries** across 4 zones: External Zone → DMZ/Web Zone → Internal Core → Third-Party (Payment)
  - Applied **STRIDE** (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege) to identify **30+ threat vectors** (SQLi, XSS, DDoS, BEC, token theft)
  - Created a **mitigation matrix** per asset type (WAF, rate limiting, 2FA, least privilege, input validation)
- **Outcome:** Comprehensive Defense-in-Depth strategy document. Scored **30/30 points** (academic validation).

---

### 4. 🔵 ASUS TUF-AX3000 V2 — Hardware Recovery (SPI Flash & UART)

> Low-level firmware recovery of a completely bricked router using physical flash programming and serial console debugging.

- **Scenario:** The router became unresponsive ("bricked") after a failed firmware update, with no software recovery possible.
- **Methodology:**
  - **SPI Flash recovery** using a CH341A programmer with SOIC8 test clip — direct physical read/write to the flash chip
  - Accessed the **U-Boot bootloader** via UART serial interface (PuTTY, 115200 baud) for diagnostics
  - Performed **TFTP firmware flash** through the bootloader console to restore the original firmware
- **Outcome:** Fully documented step-by-step recovery guide. Router restored to full functionality. Demonstrates hardware-level troubleshooting skills directly applicable to IoT/OT security and forensic analysis.

---

### 5. 🟢 Blue Team Homelab — Custom Workstation Architecture

> Purpose-built cybersecurity workstation designed from scratch for Blue Team studies, virtualization, and secure remote work.

- **Scenario:** Design and build a silent, high-performance, thermally optimized workstation as a foundation for traffic analysis, VM-based labs, and continuous security studies.
- **Methodology:**
  - Resolved **BIOS/firmware incompatibility** between MSI B450 Tomahawk MAX and a newer AMD Ryzen CPU via manual BIOS flashing with a temporary processor
  - Engineered **push-pull airflow** with Arctic fans and created custom **PWM fan curves** in BIOS for near-silent "Ninja mode" operation
  - Integrated multi-generation hardware (Sound BlasterX, XFX Radeon, Wi-Fi/BT module) into a Xilent Beam aquarium case
  - Solved **voltage mismatch** between 5V ARGB and 12V RGB standards by isolating the lighting system to a dedicated control panel
  - Diagnosed and resolved **MSI Center vs. BIOS priority conflicts**, enforcing hardware-level control
- **Outcome:** A perfectly functioning, thermally efficient, and cable-managed workstation ready for network traffic analysis, VM execution, and stable long-term operation.

---

## 🎓 Education & Certifications

| Certification | Provider | Date | Details |
|---|---|---|---|
| 🏆 **Cyber Security Fundamentals** | Robot Dreams | Jan – Mar 2026 | 97% score (193/200) · Top 4 of 19 · 14-week intensive |
| ✅ **Pre Security Learning Path** | TryHackMe | Mar 2026 | 19 hours · Networks, Linux, Web, Security Fundamentals |
| 🔧 **Electromechanic for Machinery** | Technical School, Subotica (Serbia) | 2001 – 2004 | Electronics, Mechanics, Schematics, Technical Maintenance |

**Currently targeting:** CompTIA Security+ · ISO 27001

---

## 🌍 Languages

| Language | Level |
|---|---|
| 🇭🇺 Hungarian | Native |
| 🇩🇪 German | Proficient (written & spoken) |
| 🇷🇸 Serbian | Fluent |

---

## 📊 Professional Background

**10+ years** as a Baumaschinenmechatroniker (Heavy Machinery Mechatronics Technician) at **Collé Rental & Sales**, performing systematic fault diagnosis on complex electronic systems, conducting safety inspections (DGUV/TRBS compliance), and maintaining technical documentation — skills that transfer directly to SOC operations, log analysis, and IT security auditing.

---

<div align="center">

*Built with discipline. Driven by precision. Ready to defend.*

[![Email](https://img.shields.io/badge/Contact-hucicok%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hucicok@gmail.com)

</div>
