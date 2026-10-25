# Cybersecurity-CTF-Labs-Collection-XXE-SSRF-Internal-Network-Pivoting
A curated index of hands-on CTF labs covering XML External Entity (XXE), Server-Side Request Forgery (SSRF), DNS rebinding, protocol smuggling, and cloud metadata pivoting from Learn SecByte.
# XXE & SSRF Exploitation & Defense CTF Labs Collection

A structured, searchable index of hands-on cybersecurity labs focusing on XML External Entity (XXE) injection, Server-Side Request Forgery (SSRF), Out-of-Band (OOB) data exfiltration, protocol smuggling, DNS rebinding, and cloud metadata pivoting hosted on Learn SecByte.

This collection is designed for web application security testers, penetration testers, CTF players, security analysts, and developers learning how to identify, exploit, and remediate parser vulnerabilities and internal network exposure risks.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
  - [XML External Entity (XXE) Attacks](#xml-external-entity-xxe-attacks)
  - [Server-Side Request Forgery (SSRF) & Pivoting](#server-side-request-forgery-ssrf--pivoting)
  - [Advanced Network & Protocol Bypass Techniques](#advanced-network--protocol-bypass-techniques)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Parsing untrusted data formats and processing remote user-supplied URLs present significant risks to modern web infrastructure. Vulnerabilities like XML External Entity (XXE) injection and Server-Side Request Forgery (SSRF) allow attackers to read local server files, interact with internal microservices, access cloud metadata endpoints, and achieve Remote Code Execution (RCE).

This repository organizes hands-on cybersecurity labs from Learn SecByte into logical learning paths covering advanced web security and network pivoting vectors.

---

## Lab Collection & Index

| Lab Title | Primary Category | Domain Focus | Access Link |
| :--- | :--- | :--- | :--- |
| **SVG XXE** | XXE | Embedded XML Payloads | [Access Lab](https://learn.secbyte.org/ctf/svg-xxe-embedded-xml-payloads) |
| **SOAP XXE** | XXE | Web Services / SOAP | [Access Lab](https://learn.secbyte.org/ctf/soap-xxe-from-xml-basics-to-blind-exfiltration) |
| **Out-of-Band XXE** | XXE | OOB Exploitation & Detection | [Access Lab](https://learn.secbyte.org/ctf/out-of-band-xxe-blind-xml-exploitation-and-detection) |
| **Blind XXE Fundamentals** | XXE | Out-of-Band Data Exfiltration | [Access Lab](https://learn.secbyte.org/ctf/blind-xxe-from-xml-fundamentals-to-out-of-band-data-exfiltra) |
| **XML External Entity (XXE)** | XXE | Core XML Vulnerabilities | [Access Lab](https://learn.secbyte.org/ctf/xml-external-entity-xxe) |
| **Webhook SSRF** | SSRF | Callback Abuse & Pivoting | [Access Lab](https://learn.secbyte.org/ctf/webhook-ssrf-from-callback-abuse-to-internal-pivoting) |
| **Protocol Smuggling** | Request Smuggling | Parser Disagreements | [Access Lab](https://learn.secbyte.org/ctf/protocol-smuggling-when-parsers-disagree) |
| **DNS Rebinding** | Network Bypass | Same-Origin Policy Bypass | [Access Lab](https://learn.secbyte.org/ctf/dns-rebinding-from-same-origin-to-internal-pivoting) |
| **SSRF Filter Bypass** | SSRF | Evasion & Blacklist Bypass | [Access Lab](https://learn.secbyte.org/ctf/ssrf-filter-bypass-lab) |
| **Internal Port Scanning** | Network Recon | Internal Network Discovery | [Access Lab](https://learn.secbyte.org/ctf/internal-port-scanning-fundamentals) |
| **SSRF to RCE** | SSRF | Internal Service Pivoting | [Access Lab](https://learn.secbyte.org/ctf/ssrf-to-rce-internal-service-pivoting-lab) |
| **Cloud Metadata SSRF** | SSRF / Cloud | Instance Metadata Access | [Access Lab](https://learn.secbyte.org/ctf/cloud-metadata-ssrf-pivoting-through-instance-metadata) |

---

## Categories

### XML External Entity (XXE) Attacks
Hands-on CTF labs exploring XML parser misconfigurations, file retrieval, and out-of-band data exfiltration across various media types:

* **XML External Entity (XXE) Basics:** Core mechanics of external entity processing and local file disclosure.
  * Lab Link: https://learn.secbyte.org/ctf/xml-external-entity-xxe
* **SVG XXE:** Embedding malicious XML payloads inside Scalable Vector Graphics (SVG) image uploads.
  * Lab Link: https://learn.secbyte.org/ctf/svg-xxe-embedded-xml-payloads
* **SOAP XXE:** Exploiting XML entity processing within SOAP-based web services.
  * Lab Link: https://learn.secbyte.org/ctf/soap-xxe-from-xml-basics-to-blind-exfiltration
* **Blind XXE & Out-of-Band Exfiltration:** Utilizing parameter entities and external DTDs to exfiltrate data over HTTP/FTP.
  * Lab Link: https://learn.secbyte.org/ctf/blind-xxe-from-xml-fundamentals-to-out-of-band-data-exfiltra
* **Out-of-Band XXE Detection:** Analyzing server logs and out-of-band interaction techniques for detection and defense.
  * Lab Link: https://learn.secbyte.org/ctf/out-of-band-xxe-blind-xml-exploitation-and-detection

### Server-Side Request Forgery (SSRF) & Pivoting
Practical security labs demonstrating how server-side HTTP clients can be abused to probe networks, access metadata, and achieve remote code execution:

* **Internal Port Scanning:** Using SSRF vectors to map non-public internal networks and discovering hidden services.
  * Lab Link: https://learn.secbyte.org/ctf/internal-port-scanning-fundamentals
* **Webhook SSRF:** Abusing webhook registration features to pivot into internal networks via callback abuse.
  * Lab Link: https://learn.secbyte.org/ctf/webhook-ssrf-from-callback-abuse-to-internal-pivoting
* **SSRF Filter Bypass:** Bypassing URL blacklists, IP filters, and DNS validation checks using encoding and alternative representations.
  * Lab Link: https://learn.secbyte.org/ctf/ssrf-filter-bypass-lab
* **Cloud Metadata SSRF:** Interrogating cloud instance metadata services (IMDS) to harvest IAM role credentials.
  * Lab Link: https://learn.secbyte.org/ctf/cloud-metadata-ssrf-pivoting-through-instance-metadata
* **SSRF to RCE:** Escalating SSRF vulnerabilities to Remote Code Execution by interacting with unauthenticated internal administrative interfaces.
  * Lab Link: https://learn.secbyte.org/ctf/ssrf-to-rce-internal-service-pivoting-lab

### Advanced Network & Protocol Bypass Techniques
Labs focused on network security boundaries, parser discrepancies, and origin policy bypasses:

* **DNS Rebinding:** Bypassing Same-Origin Policy (SOP) and IP filters using dynamic DNS domain switching.
  * Lab Link: https://learn.secbyte.org/ctf/dns-rebinding-from-same-origin-to-internal-pivoting
* **Protocol Smuggling:** Exploiting parser logic disagreements between front-end proxies and back-end services.
  * Lab Link: https://learn.secbyte.org/ctf/protocol-smuggling-when-parsers-disagree

---

## Learning Path

Follow this structured roadmap to build deep expertise in web parser and request forgery vulnerabilities:

1. **Core Parser Fundamentals**
   - Practice classic XXE file reading and simple SSRF request triggers.
2. **Out-of-Band Exfiltration & Media Payloads**
   - Execute blind XXE using external DTDs and test file formats like SVG image uploads.
   - Master SOAP service XXE exploitation.
3. **SSRF Filter Evasion & Network Discovery**
   - Learn internal port scanning and bypass URL/IP filtering logic.
   - Practice DNS rebinding and protocol smuggling techniques.
4. **Cloud Exposure & Full System Compromise**
   - Query cloud metadata endpoints via SSRF to steal cloud credentials.
   - Pivot from SSRF to achieve full Remote Code Execution (RCE) on internal services.

---

## How to Use the Labs

1. Select a practice environment from the index table or category sections above.
2. Access the target lab directly on Learn SecByte.
3. Utilize tools such as Burp Suite, netcat, or custom out-of-band listener servers (e.g., interactsh) to craft payloads and capture callbacks.
4. Review defense guidelines to learn how disabling DTD processing, enforcing strict URL allowlists, and hardening metadata access protect modern applications.

---

## Disclaimer

This repository is strictly intended for educational research, authorized security testing, and defensive engineering training. All concepts, techniques, and lab environments are provided to help cybersecurity practitioners identify vulnerabilities and defend systems. Unsanctioned testing or attacks against systems without prior written authorization are strictly illegal.
