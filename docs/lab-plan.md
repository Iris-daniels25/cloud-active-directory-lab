# Digital Bloom Technologies Enterprise Lab Plan

## Project Goal

Build and document a small enterprise infrastructure environment for Digital Bloom Technologies.

The lab will demonstrate cloud infrastructure, Windows administration, Active Directory, networking, PowerShell automation, Linux integration, and enterprise documentation.

---

## Core Environment

### DC01

Primary Windows Server domain controller.

Planned services:

- Active Directory Domain Services
- DNS
- Group Policy
- User and computer authentication
- Organizational Unit management

### CLIENT01

Windows 11 workstation used to test:

- Domain joining
- User authentication
- Group Policy
- DNS resolution
- Access controls

### WEB01

Linux web server managed through the separate Ansible project.

Planned integration:

- Centralized DNS
- Active Directory authentication
- SSSD
- Kerberos
- SSH access through domain accounts

---

## Domain Design

### Organization

Digital Bloom Technologies

### Planned Domain

```text
digitalbloom.local