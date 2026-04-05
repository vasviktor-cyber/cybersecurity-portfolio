<div align="center">

# Viktor Vas | Junior SOC Analyst & Blue Team Spezialist

**`Verteidigung & Incident Response · Bedrohungsmodellierung · OSINT · Hardware-Sicherheit`**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-viktor--vas-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/viktor-vas)
[![GitHub](https://img.shields.io/badge/GitHub-vasviktor--cyber-181717?style=flat&logo=github&logoColor=white)](https://github.com/vasviktor-cyber)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Pre_Security-88cc14?style=flat&logo=tryhackme&logoColor=white)](https://tryhackme.com)
[![Standort](https://img.shields.io/badge/Standort-Bad_Salzuflen,_Deutschland-blue?style=flat&logo=googlemaps&logoColor=white)](#)

</div>

---

## 🛡️ Über mich

Ich bin ein angehender IT-Sicherheitsanalytiker mit klarem Blue-Team-Fokus. Aktuell befinde ich mich im strategischen Berufswechsel — nach **über 10 Jahren als Baumaschinenmechatroniker** bringe ich eine solide Basis an systematischer Fehlerdiagnose, Lesen komplexer Schaltpläne und präzisem Troubleshooting in die Cybersicherheit mit.

Vor meiner zivilen Karriere diente ich als **Kommandant in der strategischen Luftabwehr**. Dort habe ich gelernt, in kritischen Situationen absolute Disziplin, Stressresistenz und höchste Verantwortung für die Sicherheit von Systemen zu übernehmen. Ordnung und Präzision sind die Grundpfeiler meiner Arbeitsweise.

> *„Ich warte nicht auf Gelegenheiten — ich bereite mich proaktiv vor."*

Ich habe die **Robot Dreams Cyber Security Fundamentals**-Akademie mit **97 % (193/200 Punkte)** abgeschlossen und gehörte zu den **Top 4 von 19 Teilnehmern** in einem 14-wöchigen Intensivprogramm. Mein Portfolio basiert auf realen Vorfällen — darunter die vollständige Untersuchung eines Rhadamanthys-Infostealer-Angriffs auf meine eigene Workstation.

**Ziel:** Junior SOC Analyst Position im DACH-Raum (Remote-Option), mit langfristigem Ausbau durch CompTIA Security+ und ISO 27001 Zertifizierungen.

📄 **Gesamtes Portfolio als Präsentation:** [SOC Analyst Portfolio (PDF)](portfolio/presentations/Portfolio_SOC_Analyst_Viktor_Vas_DE.pdf)

---

## 🔧 Kernkompetenzen & Werkzeuge

### Blue Team & Verteidigung
![Incident Response](https://img.shields.io/badge/Incident_Response-IR--Lifecycle-2C2D72?style=flat-square)
![Bedrohungsmodellierung](https://img.shields.io/badge/Bedrohungsmodellierung-STRIDE-D32F2F?style=flat-square)
![Kill Chain](https://img.shields.io/badge/Cyber_Kill_Chain-Analyse-FF6F00?style=flat-square)
![Log-Analyse](https://img.shields.io/badge/Log--Analyse-Triage-4CAF50?style=flat-square)
![OWASP](https://img.shields.io/badge/OWASP-Top_10-000000?style=flat-square&logo=owasp&logoColor=white)
![Defense in Depth](https://img.shields.io/badge/Defense_in_Depth-Strategie-1565C0?style=flat-square)

### OSINT & Threat Intelligence
![Maltego](https://img.shields.io/badge/Maltego-OSINT-2596BE?style=flat-square)
![Shodan](https://img.shields.io/badge/Shodan-Aufklärung-D32F2F?style=flat-square)
![VirusTotal](https://img.shields.io/badge/VirusTotal-Analyse-394EFF?style=flat-square)
![AbuseIPDB](https://img.shields.io/badge/AbuseIPDB-Threat_Intel-1B5E20?style=flat-square)

### Netzwerk- & Systemanalyse
![Nmap](https://img.shields.io/badge/Nmap-Port--Scanning-4682B4?style=flat-square)
![Wireshark](https://img.shields.io/badge/Wireshark-Verkehrsanalyse-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-Sicherheit-0078D6?style=flat-square&logo=windows&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Grundlagen-FCC624?style=flat-square&logo=linux&logoColor=black)

### Hardware & Low-Level Sicherheit
![SPI Flash](https://img.shields.io/badge/SPI_Flash-CH341A-FF6F00?style=flat-square)
![UART](https://img.shields.io/badge/UART-Serielles_Debugging-607D8B?style=flat-square)
![BIOS/UEFI](https://img.shields.io/badge/BIOS%2FUEFI-Firmware--Konfiguration-333333?style=flat-square)
![Virtualisierung](https://img.shields.io/badge/Virtualisierung-VMs_%26_Sandbox-6A1B9A?style=flat-square)

---

## 🏗️ Defense-in-Depth Architektur — Überblick

<div align="center">

<img src="portfolio/infographics/Infographic_Defense_in_Depth_Architecture_DE.png" alt="Defense-in-Depth Architektur Infografik" width="600"/>

*Vollständige Visualisierung meiner Sicherheitsarchitektur: STRIDE-Analyse, Trust Boundaries, Netzwerk-Mitigationsmatrix und IR-Lebenszyklus.*

</div>

---

## 📂 Portfolio-Projekte

### 1. 🔴 Rhadamanthys Infostealer — Realer Incident Response Fall

> Vollständige Untersuchung eines echten Malware-Angriffs auf meine eigene Workstation (Okt. 2025). Keine Simulation — ein realer Supply-Chain-Angriff mit dokumentierter C2-Infrastruktur.

- **Szenario:** Ein kompromittierter Drittanbieter-Installer (SignalRGB) lieferte die Rhadamanthys-Stealer-Malware per Drive-by-Download. Sicherheitsmechanismen (Secure Boot, Kernisolierung) waren zuvor auf Basis fehlerhafter KI-Empfehlungen deaktiviert worden.
- **Methodik:**
  - Vollständige **Cyber Kill Chain Analyse**: Initialer Zugriff → Process Injection in `wmprph.exe` → Credential-Diebstahl via `LsaIso.exe`-Modifikation → C2-Beaconing zu `178.22.24.253:58888`
  - **OSINT-Rückverfolgung** des C2-Servers mittels Shodan, VirusTotal & AbuseIPDB → Zuordnung zu **Galeon LLC, Moskau**
  - Malware-Familie identifiziert: **Rhadamanthys Stealer** (11/93 VT-Erkennungsrate)
  - Dokumentierte Auswirkungen: Session Hijacking, Kontoübernahme (Ubisoft, Microsoft, Instagram), Krypto-Mining
- **Ergebnis:** Entwicklung und Umsetzung eines **„Scorched Earth"-Remediationsprotokolls** — Netzwerkisolation, Clean Install, Router-Factory-Reset, Identity Lockdown aller Konten und Hardware-Austausch (Telefon + SIM-Karte).

📄 **Dokumentation:** [Incident Report (PDF)](portfolio/projects/Report_Rhadamanthys_Infostealer_DE.pdf) · [Analyse-Präsentation (PDF)](portfolio/presentations/Presentation_Rhadamanthys_Analysis_DE.pdf)

---

### 2. 🟠 Collé Rental & Sales — Incident Response Plan

> Praxisnaher IR-Plan für einen realen Arbeitgeber: ein internationales Baumaschinenverleih-Unternehmen mit Citrix-basierter Infrastruktur zwischen den Niederlanden und Deutschland.

- **Szenario:** Schutz kritischer Systeme (Citrix-Umgebung, Track & Trace Flottenüberwachung, zentrale niederländische Datenbank) vor Cybersicherheitsvorfällen mit Schwerpunkt auf Phishing-Bedrohungen.
- **Methodik:**
  - Definition von **Rollen und Verantwortlichkeiten** (Incident Commander, Netzwerkadministratoren, Datenanalysten, 24/7-IT-Notdienst, Vor-Ort-Support)
  - Aufbau eines **3-stufigen Klassifizierungssystems** (Kritisch / Mittel / Niedrig) mit klaren Eskalationskriterien
  - Abbildung des vollständigen **IR-Lifecycle**: Identifikation → Eindämmung → Beseitigung → Wiederherstellung → Lessons Learned
  - Erstellung des **„5555-Protokolls"** — eine dedizierte interne Notrufnummer für sofortige Vorfallsmeldung
  - Konzeption eines **verpflichtenden jährlichen Cybersicherheits-E-Learnings** mit 30-Fragen-Test (80 %-Bestehensgrenze) und zertifikatsgebundenem Systemzugang
- **Ergebnis:** Vollständiges Phishing-Angriffsszenario mit schrittweiser Eindämmung, Kommunikationsplan und Integration in das Schulungsprogramm.

📄 **Dokumentation:** [IR-Plan (PDF)](portfolio/projects/Project_Colle_Incident_Response_Plan_DE.pdf) · [Security Blueprint Präsentation (PDF)](portfolio/presentations/Presentation_Colle_Security_Blueprint_DE.pdf)

---

### 3. 🟡 E-Commerce Bedrohungsmodellierung (eBay-Architektur)

> Systematische Sicherheitsanalyse einer eBay-artigen E-Commerce-Plattform mittels STRIDE-Methodik und Microsoft Threat Modeling Tool.

- **Szenario:** Modellierung der vollständigen Angriffsoberfläche einer E-Commerce-Plattform einschließlich Käufer-/Verkäufer-Interaktionen, Zahlungsabwicklung, API-Gateways und Datenbankinfrastruktur.
- **Methodik:**
  - Erstellung eines vollständigen **Datenflussdiagramms (DFD)** mit 6 Kern-Assets: Benutzerdaten, Zahlungsdaten, APIs, Webserver, Datenbank und Anzeigen
  - Definition von **Trust Boundaries** über 4 Zonen: External Zone → DMZ/Web Zone → Internal Core → Third-Party (Payment)
  - Anwendung von **STRIDE** (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege) zur Identifikation von **über 30 Bedrohungsvektoren** (SQLi, XSS, DDoS, BEC, Token-Diebstahl)
  - Erstellung einer **Mitigationsmatrix** pro Asset-Typ (WAF, Rate Limiting, 2FA, Least Privilege, Eingabevalidierung)
- **Ergebnis:** Umfassende Defense-in-Depth-Strategie. Akademische Validierung: **30/30 Punkte**.

📄 **Dokumentation:** [Threat Model Projekt (PDF)](portfolio/projects/Project_eBay_Threat_Modeling_DE.pdf) · [Microsoft Threat Modeling Tool — Screenshot](portfolio/screenshots/Ebay_Threat_Model_Tool_Screenshot.jpg)

---

### 4. 🔵 ASUS TUF-AX3000 V2 — Hardware-Recovery (SPI Flash & UART)

> Low-Level Firmware-Wiederherstellung eines vollständig „gebrickten" Routers durch physische Flash-Programmierung und serielle Konsolendiagnose.

- **Szenario:** Der Router wurde nach einem fehlgeschlagenen Firmware-Update funktionsunfähig („bricked"), ohne Möglichkeit einer Software-basierten Wiederherstellung.
- **Methodik:**
  - **SPI-Flash-Recovery** mittels CH341A-Programmer und SOIC8-Testclip — direktes physisches Lesen/Schreiben auf den Flash-Chip
  - Zugriff auf den **U-Boot Bootloader** über UART-Schnittstelle (PuTTY, 115200 Baud) zur Diagnose
  - Durchführung eines **TFTP-Firmware-Flash** über die Bootloader-Konsole zur Wiederherstellung der Original-Firmware
- **Ergebnis:** Vollständig dokumentierte Schritt-für-Schritt-Anleitung. Router erfolgreich wiederhergestellt. Demonstriert Hardware-nahe Troubleshooting-Fähigkeiten, direkt anwendbar auf IoT/OT-Sicherheit und forensische Analyse.

📄 **Dokumentation:** [Hardware-Recovery Präsentation (PDF)](portfolio/presentations/Presentation_ASUS_Router_SPI_Recovery_DE.pdf)

---

### 5. 🟢 Blue Team Homelab — Custom Workstation Architektur

> Zweckgebaut entworfene Cybersicherheits-Workstation als stabile Grundlage für Blue-Team-Studien, Virtualisierung und sichere Remote-Arbeit.

- **Szenario:** Entwurf und Bau einer leisen, leistungsstarken und thermisch optimierten Workstation für Verkehrsanalyse, VM-basierte Labore und kontinuierliche Sicherheitsstudien.
- **Methodik:**
  - Behebung einer **BIOS/Firmware-Inkompatibilität** zwischen MSI B450 Tomahawk MAX und einem neueren AMD Ryzen Prozessor durch manuelles BIOS-Flashing mit temporärem Prozessor
  - Entwicklung eines **Push-Pull-Airflow** mit Arctic-Lüftern und Erstellung benutzerdefinierter **PWM-Lüfterkurven** im BIOS für nahezu geräuschlosen „Ninja-Modus"-Betrieb
  - Integration von Multi-Generationen-Hardware (Sound BlasterX, XFX Radeon, Wi-Fi/BT-Modul) in ein Xilent Beam Aquarium-Gehäuse
  - Lösung eines **Spannungskonflikts** zwischen 5V ARGB und 12V RGB Standards durch Auslagerung des Beleuchtungssystems auf ein dediziertes Control Panel
  - Diagnose und Behebung von **MSI Center vs. BIOS Prioritätskonflikten** zugunsten einer stabilen Hardware-Steuerung
- **Ergebnis:** Perfekt funktionierende, thermisch effiziente und kabeloptimierte Workstation, bereit für Netzwerkverkehrsanalyse, VM-Ausführung und stabilen Dauerbetrieb.

📄 **Dokumentation:** [Homelab Projekt (PDF)](portfolio/projects/Project_Blue_Team_Homelab_Build_DE.pdf) · [Architektur-Bericht (PDF)](portfolio/projects/Report_Homelab_Architecture_DE.pdf) · [Engineering Präsentation (PDF)](portfolio/presentations/Presentation_Homelab_Engineering_DE.pdf)

---

## 🎓 Ausbildung & Zertifizierungen

| Zertifizierung | Anbieter | Zeitraum | Details |
|---|---|---|---|
| 🏆 **Cyber Security Fundamentals** | Robot Dreams | Jan – Mär 2026 | 97 % (193/200 Punkte) · Top 4 von 19 · 14 Wochen intensiv |
| ✅ **Pre Security Learning Path** | TryHackMe | März 2026 | 19 Stunden · Netzwerke, Linux, Web, Sicherheitsgrundlagen |
| 🔧 **Elektromechaniker für Maschinen** | Technische Schule, Subotica (Serbien) | 2001 – 2004 | Elektronik, Mechanik, Schaltpläne, technische Wartung |

**Aktuell angestrebt:** CompTIA Security+ · ISO 27001

### Nachweise

| Nachweis | Vorschau |
|---|---|
| Robot Dreams — Cybersecurity Zertifikat (mit Auszeichnung) | [Zertifikat anzeigen](portfolio/certifications/Robot_Dreams_Cybersecurity_Zertifikat.jpg) |
| TryHackMe — Pre Security Zertifikat | [Zertifikat anzeigen](portfolio/certifications/TryHackMe_Pre_Security_Zertifikat.jpg) |

---

## 🌍 Sprachen

| Sprache | Niveau |
|---|---|
| 🇭🇺 Ungarisch | Muttersprache |
| 🇩🇪 Deutsch | Gut in Wort und Schrift |
| 🇷🇸 Serbisch | Fließend |

---

## 💼 Beruflicher Hintergrund

**Über 10 Jahre** als Baumaschinenmechatroniker bei **Collé Rental & Sales** — systematische Fehlerdiagnose an komplexen elektronischen Systemen, Durchführung von Sicherheitsprüfungen (DGUV/TRBS-Compliance) und technische Dokumentation. Kompetenzen, die direkt auf SOC-Operationen, Log-Analyse und IT-Sicherheitsaudits übertragbar sind.

---

## 📁 Repository-Struktur

```
📦 cybersecurity-portfolio
├── 📄 README.md
└── 📂 portfolio/
    ├── 📂 projects/
    │   ├── Report_Rhadamanthys_Infostealer_DE.pdf
    │   ├── Project_Colle_Incident_Response_Plan_DE.pdf
    │   ├── Project_eBay_Threat_Modeling_DE.pdf
    │   ├── Project_Blue_Team_Homelab_Build_DE.pdf
    │   └── Report_Homelab_Architecture_DE.pdf
    ├── 📂 presentations/
    │   ├── Portfolio_SOC_Analyst_Viktor_Vas_DE.pdf
    │   ├── Presentation_Rhadamanthys_Analysis_DE.pdf
    │   ├── Presentation_Colle_Security_Blueprint_DE.pdf
    │   ├── Presentation_ASUS_Router_SPI_Recovery_DE.pdf
    │   └── Presentation_Homelab_Engineering_DE.pdf
    ├── 📂 infographics/
    │   └── Infographic_Defense_in_Depth_Architecture_DE.png
    ├── 📂 screenshots/
    │   └── Ebay_Threat_Model_Tool_Screenshot.jpg
    └── 📂 certifications/
        ├── Robot_Dreams_Cybersecurity_Zertifikat.jpg
        └── TryHackMe_Pre_Security_Zertifikat.jpg
```

---

<div align="center">

*Mit Disziplin gebaut. Durch Präzision angetrieben. Bereit zur Verteidigung.*

[![E-Mail](https://img.shields.io/badge/Kontakt-hucicok%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hucicok@gmail.com)

</div>
