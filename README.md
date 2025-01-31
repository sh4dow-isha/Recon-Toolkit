# Recon-Toolkit
# Web Application Penetration Testing Recon Tools

This repository provides an introduction to several essential tools for performing reconnaissance during a web application penetration test. Reconnaissance, or recon, is the first stage of penetration testing, where the tester gathers valuable information about the target web application to find vulnerabilities.

## Tools for Web Application Reconnaissance

Below are some commonly used recon tools to gather information about a target web application.

---

### Passive Recon

Passive reconnaissance involves collecting information without actively engaging with the target. These tools are useful for gathering details without alerting the target.

#### 1. **TheHarvester**
   - **Purpose**: Gathers email accounts, domain/subdomain names, and other information from public sources like search engines and PGP key servers.
   - **Tool**: [TheHarvester](https://github.com/laramies/theHarvester)
   - **Usage**: Use TheHarvester to collect information from public sources that could aid in later phases of the penetration test.
   - **Example**:
     ```bash
     theharvester -d example.com -b google
     ```

#### 2. **Maltego**
   - **Purpose**: Provides advanced data mining and link analysis capabilities to help gather information and map out the infrastructure and relationships of the target.
   - **Tool**: [Maltego](https://www.paterva.com/)
   - **Usage**: Maltego can be used to explore domains, emails, networks, and more by analyzing and connecting different pieces of information.

#### 3. **Spyse**
   - **Purpose**: A search engine for cybersecurity data, helping you perform passive reconnaissance by discovering information about IP addresses, domains, DNS, and more.
   - **Tool**: [Spyse](https://spyse.com/)
   - **Usage**: Spyse allows users to find details about domains, IPs, subdomains, and SSL/TLS certificates, all through a user-friendly interface.

#### 4. **Techackz**
   - **Purpose**: A web-based recon tool that helps gather data from various publicly available sources, useful for mapping out the target's infrastructure.
   - **Tool**: [Techackz](https://techackz.com/)
   - **Usage**: Techackz can provide insights into the technologies, domains, and subdomains associated with the target.

#### 5. **Shodan**
   - **Purpose**: Search engine for internet-connected devices. It can be used to identify devices, servers, and applications exposed on the internet.
   - **Tool**: [Shodan](https://www.shodan.io/)
   - **Usage**: Shodan is useful for identifying exposed services and vulnerabilities in devices such as routers, webcams, and servers.

---

### Active Recon

Active reconnaissance involves engaging directly with the target to gather information. These tools perform actions such as scanning ports or interacting with the web server.

#### 1. **Nmap**
   - **Purpose**: A powerful network scanning tool used for discovering hosts, open ports, services, and vulnerabilities in a network.
   - **Tool**: [Nmap](https://nmap.org/)
   - **Usage**: Nmap is commonly used for port scanning and service discovery.
   - **Example**:
     ```bash
     nmap -v -A example.com
     ```

#### 2. **Recon-ng**
   - **Purpose**: A full-featured reconnaissance framework that helps automate the collection of target information. It is modular and allows you to gather data from different sources.
   - **Tool**: [Recon-ng](https://github.com/lanmaster53/recon-ng)
   - **Usage**: Recon-ng provides various modules to gather target information, such as domain names, subdomains, and emails.
   - **Example**:
     ```bash
     recon-cli
     ```

#### 3. **Nikto**
   - **Purpose**: A web server scanner that checks for various vulnerabilities like outdated software, security misconfigurations, and common issues.
   - **Tool**: [Nikto](https://github.com/sullo/nikto)
   - **Usage**: Nikto is used to identify security vulnerabilities in web servers.
   - **Example**:
     ```bash
     nikto -h http://example.com
     ```

#### 4. **Dirb**
   - **Purpose**: A directory brute-forcing tool used to discover hidden directories and files on a web server.
   - **Tool**: [Dirb](https://github.com/v0re/dirb)
   - **Usage**: Dirb attempts to find hidden directories by trying different wordlists.
   - **Example**:
     ```bash
     dirb http://example.com
     ```

---

## Conclusion

Reconnaissance is a critical phase in web application penetration testing. By using the tools outlined above, security professionals can gather a wealth of information that helps in identifying attack vectors. Always ensure that you have permission from the target organization before performing any penetration testing or scanning.

---

## License

This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- [OWASP](https://owasp.org/) for providing great resources and tools for web application security.
- [Burp Suite](https://portswigger.net/burp) and [OWASP ZAP](https://www.zaproxy.org/) for offering powerful penetration testing tools.

### 7. **SSL/TLS Configuration Checks**
   - **Purpose**: Test SSL/TLS configuration for vulnerabilities.
   - **Tool**: [SSL Labs](https://www.ssllabs.com/ssltest/), [Testssl.sh](https://github.com/drwetter/testssl.sh)
   - **Usage**: These tools provide detailed analysis of SSL/TLS encryption and highlight potential weaknesses like outdated protocols or weak cipher suites.

## How to Use These Tools
