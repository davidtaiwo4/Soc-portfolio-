# Tier 1 Security Operations Portfolio

## Objective
Hi, I'm Taiwo. This repository serves as a central portfolio showcasing my hands-on Security Operations Center (SOC) projects. I am a graduate with hands-on experience in incident response and security monitoring. Skilled in reconstructing attacker activity from logs, mapping techniques to the MITRE ATT&CK framework and incidence response. Experienced in producing clear, evidence-based incident reports, risk documentation and remediation recommendations. These projects show my ability to monitor logs, analyze alerts, triage and investigate basic security incidents using tools commonly used in real-world environments.


---

## Tools & Technologies

**SIEM & Detection:** Splunk, Sigma, Zeek, Suricata
**Programming & Data:** Python, DuckDB, pytest, Jinja2, STIX
**Network & Infrastructure:** Wireshark, NetworkMiner, Nmap, containerlab, FRRouting, nftables, Docker, WSL2
**Operating Systems:** Windows, Linux (Ubuntu, Kali)
**Frameworks:** MITRE ATT&CK, NIST SP 800-61 (PICERL), NIST CSF 2.0, ISO 27001:2022

### Threat Intelligence & Investigation
- **Email analysis:** Google Messageheader Analyzer, EML Analyzer
- **Reputation & URL analysis:** VirusTotal, URLScan.io, Cisco Talos
- **Infrastructure recon:** Whois/RDAP, crt.sh, Shodan
- **Sandboxing:** ANY.RUN

### Detection & Hunting
- Python, DuckDB, pytest
- MITRE ATT&CK mapping

---

## Projects

### 1. Incident Timeline Reconstruction & Response 
Description:
Rebuilt a full incident (host logs, phishing email, packet capture) into a single deterministic timeline via an automated pipeline; independently verified data exfiltration through two separate reconstruction methods, resolved a 23h46m clock drift across sources, and wrote/tested detection rules (Sigma, Zeek) with a controlled containment workflow.

Skills: incident triage, timeline reconstruction, IOC extraction, detection rules, escalation

🔗 [View Project](https://github.com/davidtaiwo4/Incident-Timeline-Reconstruction-and-Response-)

### 2. Hunt Engine: Threat Hunting at Scale

Built from scratch in Python, DuckDB and pytest. Ingested about 750,000 JSONL events from five sources, normalised three schema versions, reconstructed three attack campaigns and classified 96 review candidates (80 true positive, 16 false positive). 47+ passing tests. Caught a duplicated log source (one file byte-identical to another) with a SHA256 comparison.

Skills: threat hunting, log normalisation, campaign reconstruction, TP/FP triage, automated testing

[View Project](<LINK>)

### 3. Detection Engineering: 12 ATT&CK Rules

Wrote twelve ATT&CK technique detections in Python against a Windows event replay. Includes a versioned event adapter, a sequence and time-window correlation helper backing six rules, and a six-state regression harness with JUnit XML output.

Skills: detection engineering, ATT&CK mapping, correlation logic, regression testing

[View Project](<LINK>)

### 4. Network Range as Code

Defined a seven-zone enterprise network entirely as code on WSL2 using containerlab, FRRouting, nftables and Suricata, with a Jinja2 render pipeline driven by a single `variant.yml`. 30/30 tests passing, four fault-injection and recovery cycles evidenced with nftables counters, and a custom Suricata detection rule.

Skills: network segmentation, firewall policy, IDS rules, infrastructure as code, fault injection

[View Project](<LINK>)

### 5. Honeypot Threat Analysis

Analysed a 250,000-row honeypot dataset (T-Pot) with a reproducible Python pipeline: ingest, normalise, sessionise, cluster, hash, STIX export and detections. Found `connection_id` unreliable across schema versions; payload-hash co-occurrence was the only discriminating clustering signal. Made STIX output reproducible by deriving timestamps from sensor time.

Skills: honeypot analysis, behavioural clustering, STIX threat intelligence, reproducible pipelines

[View Project](<LINK>)


## Foundation Labs & Investigations

### SSH Brute-Force Detection (Splunk)
Ran a Hydra attack from Kali against an Ubuntu server and detected it in Splunk: failed-login spikes, attacker IP, targeted usernames, the successful login and a timeline.
🔗 [View Project](https://github.com/davidtaiwo4/Log-Monitoring-Threat-Detection/blob/main/README.md)

### Phishing Email Analysis
Header, authentication, URL and IP analysis of an impersonation email, with IOC extraction, ATT&CK mapping and an evidence-based classification.
🔗 [View Project](https://github.com/davidtaiwo4/Phishing-Email-Analysis)

### Network Traffic Analysis
Analyzed network traffic using Wireshark to detect suspicious patterns and potential threats. This project focuses on identifying malicious activity through packet inspection and protocol analysis. Forensic analysis of the packet-capture: isolated the chat, reconstructed the TCP stream, carved a transferred document and cross-checked with NetworkMiner.
🔗 [View Project](https://github.com/davidtaiwo4/network-traffic-analysis)

### Splunk Home Lab
Ubuntu Splunk server with a Windows Universal Forwarder, log ingestion and dashboards. Foundation for the brute-force detection project.
🔗 [View Project](https://github.com/davidtaiwo4/Splunk-home-lab-set-up)

---

## Skills

- Incident response and timeline reconstruction
- Detection engineering and rule testing
- Threat hunting and log analysis
- Network traffic and forensic analysis
- Phishing and threat intelligence investigation
- Incident documentation and reporting
---

### Notes
This portfolio is continuously updated as new projects and scenarios are completed, reflecting ongoing learning and practical skill development in cybersecurity and SOC operations.
<!--
**davidtaiwo4/davidtaiwo4** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
