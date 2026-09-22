# Lumica1n Core Security Profile

![Profile](https://img.shields.io/badge/Profile-Extreme%20Security-red)
![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20iPadOS%20%7C%20macOS-blue)
![Organization](https://img.shields.io/badge/Organization-LifeStudio-green)

---

## 📖 Overview
The **Lumica1n Core Configuration Profile** is a system-level security enforcement profile created by **LifeStudio** for **iOS, iPadOS, and macOS**.  

It enforces **extreme security policies** including:
- Encrypted **DNS-over-HTTPS (DoH)** with ad/malware blocking  
- Strict **web content filtering**  
- Hardened **Safari restrictions**  
- Secure **Wi-Fi enforcement** against rogue hotspots  

---

## 🛡️ Features

- **[Encrypted DNS](ca://s?q=Explain_Encrypted_DNS)**  
  Routes all DNS traffic through secure DoH resolvers with malware/ad-blocking.

- **[Web Content Filtering](ca://s?q=Explain_Web_Content_Filtering)**  
  Blocks adult content, trackers, malicious redirects, and unsafe WebClips.

- **[Safari Hardening](ca://s?q=Explain_Safari_Hardening)**  
  Disables unsafe prompts, popups, and enforces fraud warnings.

- **[Wi-Fi Security](ca://s?q=Explain_WiFi_Security)**  
  Prevents auto-joining unencrypted hotspots and captive portal phishing.

---

## 🧩 Payloads

| **[Payload](ca://s?q=Explain_Payload_in_iOS_Profile)** | **Identifier** | **Purpose** |
|-----------------|-------------------------------|----------------|
| **DoH Shield** | `com.lifestudio.lumica1n.dns` | Encrypted DNS with ad/malware blocking |
| **Web Shield** | `com.lifestudio.lumica1n.webfilter` | Strict web content filtering |
| **System Hardening** | `com.lifestudio.lumica1n.restrictions` | Safari & system restrictions |
| **Wi-Fi Enforcement** | `com.lifestudio.lumica1n.wifi` | Secure Wi-Fi rules |

---

## 🔧 DNS Enforcement

- **Protocol:** HTTPS (DoH)  
- **Resolvers:**  
  - `1.1.1.2` (Cloudflare Security)  
  - `1.0.0.2`  
  - `9.9.9.9` (Quad9)  
  - `149.112.112.112`  

- **DoH Endpoint:**  
  `https://security.cloudflare-dns.com/dns-query`

- **On-Demand Rules:**  
  - Block `.local` and `.internal` domains  
  - Enforce secure connections on Wi-Fi and cellular  

---

## 🌐 Web Filtering

- **Filter Type:** Built-in  
- **AutoFilter:** Enabled  
- **Blacklisted Domains:**  
  - `doubleclick.net`  
  - `googlesyndication.com`  
  - `adservice.google.com`  
  - `popads.net`  
  - `popcash.net`  
  - `adf.ly`  

---

## 🖥️ Safari & System Restrictions

- AutoFill: **Disabled**  
- Fraud Warning: **Forced Enabled**  
- Popups: **Blocked**  
- Cookies: **Block cross-site / 3rd party**  
- Prevent unsafe WebClip injection  
- Enforce encrypted backups  

---

## 📶 Wi-Fi Security

- Blocks auto-joining **open/unsecured hotspots**  
- Disables captive portal bypass  
- No proxy enforced  

---

## ⚠️ Security Notes

- This profile is **system-wide** and applies to all users.  
- Removal is **allowed** but strongly discouraged.  
- Do **not** expose devices with this profile directly to the public internet without additional firewalling.  
- Designed for **enterprise-grade security enforcement**.  

---

## 📂 Repository Structure

/Lumica1n-Core-Profile
├── README.md
├── Lumica1n-Core.plist
└── LICENSE

  
---

## 📜 License

This project is maintained by **LifeStudio**.  
Distributed under the **MIT License**. See `LICENSE` for details.
