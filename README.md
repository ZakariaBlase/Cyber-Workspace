# 🛡️ Cyber-Workspace — OSINT & Pentest Tools Collection

[![Stars](https://img.shields.io/github/stars/ZakariaBlase/Cyber-Workspace?style=flat-square&color=yellow)](https://github.com/ZakariaBlase/Cyber-Workspace/stargazers)
[![Issues](https://img.shields.io/github/issues/ZakariaBlase/Cyber-Workspace?style=flat-square)](https://github.com/ZakariaBlase/Cyber-Workspace/issues)
[![License](https://img.shields.io/badge/use-authorized%20security%20testing%20only-red?style=flat-square)](#%EF%B8%8F-legal)
[![Tools](https://img.shields.io/badge/tools-2327-blue?style=flat-square)](#-stats-at-a-glance)

> A curated **OSINT (Open-Source Intelligence) and pentest tools collection** — 2,327 ready-to-use shortcuts covering recon, OSINT, web app security, network scanning, forensics, password cracking, and more. Organized by category, pricing tier, and use case, browsable with zero install.

**🔎 Looking for an OSINT tools list, an OSINT resources collection, or a pentest tool directory?** This repo indexes them all in one structured, deduplicated place.

⭐ **Star this repo** if it's useful — it helps other OSINT/pentest practitioners find it.
💡 **Found a missing tool, a broken link, or a better way to organize this?** Issues and PRs are welcome — see [Contributing](#-contributing).

---

## 📑 Table of Contents

- [Stats at a glance](#-stats-at-a-glance)
- [Categories](#-categories)
- [Inside 01-Recon-OSINT](#inside-01-recon-osint)
- [Inside 02-Web-AppSec](#inside-02-web-appsec)
- [Convention](#%EF%B8%8F-convention)
- [Sources](#-sources)
- [Contributing](#-contributing)
- [Legal](#%EF%B8%8F-legal)
- [Usage](#-usage)
- [About me](#-about-me)

---

## 📊 Stats at a glance

| Metric | Count |
|---|---:|
| **Total shortcuts** | **2327** |
| Top-level categories | 13 |
| 🟢 Free tools | 1997 |
| 🟡 Freemium tools | 215 |
| 🔴 Paid tools | 61 |

## 📁 Categories

| Folder | Shortcuts | Focus |
|---|---:|---|
| `01-Recon-OSINT/` | **953** | OSINT recon — identity pivots (username/email/GEOINT/reverse-image/social/messengers), Dark-Web, General-OSINT (data intelligence, dork tools, multi-tool platforms, public data), Telegram-mined bots & regional services, OSINTCabal import |
| `02-Web-AppSec/` | **237** | Web pentest arsenal **by attack phase**: crawl → subdomains → content discovery → param discovery → tech/WAF fingerprint → vuln scanners → XSS → SQLi/NoSQLi → SSRF/LFI/redirect/CRLF → JS secrets → dorking → frameworks → bug bounty platforms, plus Crawling-Scraping & DomainInt |
| `03-Network-Scan/` | **143** | Port/service scanning, AD enumeration, Post-Exploitation, RFID, WiFi, Bluetooth, CCTV, DNS/IP, SIGINT |
| `04-Enumeration/` | 15 | Directory/subdomain/user brute-forcing (ffuf, gobuster, feroxbuster, kerbrute) |
| `05-Passwords-Hashes/` | 53 | Cracking & hash ID, Password-Managers, Breach-Data (credential leaks, password dumps) |
| `06-Wordlists/` | 11 | SecLists, PayloadsAllTheThings, fuzzdb |
| `07-Forensics-Malware/` | **287** | Forensics & malware analysis, Cryptography, Steganography, Steganalysis, Hex-Editors, Execution-Logging-Tracing, Deobfuscators, Decompilers, Disassemblers/Debuggers, Binary-Exploitation |
| `08-Tools-GUI/` | 32 | Flagship GUI suites, Operating-Systems, Hardware-Tools |
| `09-AI-Tools/` | 14 | AI-Programming, AI-Cybersecurity |
| `10-Privacy-Anonymity/` | 29 | VPNs, Privacy & Anonymity, Delete-Your-Trace |
| `11-Cryptocurrency/` | 13 | Blockchain & crypto-investigation tools |
| `12-Specialized-Tools/` | 9 | SIEM, Playbooks |
| `Web-Shortcuts/` | **531** | OSINT-Catalog (17 categories), Learning (12 sub-categories: courses, certifications, CTFs, practice labs, books, YouTube...), Media, Social, Search-Engines, Utility-Misc, and the original curated hub sites |

### Inside `01-Recon-OSINT/`
- **`Identity-OSINT/`** — shortcuts split by **pivot type**: username, email, phone, GEOINT, reverse image, breaches & leaks, face recognition, EXIF/image forensics, and per-platform folders (Instagram, LinkedIn, TikTok, OnlyFans, Twitch, Tinder, Reddit, Twitter/X, Facebook, Pinterest, Tumblr, Steam, GitHub, VKontakte) + per-messenger folders (Telegram, Discord, WhatsApp, Skype, Slack, Kik)
- **`General-OSINT/`** — multi-tool platforms, dork tools, data intelligence aggregators, bookmark collections, dark web search engines & onion directories
- **`OSINTCabal/`** — community-curated tool drop, deduplicated against the rest of the collection
- **`Telegram-Posts-Tools/`** — bots, regional services, and practice labs mined directly from OSINT Telegram channel posts (not just repo READMEs)

### Inside `02-Web-AppSec/`
A full kill-chain, phase by phase. Typical pipeline:
```
subfinder | httpx | katana | gf xss | dalfox     # recon -> live hosts -> crawl -> XSS sink discovery
nuclei -l alive.txt -t cves/                      # template-based vuln scan
sqlmap -u "<url>"                                 # SQLi exploitation
ffuf -u https://target/FUZZ -w wordlist.txt       # content discovery
```

## 🗂️ Convention

Every shortcut follows a strict naming/sorting scheme:

- **`Online/` vs `GitHub/`** — most categories split browser-based services from installable tools
- **Tier prefix** for instant sort in any file explorer:
  - `1-Gratuit` → free
  - `2-Freemium` → free tier + paid upgrade
  - `3-Payant` → paid only

## 📚 Sources

Curated and deduplicated from multiple OSINT/pentest tool collections, including [bst04/CyberSources](https://github.com/bst04/CyberSources), [osintcabal.org](https://osintcabal.org), [osintrack.com](https://osintrack.com), public GitHub awesome-lists, and OSINT Telegram channel exports (Cybdetective;OSINT Ressources) — all redistributed into this workspace's own category taxonomy and re-triaged by pricing tier.

## 🙌 Contributing

Contributions are welcome and easy:
1. Open an **issue** for a broken link, a duplicate, or a missing tool.
2. Or open a **PR** directly: drop a new `.url` shortcut (`[InternetShortcut]` / `URL=...`) into the matching category and tier folder.
3. Keep the naming convention (`Online/` vs `GitHub/`, tier prefix) so the collection stays consistent.

## ⚖️ Legal

This collection indexes **publicly available tools and services** for use in **authorized** contexts only: signed penetration tests, CTF competitions, in-scope bug bounty programs, and personal lab environments. The repository does not host any exploit code, credentials, or scraped personal data — only links.

## 🤝 Usage

Clone, open any folder, and click a `.url` file to jump straight to the tool. Want to extend it? Just drop a new `.url` shortcut (`[InternetShortcut]` / `URL=...`) into the matching category and tier.

## 👤 About me

17 y.o. student from France | Enthusiast in Cybersecurity, OSINT, Pentesting, and IoT | Exploring ethical hacking and technology innovation
