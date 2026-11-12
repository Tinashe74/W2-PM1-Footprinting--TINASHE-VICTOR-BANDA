# Week 2 - Project Module 1 (W2-PM1)
## Footprinting & Reconnaissance with Multiple Kali Tools

**Author:** Tinashe Victor Banda  
**Program:** Cybersecurity Internship (Networkwalks)  
**Batch:** B082  
**Date:** November 2026

---

## 📌 Project Overview
This repository contains the documentation and evidence for Week 2 - Project Module 1 (W2-PM1). The objective of this lab was to perform passive reconnaissance (footprinting) against the live domain `networkwalks.com` using six built-in Kali Linux tools. The goal was to gather public information, identify web technologies, and map the target's infrastructure without alerting the target.

## 🛠️ Tools Used & Key Findings
| Tool | Command Used | Key Finding |
| :--- | :--- | :--- |
| **WHOIS** | `whois networkwalks.com` | Registrar: GoDaddy, Name Servers: HostGator |
| **WhatWeb** | `whatweb networkwalks.com` | WordPress 7.1.4, Apache, IP: 192.232.216.135 |
| **Nslookup** | `nslookup networkwalks.com` | Resolved IP: 192.232.216.135 |
| **Curl** | `curl -I https://networkwalks.com` | Exposed HTTP headers and WP REST API (`/wp-json/`) |
| **Wafw00f** | `wafw00f networkwalks.com` | Detected ModSecurity (SpiderLabs) WAF |
| **DNSRecon** | `dnsrecon -d networkwalks.com` | Enumerated MX, TXT, SRV records & BIND version 9.16.23 |

## 📂 Directory Structure
The evidence for this module is organized as follows:

*   📁 **W2-PM1_Evidence/**
    *   📁 **Screenshots/** (Contains terminal screenshots for Tasks 1-6)
        *   `W2-PM1_Task1_WHOIS_Screenshot.png`
        *   `W2-PM1_Task2_WhatWeb_Screenshot.png`
        *   `W2-PM1_Task3_Nslookup_Screenshot.png`
        *   `W2-PM1_Task4_Curl_Screenshot.png`
        *   `W2-PM1_Task5_Wafw00f_Screenshot.png`
        *   `W2-PM1_Task6_DNSRecon_Screenshot.png`
    *   📁 **Text_Outputs/** (Contains the raw text output for Tasks 1-6)
        *   `W2-PM1_Task1_WHOIS_Output.txt`
        *   *(and so on for the other tasks...)*

## ⚠️ Liability Disclaimer
I have performed these activities only on the systems & devices where I had secured written permission or the devices/systems that I own myself. All these materials are for education and research purposes only. Do not use anything from here to break the law. The instructor, the authors, and Networkwalks are not responsible for what you do with this knowledge. Every action you take is your own responsibility. Misuse can lead to criminal charges, heavy fines, loss of your job, and a permanent record. In most countries, unauthorized access is a crime even when nothing is damaged.
