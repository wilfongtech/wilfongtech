# Hi, I'm Alex 👋

### Desktop Engineer | Aspiring Systems Engineer
I am a Desktop Administrator in my day job, and this is my home lab. My home lab serves as an enterprise-grade proving ground where I design, automate, and secure physical networking, clustered virtualization, modern directory federation, and containerized services.

---

## 🏗️ What I've Built (Homelab & Production Architectures)

### **Enterprise Identity & Modern Management**
* **Hybrid Identity Architecture:** Integrated **Microsoft 365 Business Premium** and **Microsoft Entra ID** with **Okta** as an Identity Provider (IdP), bridging cloud single sign-on (SSO) with an on-premises **Windows Server 2022 Active Directory** domain controller.
* **Modern Endpoint Management:** Built zero-touch **Windows Autopilot** ingestion pipelines leveraging Microsoft Graph API, Entra dynamic device groups, and **Microsoft Intune** deployment profiles.
* **Granular Role-Based Access Control:** Configured Entra ID OpenID Connect (OIDC) authentication realms for Proxmox cluster access with strict administrative group bindings.

### **Clustered Virtualization & Infrastructure as Code**
* **3-Node Proxmox VE Cluster (`wt-cluster`):** Engineered a high-availability hypervisor cluster running across dedicated compute nodes with LVM-Thin storage pools and VirtIO optimizations.
* **Cloud-Init Golden Image Pipeline:** Built automated Bash provisioning pipelines that fetch, verify (SHA512), and convert upstream Debian 13 (Trixie) cloud images into hardened, headless, passwordless templates deployed in seconds.
* **Container Orchestration:** Deployed Docker Compose stacks and Portainer environments across Debian hosts, running production services (Audiobookshelf, Prometheus, Grafana) with non-root security contexts and dropped Linux capabilities.

### **Core Networking & Perimeter Security**
* **L2/L3 Segmentation:** Configured an enterprise **Juniper EX2200-C** switch via JunOS CLI, establishing 802.1Q trunking, dedicated VLANs (`Management`, `Infra`, `Container-VMs`, `Clients`), and routed virtual interfaces (RVI).
* **Perimeter Defense & Routing:** Deployed a **UniFi Cloud Gateway Ultra** perimeter router with encrypted DNS upstream resolvers (`Cloudflare/Quad9`) and automated dynamic DNS with WireGuard remote access.

### **Observability & Incident Telemetry**
* **Centralized Monitoring Stack:** Deployed **Zabbix 7.0 LTS** with PostgreSQL and NGINX inside a Debian LXC container on an isolated VLAN, collecting metrics via Zabbix Agent 2 across hypervisor nodes.
* **Custom Alerting Pipeline:** Engineered an automated incident routing engine utilizing an Entra App Registration and Microsoft Graph API to dispatch system alerts directly via Microsoft 365.
* **Dashboards & Metrics:** Deployed an OWASP-hardened **Grafana** instance connected to the Zabbix API using dedicated, least-privilege service tokens.

---

## 💻 Tech Stack & Tools

**Identity & Cloud**  
![Microsoft Entra ID](https://img.shields.io/badge/Entra_ID-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Microsoft Intune](https://img.shields.io/badge/Microsoft_Intune-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Okta](https://img.shields.io/badge/Okta-007DC1?style=for-the-badge&logo=okta&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active_Directory-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![Microsoft 365](https://img.shields.io/badge/Microsoft_365-D83B01?style=for-the-badge&logo=microsoftoffice&logoColor=white)

**Systems & Virtualization**  
![Proxmox VE](https://img.shields.io/badge/Proxmox_VE-E57000?style=for-the-badge&logo=proxmox&logoColor=white)
![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)
![Ubuntu Server](https://img.shields.io/badge/Ubuntu-E9430F?style=for-the-badge&logo=ubuntu&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows_Server-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-000000?style=for-the-badge&logo=apple&logoColor=white)

**Networking & Observability**  
![Juniper JunOS](https://img.shields.io/badge/Juniper_Networks-000000?style=for-the-badge&logo=junipernetworks&logoColor=white)
![UniFi](https://img.shields.io/badge/UniFi-0559C9?style=for-the-badge&logo=ubiquiti&logoColor=white)
![Zabbix](https://img.shields.io/badge/Zabbix_7.0_LTS-D40000?style=for-the-badge&logo=zabbix&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![WireGuard](https://img.shields.io/badge/WireGuard-88171A?style=for-the-badge&logo=wireguard&logoColor=white)

**Automation & Development**  
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-F05138?style=for-the-badge&logo=swift&logoColor=white)

---

## 🗺️ Engineering Roadmap & Immediate Focus

* 📜 **Configuration Management (Ansible):** Moving from single-host provisioning scripts to agentless configuration playbooks for OS-level baseline hardening, automated SSH key rotation, and fleet-wide Zabbix Agent deployments.
* 📦 **CI/CD & GitOps Workflows:** Deploying private GitHub Actions self-hosted runners within isolated homelab VLANs to automate Docker stack deployments and infrastructure linting pipelines on commit.
* 🎓 **Certifications & Education:**
  * **WGU:** Master of Science in Information Technology (*In Progress*)
  * **Microsoft Certified:** MD-102 (Endpoint Administrator Associate)
  * **Linux Professional Institute:** Linux Essentials
