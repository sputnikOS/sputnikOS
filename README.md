
<div align="center">


  [![Typing SVG](https://readme-typing-svg.demolab.com?font=Source+Code&weight=700&size=72&duration=3000&pause=1000&color=00FF41&center=true&vCenter=true&multiline=true&repeat=true&width=700&height=80&lines=%3E+SputikOS;%3E+Zero-Trust+%3A%3A+Open-Source;)](https://github.com/sputnikOS)

 `>> “Privacy is a right. Security is a responsibility. Knowledge is our greatest defense. Open source is our foundation." <<` 




![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-C51A4A?style=flat-square&logo=raspberrypi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00878F?style=flat-square&logo=arduino&logoColor=white)
![RTL SDR](https://img.shields.io/badge/RTL--SDR-444444?style=flat-square)
![GNU Radio](https://img.shields.io/badge/GNU_Radio-FF6600?style=flat-square)
![Meshtastic](https://img.shields.io/badge/Meshtastic-333333?style=flat-square)
![ATAK](https://img.shields.io/badge/ATAK-263238?style=flat-square)



<br/>


<a href="https://github.com/sputnikOS/sputnikOS/blob/main/Mission%20Statement.md">
  <img src="https://img.shields.io/badge/Mission_Statement-111827?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="Knowledge Without Borders"/>
</a>

## Audit your network
`sudo dnf install nmap wireshark-cli tcpdump`


###### scan
`Ip route && ip neigh`

`sudo nmap -sn 10.0.0.0/24`
`sudo nmap -sT -sV --top-ports 100 10.0.0.1`
`sudo nmap -sT -p- --reason 10.0.0.1`
`nmap -sT --top-ports 100 PUBLIC_IP`
###### monitor 
`sudo wireshark`
`sudo arp-scan --localnet`
`sudo tcpdump -i any -nn`
`sudo tcpdump -i any -nn port 53` (DNS)

`ss -tulpn` or `ps aux --sort=-%cpu | head -20`
`systemctl --type=service --state=running` (most CPU)


## Frameworks 
### 
[MITRE Framework](https://attack.mitre.org/)
[MITRE Training](https://attack.mitre.org/resources/learn-more-about-attack/training/)

[OSINT Framework](https://osintframework.com/)

[Red Hat Linux Security Guide](https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/7/html/security_guide/index)

[SANS Blue Team Wiki](https://github.com/sans-blue-team/blue-team-wiki/)


[Tools List](https://www.kali.org/tools/)
[Python](https://github.com/vinta/awesome-python?tab=readme-ov-file#distributed-computing)

[Kali Linux](https://github.com/0xsyr0/OSCP)

[Threat Intelligence](https://github.com/hslatman/awesome-threat-intelligence)

### Hardware 
[P4WN Aloha](https://github.com/sputnikOS/P4wnP1_aloa)

### Signals Intelligence (SIGINT)
[GNU Radio](https://wiki.gnuradio.org/)

[WebSDR](http://websdr.org/)

[ArcGis](https://www.arcGis.com)


  ## 🚀 Penetration Testing Environment

  <details>
  <summary><strong>Click to expand toolkit list</strong></summary>
  <br>

  ### 💻 Install VMWare/Virtualbox on your windows machine. Alternatively, you can use WSL.
  <a href="https://www.vmware.com/products/workstation-player/">
    <img src="https://img.shields.io/badge/VMware-231f20?style=for-the-badge&logo=VMware&logoColor=white" alt="VMware">
  </a>
  <a href="https://www.virtualbox.org/wiki/Downloads">
    <img src="https://img.shields.io/badge/VirtualBox-21416b?style=for-the-badge&logo=VirtualBox&logoColor=white" alt="VirtualBox">
  </a>

  ### 🖥️ Virtual Machines
  <a href="https://kali.org">
    <img src="https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white" alt="Kali Linux">
  </a>
  <a href="https://blackarch.org/downloads.html">
    <img src="https://img.shields.io/badge/BlackArch-000000?style=for-the-badge&logo=arch-linux&logoColor=white" alt="BlackArch">
  </a>

  ### 🐧 Core Operating Systems
  <a href="https://www.debian.org/download">
    <img src="https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white" alt="Debian">
  </a>
  <a href="https://ubuntu.com/download">
    <img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" alt="Ubuntu">
  </a>
  <a href="https://archlinux.org/download/">
    <img src="https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white" alt="Arch Linux">
  </a>
  
  | Category | Tools |
  | :--- | :--- |
  | **Exploitation** | [Metasploit](https://github.com/rapid7/metasploit-framework), [Metasploitable3](https://github.com/rapid7/metasploitable3), [Empire](https://github.com/EmpireProject/Empire), [Powersploit](https://github.com/PowerShellMafia/PowerSploit), [Nishang](https://github.com/samratashok/nishang) |
  | **Reconnaissance** | [Nmap](https://nmap.org), [Netdiscover](https://www.kali.org/tools/netdiscover/), [Masscan](https://github.com/robertdavidgraham/masscan), [Recon-ng](https://github.com/lanmaster53/recon-ng), [F-Society Toolkit](https://github.com/Manisso/fsociety) |
  | **Post-Exploitation** | [Mimikatz](https://github.com/ParrotSec/mimikatz), [Responder](https://github.com/SpiderLabs/Responder), [Veil Framework](https://github.com/Veil-Framework) |
  | **Network Analysis** | [Wireshark](https://www.wireshark.org/download.html), [Proxychains](https://github.com/haad/proxychains), [Burp Suite](https://portswigger.net/burp) |
  | **Web & Social Eng.** | [BeEF](https://github.com/beefproject/beef), [Social Engineer's Toolkit](https://github.com/trustedsec/social-engineer-toolkit) |
  | **Exploits** | [VulnHub](https://www.vulnhub.com/),  [ExploitDB](https://www.exploit-db.com/) |
  

  </details>

  
</div>

