### 1.1 Company Overview & Structure
# Week 1: Foundational IT Infrastructure Documentation
## Project: IT Support and Infrastructure Plan for Ubuntu Innovations (Pty) Ltd

---

## Task-1. Business Requirements Analysis

### Company Overview
Ubuntu Innovations (Pty) Ltd is a fast-growing technology startup based in Cape Town, South Africa. The company is moving to a new office space and needs a complete, secure, and modern IT infrastructure setup to support its daily business functions.

### Department and User Breakdown
The office hosts a total of **25 employees** distributed across five main departments. Each department has distinct functional needs that the IT infrastructure must accommodate:

| Department | Number of Employees | Primary Technical Roles & Needs |
| :--- | :---: | :--- |
| **Executive Management** | 3 | High-level operations, secure communications, mobility tools. |
| **Finance** | 4 | Invoicing, payroll, accounting software, highly secure data handling. |
| **Human Resources** | 3 | Staff records, recruitment systems, compliance, confidential data storage. |
| **Sales and Marketing** | 7 | Client management (CRM), online marketing tools, high mobility. |
| **Software Development** | 8 | Writing code, local environments, testing, heavy compute requirements. |
| **Total Staff** | **25** | |

### Core Business Applications
To keep the business running smoothly, the infrastructure must support the following software applications:
* **Office Productivity & Communication:** Email, shared calendars, spreadsheets, documents, and video conferencing tools (such as Google Workspace or Microsoft 365).
* **Financial & HR Systems:** Secure cloud-based accounting software (such as Sage or Xero) and payroll/HR portals.
* **Development Tools:** Git-based version control (GitHub), integrated development environments (IDEs like VS Code), and container tools (Docker).
* **Customer Relationship Management (CRM):** Sales tracking tools to manage client interactions.

### Infrastructure & Connectivity Requirements
* **Network Access:** Reliable, high-speed wired Ethernet connections for fixed office desks and high-speed Wi-Fi 6 coverage for laptops, mobile devices, and guests.
* **Central Storage:** Shared central file storage that allows team collaboration while keeping sensitive department folders private.
* **Peripherals:** Shared high-speed network printers accessible to all authorized staff.

### Security & Operational Requirements
* **Identity Management:** Individual user accounts for every employee to log into devices and network resources securely.
* **Access Control:** A strict permission setup based on departments so users can only open folders and files necessary for their specific job roles.
* **Endpoint Security:** Active antivirus and endpoint protection on every machine to prevent malware infections.
* **Data Protection:** Automatic local and cloud backup routines to protect against accidental deletion, hardware failure, or power disruptions.

---

## Task-2. Hardware Inventory Plan

The following hardware is selected to meet the exact operational requirements of Ubuntu Innovations (Pty) Ltd. Equipment is scaled to handle everyday startup tasks efficiently without unnecessary expenses.

| Asset Type | Quantity | Suggested Technical Specifications | Business Justification |
| :--- | :---: | :--- | :--- |
| **Desktop Computers** | 20 | Intel Core i5, 16GB RAM, 512GB SSD, Windows 11 Pro / Ubuntu Linux | Standard workstations for the Finance, HR, Sales, and Development teams to run everyday business applications and development tasks smoothly. |
| **Laptops** | 5 | Intel Core i7, 16GB RAM, 512GB SSD, Windows 11 Pro / macOS | Distributed to the 3 Executive Management members and 2 roaming team leaders to ensure work mobility and remote access capabilities. |
| **Router / Firewall** | 1 | Business-grade firewall router with built-in VPN and security scanning | Acts as the gateway to the internet, providing secure routing, a strong firewall to keep threats out, and secure remote VPN connections. |
| **Network Switch** | 1 | 24-Port Gigabit Managed Switch (with PoE support) | Connects all wired office desks, desktop computers, network printers, and access points together into a fast local network. |
| **Wireless Access Points** | 2 | Dual-band Wi-Fi 6 (802.11ax) business-grade access points | Placed strategically across the office to provide stable, fast, and seamless wireless internet coverage for all laptops and mobile devices. |
| **Network Printers** | 2 | Heavy-duty monochrome/color laser printers with network cards | Shared office printers connected to the local network so all departments can print and scan reports easily. |
| **NAS Device (Storage)** | 1 | 8TB Network Attached Storage (NAS) with RAID 1/5 capability | Acts as a central file server for local shared folders and serves as the destination for automated local backups. |
| **Uninterruptible Power Supply (UPS)** | 2 | 1500VA Line-Interactive UPS systems with surge protection | Protects critical network gear (router, switch, NAS) from power surges and keeps them running during brief power outages or load shedding. |

---

## Task-3. Software Inventory & Licensing Plan

This plan outlines the software footprint required across the organization, categorized by standard office use and specialized department needs.

### Standard Operating Software (All Departments)
* **Operating Systems:** Windows 11 Pro / Ubuntu Linux (Pre-installed on desktops/laptops). OEM licenses are included with hardware purchases; open-source setup is used for Linux machines.
* **Productivity & Collaboration Suites:** Google Workspace or Microsoft 365 Business Standard. Handles company email hosting, cloud file storage (Drive/OneDrive), text documents, spreadsheets, and team communication via chat or video calls. Requires a per-user monthly subscription (25 licenses needed).
* **Endpoint Security:** Business Antivirus & EDR Suite (such as Bitdefender GravityZone or Microsoft Defender for Business). Provides real-time protection against malware, ransomware, phishing links, and viruses. Requires a centralized cloud-managed subscription (25 licenses needed).

### Specialized Departmental Software

#### 1. Executive Management
* **Software Needed:** Digital Signature software (such as Adobe Acrobat Sign or DocuSign) for signing legal and business documents securely.
* **Licensing:** 3 user licenses.

#### 2. Finance
* **Software Needed:** Professional Accounting & Payroll Cloud Platform (such as Xero or Sage Pastel).
* **Licensing:** 4 user licenses with strict multi-factor authentication (MFA) enabled.

#### 3. Human Resources
* **Software Needed:** HR Management System (HRMS) portal for tracking leave, recruitment, and onboarding documentation.
* **Licensing:** 3 user licenses.

#### 4. Sales and Marketing
* **Software Needed:** Customer Relationship Management (CRM) platform (such as HubSpot CRM or Zoho CRM) along with basic design software (such as Canva Pro).
* **Licensing:** 7 CRM user licenses; 2 design licenses.

#### 5. Software Development
* **Software Needed:** Version Control via GitHub Team Plan accounts, IDEs like Visual Studio Code, and local virtualization tools like Docker Desktop or VirtualBox for running test environments.
* **Licensing:** 8 GitHub Team licenses; IDEs utilize open-source options; Docker Desktop team licenses as applicable.