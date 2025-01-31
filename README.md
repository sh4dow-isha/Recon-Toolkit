# Recon-Toolkit
# Web Application Penetration Testing Recon Tools

This repository provides an introduction to several essential tools for performing reconnaissance during a web application penetration test. Reconnaissance, or recon, is the first stage of penetration testing, where the tester gathers valuable information about the target web application to find vulnerabilities.

## Tools for Web Application Reconnaissance

Below are some commonly used recon tools to gather information about a target web application.

### 1. **Whois Lookup**
   - **Purpose**: Retrieve domain registration details (e.g., owner, registrar, and IP).
   - **Tool**: [Whois](https://whois.domaintools.com/), [Whois CLI](https://github.com/whois-api/whois)
   - **Usage**: Use Whois to gather information about the domain, such as the organization, contact information, and DNS records.

### 2. **Subdomain Enumeration**
   - **Purpose**: Identify subdomains of the target domain.
   - **Tool**: [Sublist3r](https://github.com/aboul3la/Sublist3r), [Amass](https://github.com/OWASP/Amass)
   - **Usage**: These tools help you discover hidden subdomains that could lead to attack vectors like exposed services or misconfigured applications.

### 3. **DNS Interrogation**
   - **Purpose**: Collect DNS records to gather information about the target's infrastructure.
   - **Tool**: [DNSdumpster](https://dnsdumpster.com/), [Fierce](https://github.com/mschwager/fierce)
   - **Usage**: Use DNS interrogation tools to enumerate DNS records, identify services, and gather insights into the target's DNS configuration.

### 4. **Directory and File Brute Forcing**
   - **Purpose**: Discover hidden directories and files on the web server.
   - **Tool**: [Dirb](https://github.com/dirb/dirb), [Gobuster](https://github.com/OJ/gobuster)
   - **Usage**: These tools help you discover hidden directories or files that may not be publicly listed, such as backup files, old admin interfaces, or sensitive data.

### 5. **Web Application Scanning**
   - **Purpose**: Identify vulnerabilities in the web application.
   - **Tool**: [Burp Suite](https://portswigger.net/burp), [OWASP ZAP](https://www.zaproxy.org/)
   - **Usage**: These tools allow you to scan the web application for common security issues, such as SQL injection, cross-site scripting (XSS), and insecure configurations.

### 6. **Fingerprinting Technologies**
   - **Purpose**: Identify technologies used in the web application (e.g., web servers, frameworks, and CMS).
   - **Tool**: [Wappalyzer](https://www.wappalyzer.com/), [WhatWeb](https://github.com/urbanadventurer/WhatWeb)
   - **Usage**: These tools detect the software stack (e.g., CMS, programming languages, web server types) used by the target web application.

### 7. **SSL/TLS Configuration Checks**
   - **Purpose**: Test SSL/TLS configuration for vulnerabilities.
   - **Tool**: [SSL Labs](https://www.ssllabs.com/ssltest/), [Testssl.sh](https://github.com/drwetter/testssl.sh)
   - **Usage**: These tools provide detailed analysis of SSL/TLS encryption and highlight potential weaknesses like outdated protocols or weak cipher suites.

## How to Use These Tools
