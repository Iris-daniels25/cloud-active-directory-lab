# Digital Bloom Technologies Enterprise Infrastructure

## Project Overview

This project simulates the enterprise infrastructure for Digital Bloom Technologies.

The objective is to demonstrate real-world systems administration, cloud infrastructure, Windows administration, Linux administration, automation, networking, and security using enterprise best practices.

---

# Enterprise Environment

```
Internet
    │
    ▼
WEB01 (Oracle Linux)
    │
    │  (Future Active Directory Integration)
    │
───────────────
    │
DC01
Windows Server
Active Directory
DNS
Group Policy
    │
CLIENT01
Windows 11
```

---

# Windows Infrastructure

## DC01

Primary Domain Controller

Responsibilities

- Active Directory
- DNS
- Group Policy
- User Authentication
- Organizational Units

---

## CLIENT01

Windows workstation joined to the domain.

---

# Linux Infrastructure

## WEB01

Oracle Linux web server.

Maintained separately using the ansible-linux-webserver project.

Future integration:

- Active Directory authentication
- SSSD
- Kerberos
- SSH
- Nginx

---

# Organizational Units

```
Digital Bloom Technologies

Users
│
├── IT
├── Human Resources
├── Finance
├── Operations
└── Executives

Computers
│
├── Workstations
├── Servers
└── Test Machines

Groups
│
├── Security
├── Distribution
└── Administrative

Service Accounts

Domain Controllers
```

---

# Planned Servers

DC01
Primary Domain Controller

CLIENT01
Windows workstation

WEB01
Oracle Linux

FILE01
Windows File Server (Future)

DB01
Database Server (Future)

MON01
Monitoring Server (Future)

---

# Long-Term Goals

- Active Directory
- DNS
- Group Policy
- PowerShell Automation
- Linux Integration
- Ansible Automation
- Docker
- Monitoring
- Cloud Networking