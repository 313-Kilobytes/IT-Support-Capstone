# Week 1: Foundational IT Infrastructure Documentation
## Project: IT Support and Infrastructure Plan for Ubuntu Innovations (Pty) Ltd

---

## 📋 Task-1. Business Requirements Analysis

### 🏢 Company Overview
Ubuntu Innovations (Pty) Ltd is a fast-growing technology startup based in Cape Town, South Africa. As the company transitions into a new office space, it requires a robust, scalable, and secure IT infrastructure to support ongoing business operations.

### 👥 Department & User Breakdown

| Department | Staff | Primary Technical Roles & Core Needs |
| :--- | :---: | :--- |
| 👔 Executive Management | 3 | High-level operations, secure communications, mobile productivity tools. |
| 💰 Finance | 4 | Invoicing, payroll, cloud accounting, highly secure financial data handling. |
| 🤝 Human Resources | 3 | Staff records, recruitment systems, compliance, confidential storage. |
| 📈 Sales and Marketing | 7 | Client management (CRM), online marketing tools, high asset mobility. |
| 💻 Software Development | 8 | Code compilation, local testing environments, heavy compute & memory. |
| 📊 Total Staff | 25 | Fully unified under a single managed domain. |

### 🚀 Core Application Stack
- 💼 Office & Communication: Email, shared calendars, document collaboration, and video conferencing (Google Workspace or Microsoft 365).
- 🔒 Financial & HR Systems: Secure cloud accounting (Sage or Xero) and automated payroll/HR portals.
- 🛠️ Development Tools: Git-based version control (GitHub), lightweight IDEs (VS Code), and containerization (Docker).
- 🤝 Customer Management: Centralized CRM platform for sales pipeline tracking and client history.

---

### 🌐 Infrastructure & Operational Targets

---

## 🔌 Task-2. Hardware Inventory Plan

This hardware baseline satisfies your immediate operational footprint while maintaining space for seamless expansion.

| Asset & Icon | Qty | Suggested Specifications | Business Justification |
| :--- | :---: | :--- | :--- |
| 🖥️ Workstation PC | 20 | Intel i5, 16GB RAM, 512GB SSD<br>`Windows 11 Pro / Ubuntu` | Standard desktop layout for localized tasks across Finance, HR, Sales, and Devs. |
| 💻 Corporate Laptop | 5 | Intel i7, 16GB RAM, 512GB SSD<br>`Windows 11 Pro / macOS` | Distributed to Executives and roaming Team Leads for mobility and remote work. |
| 🛡️ Router / Firewall | 1 | Business-grade gateway with built-in VPN & threat scanning | Perimeter defense, secure remote employee access, and traffic routing. |
| 🔌 Managed Switch | 1 | 24-Port Gigabit Switch<br>`Power over Ethernet (PoE)` | Connects all desk drops, network printers, and APs into a high-speed local network. |
| 📶 Access Point (AP) | 2 | Dual-band Wi-Fi 6 (802.11ax)<br>`Enterprise Grade` | Strategic office placement for high-density, seamless wireless roaming. |
| 🖨️ Network Printer | 2 | Heavy-duty Laser MFP<br>`Monochrome/Color + Network Card` | Shared departmental printing, scanning, and digital archiving. |
| 🗄️ NAS Storage | 1 | 8TB Network Attached Storage<br>`RAID 1 or RAID 5 Configured` | Central file sharing coupled with a local repository for automated backups. |
| 🔋 Uninterruptible Power (UPS)| 2 | 1500VA Line-Interactive<br>`Surge Protection` | Critical for South African operations: Keeps the core network online during load-shedding. |

---

## 💾 Task-3. Software Inventory & Licensing Plan

### 🌐 Core Operating Software (Company-Wide)

#### 🖥️ Operating Systems
- Platforms: Windows 11 Pro / Ubuntu Linux
- Licensing: OEM licenses bundled with hardware purchases; open-source licensing for Linux environments.

#### 📧 Productivity & Collaboration Suites
- Platforms: Google Workspace OR Microsoft 365 Business Standard
- Licensing: 25 x Per-user monthly subscriptions
- Scope: Cloud email hosting, shared cloud storage (Drive/OneDrive), document collaboration, and video conferencing.

#### 🛡️ Endpoint Security & Defense
- Platforms: Bitdefender GravityZone OR Microsoft Defender for Business
- Licensing: 25 x Managed endpoint licenses
- Scope: Centralized cloud-managed agent deployment covering malware, anti-phishing, and ransomware isolation.

---

### 🛠️ Specialized Departmental Software
👔 Executive Management
└── 📝 Digital Signatures (e.g., DocuSign / Adobe Sign)
    └── 💳 3 User Licenses (Secure executive signing workflow)

💰 Finance Department
└── 📈 Cloud Accounting & Payroll (e.g., Xero / Sage Pastel)
    └── 💳 4 User Licenses (Enforced Multi-Factor Authentication)

🤝 Human Resources
└── 👥 HR Management System (HRMS Portal)
    └── 💳 3 User Licenses (Employee records, leave tracking, onboarding)

📈 Sales and Marketing
├── 🤝 CRM Platform (e.g., HubSpot / Zoho CRM) ──> 💳 7 User Licenses
└── 🎨 Creative Tools (e.g., Canva Pro) ─────────> 💳 2 User Licenses

💻 Software Development
├── 🐙 Version Control ──> 💳 8 GitHub Team Licenses
├── 💻 Coding IDEs ───────> 🟢 Open-Source VS Code (Zero Licensing Costs)
└── 🐳 Virtualization ──> 💳 8 Docker Desktop Team Licenses
---

> ⚠️ Security Baseline Note: Access control must be configured using the Principle of Least Privilege (PoLP). No employee should have write or read access to directories outside their designated functional department unless explicitly approved by Executive Management.
