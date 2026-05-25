# 🖥️ Week 2 – OS Administration & Access Control

> **Tech Career Accelerator** · Week 2 Project  
> Designing and documenting an operating system administration and access control structure for a simulated enterprise environment.

---

## 📋 Overview

This project covers the design and documentation of core system administration components, including user access control, shared folder architecture, command-line operations, software deployment, and network IP addressing. All deliverables are modelled around a multi-department organisation with clearly defined security boundaries.

---

## 🎯 Objectives

- Design a user and permissions matrix aligned to departmental security groups
- Architect a shared folder structure that enforces least-privilege access
- Document essential Linux command-line administration procedures
- Produce a structured software deployment plan covering licensing and update cycles
- Define a segmented IP addressing scheme for all device categories

---

## 📁 Project Structure

```
week-2/
├── docs/
│   ├── Task1_User_Permissions_Matrix.pdf
│   ├── Task2_Shared_Folder_Design.pdf
│   ├── Task3_CommandLine_Admin_Guide.pdf
│   ├── Task4_Software_Deployment_Plan.pdf
│   └── Task5_IP_Addressing_Plan.pdf
└── README.md
```

---

## 📌 Tasks

### Task 1 — User and Permissions Matrix

Defines the mapping between departments, security groups, folder access, and permission levels across the organisation.

| Department | Security Group | Folder Access | Permission Level |
|---|---|---|---|
| Management | `mgmt_grp` | All folders | Full Control |
| Finance | `finance_grp` | `/Company/Finance` | Read / Write |
| HR | `hr_grp` | `/Company/HR` | Read / Write |
| Sales | `sales_grp` | `/Company/Sales` | Read / Write |
| Development | `dev_grp` | `/Company/Development` | Read / Write |
| All Staff | `all_staff` | `/Company/Public` | Read Only |

> All access follows the **principle of least privilege** — each group receives only the permissions required to perform its designated function.

---

### Task 2 — Shared Folder Design

Documents the recommended folder hierarchy for the company file server.

```
/Company/
├── Public/          ← All staff (Read Only)
├── Finance/         ← finance_grp (Read/Write)
├── HR/              ← hr_grp (Read/Write)
├── Sales/           ← sales_grp (Read/Write)
├── Development/     ← dev_grp (Read/Write)
└── Management/      ← mgmt_grp (Full Control)
```

Each departmental folder includes standardised sub-folders:

```
<Department>/
├── Archive/
├── Templates/
├── Reports/
└── Working/
```

---

### Task 3 — Command-Line Administration Guide

A practical reference for Linux system administration commands used in the environment.

| Command | Purpose |
|---|---|
| `pwd` | Print the current working directory |
| `ls` | List directory contents with metadata |
| `cd` | Navigate between directories |
| `mkdir` | Create directories, including nested paths with `-p` |
| `touch` | Create empty files or update timestamps |
| `chmod` | Modify file and directory permissions |
| `chown` | Change file ownership and group assignment |
| `ps` | View a snapshot of running processes |
| `top` | Monitor real-time system resource utilisation |
| `apt install` | Install packages from APT repositories |

**Example — Setting permissions on a departmental folder:**

```bash
# Create the Finance directory and assign ownership
sudo mkdir -p /Company/Finance
sudo chown -R root:finance_grp /Company/Finance
sudo chmod 750 /Company/Finance
```

**Example — Installing a package:**

```bash
sudo apt update && sudo apt install openssh-server
```

---

### Task 4 — Software Deployment Plan

#### Standard Baseline (All Devices)

| Package | Purpose |
|---|---|
| Ubuntu LTS | Operating system |
| LibreOffice | Productivity suite |
| Mozilla Firefox (ESR) | Approved web browser |
| ClamAV | Endpoint antivirus |
| OpenSSH Client | Secure shell access |
| Timeshift | System snapshots and recovery |

#### Department-Specific Applications

| Department | Application | Purpose |
|---|---|---|
| Finance | GnuCash / Sage | Accounting and financial management |
| HR | OrangeHRM | Employee records and leave management |
| Sales | Odoo CRM | Customer relationship management |
| Development | VS Code, Docker, Git | Code editing and version control |
| Management | Metabase | Business intelligence and reporting |

#### Update Schedule

| Cycle | Frequency | Scope |
|---|---|---|
| Security patches | Weekly (Sunday 02:00) | All servers and workstations |
| Feature updates | First Tuesday of month | Staged rollout — Dev first |
| Emergency patches | As required (< 48 hrs) | Zero-day / actively exploited CVEs |

---

### Task 5 — IP Addressing Plan

All subnets are drawn from RFC 1918 private address space.

| Device Category | Subnet | Usable Range | DHCP |
|---|---|---|---|
| Servers | `192.168.10.0/24` | .1 – .254 | No (static) |
| User Devices | `192.168.20.0/24` | .50 – .200 (pool) | Yes |
| Printers | `192.168.30.0/24` | .1 – .254 | No (static) |
| Wi-Fi / BYOD | `192.168.40.0/24` | .50 – .200 (pool) | Yes |
| Management VLAN | `192.168.100.0/24` | .1 – .254 | No (static) |

**DNS Configuration:**
- Primary DNS: `192.168.10.10`
- Secondary DNS: `192.168.10.11`
- External forwarding: `1.1.1.1` / `8.8.8.8`

> The Wi-Fi / BYOD VLAN (`192.168.40.0/24`) is isolated with no direct route to the Server or Management VLANs.

---

## 📦 Deliverables

- [x] User and Permissions Matrix
- [x] Shared Folder Structure
- [x] Command-Line Administration Guide
- [x] Software Deployment Plan
- [x] IP Addressing Plan

---

## 🛠️ Technologies & Tools Referenced

- **Ubuntu LTS** — Primary operating system for all servers and workstations
- **Linux (Bash)** — Command-line environment for system administration
- **Git & GitHub CLI** — Version control and repository management
- **Docker & Docker Compose** — Containerised development environments
- **VS Code** — Primary code editor (Development department)
- **OpenSSH** — Secure remote access to servers
- **APT (Advanced Package Tool)** — Package management and software deployment
- **ClamAV** — Endpoint antivirus and malware protection
- **OrangeHRM / Odoo / Metabase** — Department-specific web applications

---

## 📄 Licence

This project was produced as part of the **Tech Career Accelerator** training programme. All documentation is intended for educational purposes.
