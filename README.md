# My CyberSec and Forensics Roadmaps

---

# 🎯 HTB Junior Cybersecurity Analyst → Red Teamer + Blue Team Foundations

> Note: always operate **legally and ethically**. Only test systems and networks you own or have explicit written permission to test.

---

## Quick context
You’re completing the **Hack The Box — Junior Cybersecurity Analyst** path. This roadmap blends that analyst foundation into two career directions:
- **Red Team** (offensive) — adversary emulation, pen-testing, exploitation, AD attacks, C2
- **Blue Team** (defensive) — detection, incident response, DFIR, SIEM & EDR operations

Suggested timeline: **6–12 months** (flexible). Use HTB boxes and TryHackMe labs to practice both sides.

---

## Priority checklist (do these first)
- [ ] Finish HTB **Junior Cybersecurity Analyst** path boxes and challenges.
- [ ] Learn/refresh networking fundamentals (TCP/IP, ports, protocols).
- [ ] Get comfortable with **Linux** CLI and **Windows** basics (PowerShell, Event logs).
- [ ] Set up a personal lab (attacker VM, defender VM, target VMs including Windows AD VM).
- [ ] Keep an ethics/legal checklist and obtain written permission for any tests.

---

## Month 0–1 — Core foundations (both)
- [ ] Networking fundamentals: OSI model, TCP/UDP, common ports, DNS, DHCP
- [ ] OS basics:
  - Linux: filesystem, permissions, processes, sudo
  - Windows: registry, services, Event Viewer, PowerShell essentials
- [ ] Basic scripting: Bash and Python fundamentals
- [ ] Lab setup:
  - Kali / Parrot / equivalent attacker VM
  - Windows Server + client VMs for AD
  - Defender VM with SIEM/ELK or Splunk trial
- [ ] Tools to install / try:
  - Nmap — https://nmap.org/
  - Wireshark — https://www.wireshark.org/
  - Netcat — https://nc110.sourceforge.io/
  - PowerShell docs / learning — https://learn.microsoft.com/powershell/

---

## Month 2–3 — Dual-track fundamentals

### Offensive (Red)
- [ ] Recon & enumeration: Nmap, smbclient, enum4linux
- [ ] Basic web testing: Burp Suite basics (Community) — https://portswigger.net/burp
- [ ] Exploitation basics and payloads: Metasploit overview — https://www.metasploit.com/
- [ ] Practice HTB boxes focused on enumeration → exploit → post-exploit

### Defensive (Blue)
- [ ] Host & network logging basics: Windows Event Logs, Sysmon
- [ ] Packet capture and analysis: Wireshark fundamentals
- [ ] Intro to detection: what makes a detectable vs stealthy action
- [ ] Set up a simple SIEM pipeline (ELK / Splunk trial):
  - Elastic — https://www.elastic.co/
  - Splunk — https://www.splunk.com/
- [ ] Start learning MITRE ATT&CK mapping: https://attack.mitre.org/

---

## Month 4–5 — Intermediate skills & tooling

### Offensive
- [ ] Footholds & shells: reverse shells, persistence basics
- [ ] Local privilege escalation basics (Linux & Windows)
- [ ] Post-exploitation tools: Meterpreter, `msfvenom`, basics of payload generation
- [ ] Web exploitation common classes (sqli, xss, rce basics)
- [ ] Practice HTB / CTF write-ups for 3–5 boxes

### Defensive
- [ ] Endpoint detection & response (EDR) basics — concepts and telemetry
- [ ] Host forensics basics: Volatility memory analysis — https://www.volatilityfoundation.org/
- [ ] Endpoint query tooling: osquery — https://osquery.io/
- [ ] Open-source DFIR tooling: Velociraptor — https://www.velocidex.com/velociraptor/
- [ ] Network IDS/NSM basics: Zeek — https://zeek.org/ and Suricata — https://suricata.io/

---

## Month 6–7 — Active Directory & Incident Response

### Offensive (AD focus)
- [ ] Active Directory fundamentals: users, groups, trusts, Kerberos, LDAP
- [ ] AD attack basics: Kerberoasting, AS-REP roast, pass-the-hash/ticket concepts
- [ ] Tools: Impacket — https://github.com/SecureAuthCorp/impacket, BloodHound — https://github.com/BloodHoundAD/BloodHound
- [ ] Practice AD attack chains in a lab and document every step

### Defensive (IR focus)
- [ ] Incident response workflow: identification → containment → eradication → recovery
- [ ] Timeline & correlation: build timelines from logs (Windows, network, endpoint)
- [ ] Hunting fundamentals: hypotheses → queries → investigation
- [ ] Detection engineering: write Sigma rules (generic detection format) — https://sigmahq.org/
- [ ] Use Timesketch / Plaso for timeline reconstruction:
  - Timesketch — https://timesketch.org/
  - Plaso — https://plaso.readthedocs.io/en/latest/

---

## Month 8–9 — Red Team ops & Blue team scaling

### Offensive (Red Team ops)
- [ ] Command & Control concepts and safe labbed C2 frameworks (open-source alternatives):
  - Covenant — https://github.com/cobbr/Covenant
  - Mythic — https://github.com/its-a-feature/Mythic
  - PoshC2 — https://github.com/NetSPI/PoshC2
- [ ] Lateral movement at scale; persistence patterns and opsec considerations
- [ ] Emulate adversary techniques and map to MITRE ATT&CK coverage
- [ ] Create a red-team engagement template (ROE, scope, exfil simulation in lab)

### Defensive (Blue Team ops)
- [ ] SIEM rule creation and tuning (Splunk or ELK): ingest logs, reduce false positives
- [ ] Endpoint telemetry enrichment and EDR alert triage
- [ ] Threat hunting playbooks for common TTPs (mapped to ATT&CK)
- [ ] Purple-team exercises: run an attack in lab and iterate detection coverage

---

## Month 10 — Automation & tooling polish
- [ ] Automate common tasks with Python and PowerShell (reporting, detection queries)
- [ ] Build scripts to gather host/network telemetry for faster triage
- [ ] Harden lab infra: logging retention, secure collection pipelines
- [ ] Contribute small detection or red tool scripts to GitHub for your portfolio

---

## Month 11–12 — Certification, portfolio & job-ready artefacts
- [ ] Consider certification pathway:
  - Defensive: CompTIA Security+, CySA+ (CompTIA), Splunk Core or Splunk SOAR basics
  - Offensive: eJPT (eLearnSecurity) for beginners, OSCP (Offensive Security) later
- [ ] Build a portfolio:
  - 5+ detailed HTB/CTF write-ups (full steps + detection notes)
  - 1 AD attack lab write-up showing the full chain and mitigations
  - 1 red-team style engagement report (lab) + 1 blue-team detection report
- [ ] Prepare interview artifacts: sample detection queries, sample playbooks, incident timeline examples

---

## Ongoing practice (always)
- [ ] Regular HTB / TryHackMe / CTF practice (rotate offensive & defensive labs)
- [ ] Read detection & DFIR blogs; follow changelogs for offensive tooling
- [ ] Participate in Purple Team exercises and knowledge sharing
- [ ] Keep a learning journal / DB of commands, detection queries, privesc methods and mitigations

---

## Tools & resources (quick-links)

### Offensive tools
- Nmap — https://nmap.org/
- Metasploit — https://www.metasploit.com/
- Burp Suite — https://portswigger.net/burp
- Impacket — https://github.com/SecureAuthCorp/impacket
- BloodHound — https://github.com/BloodHoundAD/BloodHound
- Mimikatz — https://github.com/gentilkiwi/mimikatz
- Covenant — https://github.com/cobbr/Covenant
- Mythic — https://github.com/its-a-feature/Mythic
- PoshC2 — https://github.com/NetSPI/PoshC2

### Defensive / DFIR tools
- Wireshark — https://www.wireshark.org/
- Volatility — https://www.volatilityfoundation.org/
- osquery — https://osquery.io/
- Velociraptor — https://www.velocidex.com/velociraptor/
- Zeek — https://zeek.org/
- Suricata — https://suricata.io/
- Elastic (ELK) — https://www.elastic.co/
- Splunk — https://www.splunk.com/
- Timesketch — https://timesketch.org/
- Sigma rules — https://sigmahq.org/

### Learning platforms & references
- Hack The Box — https://www.hackthebox.com/
- TryHackMe — https://tryhackme.com/
- PortSwigger Web Security Academy — https://portswigger.net/web-security
- MITRE ATT&CK — https://attack.mitre.org/
- DFIR Training — https://www.dfir.training/

---

## Ethics & legal checklist (must do)
- [ ] Obtain **written authorization** for any engagement or test.
- [ ] Keep logs and evidence chain-of-custody for any authorized tests.
- [ ] When practicing C2 or offensive tooling, always isolate to your lab and never run on the public internet without permission.

---

## Suggested mini-projects (portfolio & learning)
- [ ] Full HTB box write-up (enumeration → exploitation → post-exploit) + detection notes for defenders
- [ ] AD chain-of-exploit lab with mitigation notes (show both attack steps and detection queries)
- [ ] Create 3 Sigma rules or SIEM searches to detect the behaviors you used in a lab attack
- [ ] Small C2 implant demo in a controlled lab (document detection & mitigation)

---

### TL;DR — How to prioritise
1. Finish HTB Junior Cybersecurity Analyst boxes → build confidence.  
2. Master networking, Linux, Windows fundamentals.  
3. Alternate offensive and defensive practice: for every attack lab, write detection rules and a response playbook.  
4. Focus on AD attacks and DFIR skills (both are high-value).  
5. Build write-ups and a portfolio showing *both* how you attack and how you detect/defend.  
6. Pick entry certs (eJPT / Security+ / CySA+) then progress to OSCP / advanced DFIR quals as needed.
 
---

# 🧭 Digital Forensics Roadmap (2025 Edition)

## Foundations & Core Concepts
- [ ] Understand **Digital Forensics Principles** ([NIST SP 800-101 Rev.1](https://csrc.nist.gov/publications/detail/sp/800-101/rev-1/final))
- [ ] Study **Evidence Handling & Chain of Custody** ([ACPO Guidelines](https://www.digital-detective.net/digital-evidence-the-acpo-principles/))
- [ ] Learn about **File Systems (NTFS, FAT32, EXT4)** ([File System Basics](https://www.geeksforgeeks.org/file-system-basics/))
- [ ] Explore **Operating Systems Forensics** ([Windows Forensics Guide](https://resources.infosecinstitute.com/topics/forensics/windows-forensics/))
- [ ] Install and configure forensic tools:
  - [Autopsy](https://www.autopsy.com/)
  - [FTK Imager](https://accessdata.com/product-download)
  - [Magnet AXIOM](https://www.magnetforensics.com/resources/download-magnet-axiom/)
  - [Caine Linux](https://www.caine-live.net/)
  - [SIFT Workstation](https://digital-forensics.sans.org/community/downloads)
- [ ] Practise **data acquisition** from USB and disk images
- [ ] Review **Digital Evidence Standards** ([Forensic Science Regulator Codes](https://www.gov.uk/government/collections/forensic-science-regulator-codes-of-practice-and-conduct))

---

## Analysis & Tools
- [ ] Learn **Memory Forensics** using [Volatility](https://www.volatilityfoundation.org/) or [Rekall](https://github.com/google/rekall)
- [ ] Practise **Network Capture Analysis** with [Wireshark](https://www.wireshark.org/)
- [ ] Extract and analyze **Mobile Data** using [Cellebrite Reader](https://www.cellebrite.com/en/downloads/)
- [ ] Practise **hashing & integrity verification** (MD5, SHA256) ([HashCalc](https://hashcalc.soft112.com/))
- [ ] Build a case using multiple evidence types
- [ ] Write **interim forensic reports** with clear methodology

---

## Advanced Practice & Reporting
- [ ] Practise full case workflow: Acquisition → Examination → Analysis → Reporting
- [ ] Conduct **timeline analysis** using [Autopsy](https://www.autopsy.com/) or [Plaso](https://plaso.readthedocs.io/en/latest/)
- [ ] Perform **keyword and metadata searches**
- [ ] Study **Forensic Reporting Standards** ([FSR Codes](https://www.gov.uk/government/collections/forensic-science-regulator-codes-of-practice-and-conduct))
- [ ] Review **ISO 17025 requirements** ([ISO Summary](https://www.iso.org/standard/66912.html))
- [ ] Conduct a **mock case review** and present findings
