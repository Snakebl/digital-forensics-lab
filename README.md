# Digital Forensics Investigation Lab

## Overview
This repository documents the digital forensics investigations, methodologies, and 
technical lab exercises completed during my Forensic Evidence Collection and Advanced 
Digital Forensics coursework at Stevenson University. All investigations follow 
forensically sound procedures, maintaining evidence integrity and chain of custody.

## Important Note
All case data used in these investigations is either simulated or publicly available 
training material. No real victim data, organizational data, or personally identifiable 
information is included in this repository.

## Investigations Completed

### 1. Disk Image Forensic Analysis
**Objective:** Recover deleted files, trace user activity, and identify malware artifacts

**Methodology:**
- Acquired forensic disk images using FTK Imager with MD5 hash verification
- Performed file carving and deleted file recovery using Autopsy
- Analyzed NTFS file records, including MFT entries and MACB timestamps
- Identified malware artifacts and traced execution history through registry analysis
- Documented findings in DELREX (Digital Examination Laboratory Report) format

**Tools Used:** FTK Imager, Autopsy, Magnet AXIOM, OSForensics, Ez Viewer

---

### 2. Memory Forensics Analysis
**Objective:** Identify running processes, detect malware, and analyze volatile memory

**Methodology:**
- Acquired RAM dumps and pagefile data from target systems
- Used the Volatility framework to enumerate running processes and identify anomalies
- Analyzed parent-child process relationships to detect process injection
- Identified WannaCry ransomware artifacts in memory
- Cross-referenced findings with disk artifacts for a comprehensive timeline

**Tools Used:** Volatility, Magnet AXIOM

---

### 3. Mobile Device Forensics (iOS)
**Objective:** Extract and analyze evidence from an iPhone logical filesystem backup

**Methodology:**
- Utilized a Lockdown Certificate to authorize acquisition from the iPhone 6 backup
- Analyzed logical filesystem dump using Magnet AXIOM Examine
- Recovered browser cookies, images, and application data
- Documented artifacts with timestamps for timeline reconstruction

**Tools Used:** Magnet AXIOM Examine, FTK Imager

---

### 4. Network Traffic and Phishing Analysis
**Objective:** Analyze malicious email and network traffic for indicators of compromise

**Methodology:**
- Examined email headers and raw .eml file to identify spoofed sender
- Extracted and defanged the malicious URL from the phishing email body
- Identified an impersonated trusted entity (Home Depot) used in a lure
- Captured and analyzed network traffic using Wireshark
- Documented IOCs for threat intelligence reporting

**Tools Used:** Wireshark, email analysis tools

---

### 5. Windows Registry and Timeline Analysis
**Objective:** Trace user activity and establish a forensic timeline from registry artifacts

**Methodology:**
- Analyzed Windows registry hives using Registry Explorer, ShellBag Explorer, 
  AppCompatCache Parser, and RegRipper
- Identified evidence of program execution, file access, and USB activity
- Used Plaso (log2timeline.py) to create super timelines from disk images
- Filtered and analyzed events using psort.py
- Visualized timeline data in Timesketch

**Tools Used:** Registry Explorer, ShellBag Explorer, AppCompatCache Parser, 
RegRipper, Plaso, Timesketch

---

### 6. MBR and File System Repair
**Objective:** Repair corrupted Master Boot Record and verify file system integrity

**Methodology:**
- Used HxD hex editor to identify and repair corrupted MBR bytes
- Verified repaired file system readability using FTK Imager
- Documented byte-level changes and recovery methodology

**Tools Used:** HxD, FTK Imager

---

### 7. Network Monitoring Tool — Raspberry Pi IDS
**Objective:** Build a low-cost real-time network monitoring and intrusion detection tool

**Methodology:**
- Configured Raspberry Pi as a passive network monitoring node
- Implemented real-time traffic capture and alert generation
- Tested detection capability against simulated network anomalies
- Documented build process and detection methodology

**Tools Used:** Raspberry Pi, Wireshark, custom scripts

---

## Forensic Documentation Standards
All investigations follow:
- IACIS Code of Ethics
- Stevenson University Digital Forensics Lab examination templates
- DELREX (Digital Examination Laboratory Report of Examination) format
- Chain of custody documentation requirements
- Hash verification at acquisition and analysis stages

## Tool Proficiency Summary
| Category | Tools |
|---|---|
| Acquisition | FTK Imager, dc3dd, Magnet AXIOM |
| Analysis | Autopsy, Magnet AXIOM Examine, OSForensics |
| Memory | Volatility |
| Registry | Registry Explorer, ShellBag Explorer, RegRipper, AppCompatCache Parser |
| Timeline | Plaso, psort, Timesketch |
| Network | Wireshark |
| Hex Editing | HxD |
| Reporting | DELREX format, Stevenson University templates |

## Certifications Supporting This Work
- Digital Forensic Examiner
- Digital Media Collector
- ISC2 Certified in Cybersecurity (CC)
- BCR SOC Operations Analyst I

## Academic Context
Courses: Forensic Evidence Collection Tools and Techniques, Advanced Digital Forensics
Institution: Stevenson University, B.S. Cybersecurity and Digital Forensics
