<h1 align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=28&duration=3000&pause=1000&color=00E0A4&center=true&vCenter=true&width=600&lines=Hey%2C+I'm+Karan+Desai+%F0%9F%91%8B;Security+Engineer+%7C+Builder;Red+Team+%7C+Container+Security;GSoC+2026+Applicant+%E2%80%94+Metasploit" alt="Typing SVG" />
</h1>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=karandesai2005&label=Profile%20Views&color=00e0a4&style=flat-square" alt="karandesai2005" />
  <img src="https://img.shields.io/badge/eJPT-Certified-00e0a4?style=flat-square&logo=elearnsecurity" />
  <img src="https://img.shields.io/badge/GSoC%202026-Applicant-4285F4?style=flat-square&logo=google" />
  <img src="https://img.shields.io/badge/Open%20to-Internships-orange?style=flat-square" />
</p>

---

## 🧑‍💻 About Me

```
┌─────────────────────────────────────────────────────────┐
│  karan@security:~$ whoami                               │
│                                                         │
│  ▸ 3rd-year CS undergrad @ Symbiosis Institute of Tech  │
│  ▸ eJPT certified penetration tester                   │
│  ▸ GSoC 2026 applicant → Metasploit / Honeynet Project  │
│  ▸ Co-founded a startup, shipped to 100+ users         │
│  ▸ Building Maya: an autonomous deception framework     │
│  ▸ CTF player, home lab operator, open-source lurker   │
└─────────────────────────────────────────────────────────┘
```

- 🔐 I work at the intersection of **offensive security**, **container infrastructure**, and **systems programming**
- 🚀 GSoC 2026: Proposing **`build_vuln`** — automated vulnerable environment provisioning for Metasploit Framework (Ruby · Docker · Podman · OCI)
- 🎭 Currently designing **Maya**, an autonomous honeypot platform with CRDT-based state sync and MITRE ATT&CK mapping
- 🏴‍☠️ Regular **CTF player** (web, networking, forensics, OSINT)
- 📝 I write on [Medium](https://medium.com/@karanishudesai2) about networking, distributed systems, and security
- 📫 **desaikaran.me@gmail.com** · [Portfolio](https://karan-desai.vercel.app)

---

## 🌱 GSoC 2026 — Metasploit Framework

> **Project: Automated Vulnerable Environment Provisioning**
> Organisation: The Honeynet Project → Metasploit (Rapid7)

Metasploit ships hundreds of exploit modules but has **no first-class way to provision matching targets**. I'm building that:

| Component | Description |
|-----------|-------------|
| `vuln_env.yml` schema | Per-module YAML config declaring OCI image, ports, healthchecks |
| `build_vuln` command | New msfconsole command that spins up containers on demand |
| Rootless Podman support | Works on hardened machines without Docker Desktop |
| 10+ environment definitions | Shellshock, EternalBlue, Drupalgeddon2, HeartBleed, and more |
| GitHub Actions pipeline | Auto-builds and publishes images to `ghcr.io/rapid7/msf-vuln` |

```bash
msf6 exploit(linux/http/apache_mod_cgi_bash_env) > build_vuln
[*] Pulling ghcr.io/rapid7/msf-vuln/apache-shellshock:latest ...
[*] Starting container msf_vuln_abc123 ...
[+] Environment ready. Set RHOSTS 127.0.0.1, RPORT 8080
```

📄 [Read the full proposal](https://github.com/karandesai2005) · 🏗️ [Tracking issue (WIP)](https://github.com/karandesai2005)

---

## 🔨 Featured Projects

<table>
<tr>
<td width="50%">

### 🎭 Maya — Autonomous Deception Framework
`Security` · `Distributed Systems` · `ML`

Autonomous honeypot/deception platform that detects and contains post-compromise attackers using parallel shadow infrastructure.

- CRDT-based state sync for consistent attacker identity tracking across distributed nodes
- Adaptive responses based on observed attacker TTPs
- Full MITRE ATT&CK mapping for structured threat intel

</td>
<td width="50%">

### 🔒 Rootless — Secure Pentesting Console
`Electron` · `FastAPI` · `Go` · `Firejail`

Sandboxed pentesting console that isolates every tool execution using Firejail — no unsafe sudo, no VM overhead.

- Layered arch: Electron → FastAPI → Go execution engine
- Least-privilege model with per-session filesystem restrictions
- Process-level isolation as a first-class design constraint

</td>
</tr>
<tr>
<td width="50%">

### 🏠 Cybersecurity Home Lab
`Proxmox` · `pfSense` · `VLANs` · `Splunk`

Enterprise-grade virtualized lab with VLAN segmentation, firewall policies, and isolated attack/defense subnets.

- Wireshark traffic analysis + Splunk SIEM correlation
- Full exploitation → lateral movement → detection pipeline
- Simulated intrusion scenarios in a safe, controlled environment

</td>
<td width="50%">

### 📡 TraceProbe — Real-Time Log Analysis
`Apache Kafka` · `Apache Flink`

Streaming log ingestion and anomaly detection pipeline using Kafka for messaging and Flink for stateful processing.

- Alert rules surface suspicious patterns as they happen
- Reduced MTTD on simulated security events

</td>
</tr>
</table>

---

## 🛡️ Security Philosophy

```
> "If it needs sudo, it needs isolation."
> "Build for the attacker's perspective, not just the happy path."
> "Reproducibility is a security property."
```

I care deeply about:

- **Least privilege** — every process, every container, every API call
- **Attack surface reduction** — fewer moving parts, fewer failure modes
- **Reproducible environments** — ad-hoc setups are the enemy of good security testing
- **Fail safely** — design for breach, not just prevention

---

## 🧰 Tech Stack

### Languages
![Ruby](https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-121011?style=for-the-badge&logo=gnu-bash&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)

### Security & Infrastructure
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Podman](https://img.shields.io/badge/Podman-892CA0?style=for-the-badge&logo=podman&logoColor=white)
![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=for-the-badge&logo=proxmox&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596BE?style=for-the-badge&logo=metasploit&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)

### Backend & Systems
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)

---

## 📜 Certifications

- 🟢 **eJPT** — eLearnSecurity Junior Penetration Tester
- 🔵 **Google Cybersecurity Professional Certificate** (2024)
- ☁️ **Nutanix Hybrid Cloud Fundamentals** (2026)
- ☁️ **IBM Cloud Computing Fundamentals** (2026)
- 🔐 **Cybersecurity: Risk & Compliance** — University of San Diego (2024)

---
## 📊 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=karandesai2005&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" width="48%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=karandesai2005&theme=tokyonight&hide_border=true" width="48%" />
</p>
<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=karandesai2005&theme=matrix&margin-w=15&no-bg=true&no-frame=true" />
</p>

## 🔗 Connect

<p align="left">
  <a href="https://github.com/karandesai2005"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
  <a href="https://linkedin.com/in/karandesai2005"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://karan-desai.vercel.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white"/></a>
  <a href="https://medium.com/@karanishudesai2"><img src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white"/></a>
  <a href="https://twitter.com/White_Crow017"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white"/></a>
</p>

---

<p align="center">
  <sub>Currently building things that break other things — responsibly.</sub>
</p>
