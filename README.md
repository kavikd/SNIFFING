💙PRESENT ABOUT💙: KAVIARASAN 

<!-- ======================= BANNER ======================= -->
<h1 align="center">‼️🌎❌SNIFFING🌎❌‼️</h1>

<!-- ======================= BANNER ======================= -->
<h1 align="center">🧠🔍 Sniffing in Cyber Forensics</h1>
<h3 align="center">Seminar • Assignment • Case Study Ready Notes</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Cyber%20Security-Cyber%20Forensics-0A66C2?style=for-the-badge&logo=hackaday&logoColor=white"/>
  <img src="https://img.shields.io/badge/Topic-Packet%20Sniffing-16A085?style=for-the-badge&logo=wireshark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Level-Student%20Seminar-F39C12?style=for-the-badge&logo=readthedocs&logoColor=white"/>
  <img src="https://img.shields.io/badge/Use-Assignment%20%2B%20Presentation-8E44AD?style=for-the-badge&logo=googleclassroom&logoColor=white"/>
</p>

---

---

## 🔷 1. What is Sniffing?

Sniffing is a network surveillance technique where data packets traveling across a network are intercepted, captured, and examined.

In digital communication:
- Data is broken into packets
- Each packet travels independently
- Packets pass through switches, routers, and gateways

A sniffer:
- Captures packets
- Reads metadata
- Extracts useful information
- Reconstructs sessions

Sniffing = Eavesdropping on digital communication.

---

## 🔷 2. Types of Sniffing

### ✅ Passive Sniffing
Listening to traffic without altering it.

**How it works:**
- Common in hub-based networks
- Traffic is broadcast to all devices
- Sniffer captures packet copies

**Features:**
- No traffic modification
- No delay
- Hard to detect
- Very stealthy

**Uses:**
- Network diagnostics
- Performance monitoring
- Digital forensics

---

### ❌ Active Sniffing
Traffic is manipulated so packets pass through attacker’s device.

**Why needed?**
Switches send packets only to intended devices.
Attackers must trick the switch.

---

### ⚠️ Active Sniffing Techniques

#### 1️⃣ ARP Spoofing
- ARP maps IP → MAC
- Fake ARP replies sent
- Victim links attacker MAC to gateway IP
- Traffic redirected through attacker
- Enables Man-in-the-Middle attack

#### 2️⃣ MAC Flooding
- Switch stores MAC addresses in CAM table
- Attacker floods with fake MAC entries
- Table overflow occurs
- Switch behaves like hub
- All packets broadcast

#### 3️⃣ DNS Spoofing
- DNS converts domain → IP
- Fake DNS responses sent
- Victim redirected to malicious server
- Traffic can be sniffed or altered

---

## 🔷 3. Protocols Vulnerable to Sniffing

Protocols without encryption expose payload data.

| Protocol | Risk |
|---------|------|
| HTTP | Web content visible |
| FTP | Username & password exposed |
| Telnet | Remote login readable |
| SMTP | Email content visible |
| POP3 | Email retrieval exposed |
| SNMP v1/v2 | Device data exposed |

**Note:** Encrypted protocols like HTTPS, SSH, FTPS are safer.

---
### 📌 Definition of Packet Sniffing

**Packet sniffing** is the process of capturing, intercepting, and analyzing data packets as they travel across a computer network.

It enables monitoring of network traffic to examine:
- Source and destination addresses
- Protocol information
- Data being transmitted

Packet sniffing is used for:
- Network troubleshooting
- Performance monitoring
- Cyber security analysis
- Digital forensic investigations

If used maliciously, it can also be used to steal sensitive information from unencrypted traffic.

## 🔷 4. Forensic Significance of Sniffing

Sniffing plays a key role in Cyber Forensics.

### 🧪 Investigation Benefits
- Reconstructs communication sessions
- Identifies attacker IP addresses
- Tracks data exfiltration
- Detects unauthorized access
- Reveals attacker behavior

### 📁 Digital Evidence
- Packet capture files (PCAP)
- Network flow records
- Session timestamps
- Protocol logs
- Payload fragments

### ⚖️ Court Value
- Technical evidence
- Timeline proof
- Attack pattern record
- Proof of intent

---

## 🔷 5. How Investigators Detect Sniffers

### 🔍 Promiscuous Mode Detection
- Normal device → receives own packets only
- Sniffer → captures all packets
- NIC behavior analysis used

### 🔍 ARP Traffic Analysis
- High ARP reply frequency indicates spoofing

### 🔍 Duplicate IP Detection
- Same IP used by multiple MACs = MITM suspicion

### 🔍 Network Flow Anomalies
- Sudden rerouting
- Increased latency
- Packet duplication

### 🔍 IDS / IPS Alerts
- Signature-based detection
- Behavioral anomaly detection
- Suspicious packet pattern analysis

---
 ### Sniffing Tool — Wireshark

<p align="center">
  <img src="https://img.shields.io/badge/Tool-Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Type-Open%20Source-2ECC71?style=for-the-badge&logo=opensourceinitiative&logoColor=white"/>
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-34495E?style=for-the-badge&logo=windows&logoColor=white"/>
</p>

### 🛠️ Wireshark
- GUI-based packet analyzer
- Deep packet inspection
- Protocol decoding
- Stream reconstruction
- Forensic export support

### 🛠️ Tcpdump
- Command-line packet analyzer
- Lightweight and fast
- Real-time capture
- Advanced filtering
- Ideal for servers

---

# 🚨 Case Study — TJX Companies Data Breach (2007)

---

## 🏢 Parties Involved

### Victim
TJX Companies  
Multinational retail corporation.

### Attacker
Albert Gonzalez  
Leader of organized cybercrime group.

---

## ⚙️ Attack Method (Technical Flow)

1. Wireless reconnaissance
2. WEP encryption cracked
3. Packet sniffers deployed
4. Payment transaction interception
5. Credential harvesting
6. Corporate network infiltration
7. Malware and sniffers installed internally
8. Long-term traffic monitoring
9. Data exfiltration to remote servers

---

## 📉 Impact
- 45+ million payment card records stolen
- Massive financial losses
- Legal consequences
- Reputation damage

---

## ⚖️ Legal Judgment and Punishment
- Arrested by US authorities
- Charged with computer fraud and conspiracy
- Sentenced to 20 years imprisonment

---

## 🇮🇳 Relevant IT Law Sections (India)

Information Technology Act, 2000 (Amended 2008)

- Section 43 — Unauthorized access and data theft
- Section 65 — Source code tampering
- Section 66 — Computer-related offences
- Section 66B — Receiving stolen data
- Section 66C — Identity theft
- Section 66D — Online cheating

---

## 🧪 Forensic Takeaway

- Weak wireless security enables packet interception
- Sniffing allows silent data theft
- Encryption is essential
- Continuous monitoring is critical
- Early anomaly detection reduces damage

---

## 🕵️ How Investigators Found the Suspect  
### “Follow the Breadcrumbs” Method

- Fraud systems flagged unusual transactions
- Stolen card data traced to underground markets
- Server logs analyzed
- IP addresses tracked across networks
- ISP records identified suspect locations
- Wi-Fi hotspot logs correlated
- CCTV and hotel records verified presence
- Informants provided intelligence

Digital trail → Network identity → Physical identity

---

## ⏳ Case Timeline

- 2005 — Initial intrusion
- 2006 — Silent data theft
- 2007 — Breach discovered
- 2008 — Investigation expands
- 2009 — Arrest
- 2010 — Sentencing

**Total Duration:** ~5 years

---

# ✅ Conclusion

Sniffing is a double-edged sword.

Used ethically:
- Powerful diagnostic tool
- Helps forensic investigations
- Improves network performance

Used maliciously:
- Serious cyber threat
- Data theft
- Privacy invasion

Strong encryption and monitoring are essential in modern networks.
