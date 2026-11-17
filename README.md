
<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=48&duration=3000&pause=1000&color=00FF41&center=true&vCenter=true&repeat=true&width=800&height=70&lines=%3E+SputikOS;%3E+Security+Without+Borders" alt="SputnikOS"/>

**ZERO TRUST • OPEN-SOURCE**

<br/>

*Privacy is a right. Security is a responsibility.*
*Knowledge is our greatest defense. Open source is our foundation.*

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-SputnikOS-181717?style=flat-square&logo=github)](https://github.com/sputnikOS)
[![Linux](https://img.shields.io/badge/Linux-Systems-FCC624?style=flat-square&logo=linux&logoColor=black)](https://kernel.org/)
[![Open Source](https://img.shields.io/badge/Open%20Source-First-3DA639?style=flat-square&logo=opensourceinitiative&logoColor=white)](https://opensource.org/)
[![Security](https://img.shields.io/badge/Security-By%20Design-00FF41?style=flat-square&logo=shield&logoColor=black)](#)

<br/>

![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=flat-square&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00878F?style=flat-square&logo=arduino&logoColor=white)
![RTL-SDR](https://img.shields.io/badge/RTL--SDR-333333?style=flat-square)
![GNU Radio](https://img.shields.io/badge/GNU%20Radio-FF6600?style=flat-square)
![Meshtastic](https://img.shields.io/badge/Meshtastic-333333?style=flat-square)
![ATAK](https://img.shields.io/badge/ATAK-263238?style=flat-square)

<br/>


</div>

---

## 01 / MISSION

SputnikOS is an open-source initiative focused on cybersecurity, resilient infrastructure, and digital independence.

We believe technology should empower individuals, strengthen communities, and remain accessible to everyone.

Our work explores the intersection of Linux, open-source intelligence, network defense, embedded systems, and privacy-focused infrastructure.

## 02 / CORE PRINCIPLES

| Principle | Philosophy |
|:---|:---|
| **Security by Design** | Build security into every layer, not as an afterthought. |
| **Digital Sovereignty** | Own your infrastructure. Control your data. Understand your technology. |
| **Defense in Depth** | Trust no single safeguard. Build resilience through layered protection. |
| **Open Knowledge** | Share knowledge, develop openly, and make technology accessible. |
| **Continuous Learning** | Understand the systems we use, challenge assumptions, and improve constantly. |

---

## 03 / NETWORK AUDIT

Practical Linux commands for auditing and monitoring networks you own or are authorized to assess.

### Install essential tools

```bash
sudo dnf install nmap wireshark-cli tcpdump arp-scan
```

### Network discovery

```bash
# Identify local network configuration
ip -br addr
ip route

# Inspect neighboring devices
ip neigh

# Discover active hosts on your LAN
sudo nmap -sn 10.0.0.0/24

# Inspect common TCP services on your gateway
sudo nmap -sT -sV --top-ports 100 10.0.0.1

# Inspect all TCP ports on an authorized target
sudo nmap -sT -p- --reason 10.0.0.1
```

### Traffic monitoring

```bash
# Capture network traffic
sudo tcpdump -i any -nn

# Monitor DNS traffic
sudo tcpdump -i any -nn port 53

# Monitor active listening services
sudo ss -tulpn

# Inspect running services
systemctl --type=service --state=running

# Monitor network traffic interactively
sudo wireshark
```

### Host inspection

```bash
# Inspect processes consuming the most CPU
ps aux --sort=-%cpu | head -20

# Inspect active network connections
ss -tunap

# Review system logs
sudo journalctl -p warning -b
```

> Only scan external IP addresses and networks when you have explicit authorization.

---

## 04 / SECURITY FRAMEWORKS & KNOWLEDGE

A curated collection of frameworks, documentation, and technical references.

### Security frameworks

| Resource | Description |
|:---|:---|
| [MITRE ATT&CK](https://attack.mitre.org/) | Adversary tactics and techniques |
| [MITRE Training](https://attack.mitre.org/resources/learn-more-about-attack/training/) | Security training and education |
| [OSINT Framework](https://osintframework.com/) | Open-source intelligence resources |
| [SANS Blue Team Wiki](https://github.com/sans-blue-team/blue-team-wiki) | Defensive security knowledge |
| [Red Hat Security Guide](https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/9/html/security_hardening/) | Linux security hardening |
| [Awesome Threat Intelligence](https://github.com/hslatman/awesome-threat-intelligence) | Threat intelligence resources |

### Development & security research

| Resource | Description |
|:---|:---|
| [Kali Linux Tools](https://www.kali.org/tools/) | Penetration testing toolkit |
| [Awesome Python](https://github.com/vinta/awesome-python) | Python ecosystem |
| [OSCP Resources](https://github.com/0xsyr0/OSCP) | Offensive security learning |
| [Exploit Database](https://www.exploit-db.com/) | Public vulnerability research |
| [VulnHub](https://www.vulnhub.com/) | Vulnerable lab environments |

---

## 05 / HARDWARE & EMBEDDED SYSTEMS

Open-source hardware, portable computing, and independent infrastructure.

| Platform | Application |
|:---|:---|
| [Raspberry Pi](https://www.raspberrypi.com/) | Edge computing and network infrastructure |
| [Arduino](https://www.arduino.cc/) | Embedded systems and hardware prototyping |
| [RTL-SDR](https://www.rtl-sdr.com/) | Software-defined radio experimentation |
| [GNU Radio](https://www.gnuradio.org/) | Signal processing and SDR development |
| [Meshtastic](https://meshtastic.org/) | Decentralized mesh communications |
| [ATAK](https://www.civtak.org/) | Situational awareness and geospatial tools |

### Hardware projects

- [P4wnP1 A.L.O.A.](https://github.com/RoganDawes/P4wnP1_aloa) — Raspberry Pi-based USB security research platform.
- [Raspberry Pi](https://github.com/raspberrypi) — Open hardware and software ecosystem.
- [Meshtastic](https://github.com/meshtastic) — Open-source mesh networking.

---

## 06 / SIGNALS INTELLIGENCE & GEOINT

Open-source signal analysis, radio experimentation, and geospatial intelligence.

| Resource | Description |
|:---|:---|
| [GNU Radio](https://wiki.gnuradio.org/) | Software-defined radio framework |
| [WebSDR](http://websdr.org/) | Web-accessible radio receivers |
| [RTL-SDR](https://www.rtl-sdr.com/) | Affordable SDR hardware and experimentation |
| [QGIS](https://qgis.org/) | Open-source geographic information systems |
| [ArcGIS](https://www.arcgis.com/) | Geospatial intelligence and mapping |

---

## 07 / PENETRATION TESTING ENVIRONMENT

A modular environment for security research, penetration testing, and defensive validation.

<details>
<summary><strong>01 — Virtualization & Lab Infrastructure</strong></summary>

<br/>

| Platform | Purpose |
|:---|:---|
| [VMware Workstation](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion) | Desktop virtualization |
| [VirtualBox](https://www.virtualbox.org/) | Open-source virtualization |
| [WSL2](https://learn.microsoft.com/en-us/windows/wsl/) | Linux environment within Windows |

</details>

<details>
<summary><strong>02 — Security Distributions</strong></summary>

<br/>

| Distribution | Purpose |
|:---|:---|
| [Fedora](https://fedoraproject.org/) | Modern Linux workstation |
| [Debian](https://www.debian.org/) | Stable Linux infrastructure |
| [Arch Linux](https://archlinux.org/) | Customizable Linux environment |
| [Kali Linux](https://www.kali.org/) | Penetration testing |
| [BlackArch](https://blackarch.org/) | Security research distribution |

</details>

<details>
<summary><strong>03 — Security Toolkits</strong></summary>

<br/>

| Category | Tools |
|:---|:---|
| **Reconnaissance** | [Nmap](https://nmap.org/), [Masscan](https://github.com/robertdavidgraham/masscan), [Recon-ng](https://github.com/lanmaster53/recon-ng) |
| **Exploitation** | [Metasploit](https://github.com/rapid7/metasploit-framework), [Empire](https://github.com/BC-SECURITY/Empire) |
| **Network Analysis** | [Wireshark](https://www.wireshark.org/), [Tcpdump](https://www.tcpdump.org/), [Burp Suite](https://portswigger.net/burp) |
| **Web Security** | [OWASP ZAP](https://www.zaproxy.org/), [Burp Suite](https://portswigger.net/burp), [Nuclei](https://github.com/projectdiscovery/nuclei) |
| **Digital Forensics** | [Autopsy](https://www.autopsy.com/), [Volatility](https://github.com/volatilityfoundation/volatility3) |
| **OSINT** | [SpiderFoot](https://github.com/smicallef/spiderfoot), [theHarvester](https://github.com/laramies/theHarvester) |
| **Vulnerability Research** | [Exploit Database](https://www.exploit-db.com/), [VulnHub](https://www.vulnhub.com/) |
| **Defensive Security** | [Wazuh](https://github.com/wazuh/wazuh), [Suricata](https://github.com/OISF/suricata), [Zeek](https://github.com/zeek/zeek) |

</details>

<details>
<summary><strong>04 — Linux Hardening & Privacy</strong></summary>

<br/>

| Project | Purpose |
|:---|:---|
| [Lynis](https://github.com/CISOfy/lynis) | Linux security auditing |
| [OpenSCAP](https://www.open-scap.org/) | Security compliance assessment |
| [Firejail](https://github.com/netblue30/firejail) | Application sandboxing |
| [SELinux](https://github.com/SELinuxProject) | Mandatory access control |
| [WireGuard](https://www.wireguard.com/) | Modern VPN protocol |
| [Proton](https://proton.me/) | Privacy-focused services |
| [Signal](https://signal.org/) | End-to-end encrypted communications |

</details>

---

## 08 / CAPABILITIES 

Our development priorities center around five interconnected areas:

- **Secure Infrastructure** — Hardened Linux systems, network defense, and resilient home infrastructure.
- **Open-Source Intelligence** — Research, collection, analysis, and responsible information gathering.
- **Embedded Systems** — Raspberry Pi, Arduino, SDR, and open-source IoT.
- **Digital Privacy** — Encryption, secure communications, and personal data sovereignty.
- **Security Education** — Documentation, practical labs, and accessible technical knowledge.

---

<div align="center">

<br/>

**SPUTNIKOS**

*Knowledge Without Borders.*

`OPEN SOURCE` · `DIGITAL SOVEREIGNTY` · `DEFENSE IN DEPTH`

<br/>

[![GitHub](https://img.shields.io/badge/Explore%20Projects-181717?style=for-the-badge&logo=github)](https://github.com/sputnikOS)

<br/>

<sub>Built on open knowledge. Strengthened through shared innovation.</sub>

</div>
