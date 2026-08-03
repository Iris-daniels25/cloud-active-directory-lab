# Infrastructure Integration Plan

## Overview

The Digital Bloom Technologies Enterprise Infrastructure Lab is designed as a collection of connected infrastructure projects.

Each project remains independently documented and deployable while contributing to a larger enterprise environment.

The existing Ansible Linux Web Server project will represent the Linux web server named `WEB01`.

---

## WEB01

### Purpose

`WEB01` is the Linux web server for Digital Bloom Technologies.

It is maintained in a separate GitHub repository so the Ansible automation project can stand on its own as a complete portfolio project.

### Related Repository

[Ansible Linux Web Server Automation](https://github.com/Iris-daniels25/ansible-linux-webserver)

### Current Capabilities

The existing Ansible project demonstrates:

- Automated Nginx installation
- Custom webpage deployment
- Configuration management
- Service management
- Playbook idempotency
- Linux server verification

### Planned Enhancements

The Ansible project may later be expanded to include:

- Firewall configuration
- SSH hardening
- Automated security updates
- Non-root administrator accounts
- Fail2Ban
- Monitoring tools
- Reusable Ansible roles

---

## Planned Enterprise Integration

Once the Active Directory environment is available, `WEB01` may be integrated with the Digital Bloom Technologies domain.

Planned integration includes:

- Connecting `WEB01` to the enterprise network
- Using centralized DNS
- Joining Linux to Active Directory
- Configuring SSSD
- Configuring Kerberos authentication
- Allowing selected domain users to sign in through SSH
- Granting administrative access through an Active Directory security group
- Continuing to manage Linux configuration through Ansible

---

## Project Boundaries

The Active Directory and Ansible repositories will remain separate.

### Cloud Active Directory Lab

Responsible for:

- Active Directory Domain Services
- DNS
- Organizational Units
- Users and groups
- Group Policy
- Windows client management
- PowerShell automation
- Enterprise architecture documentation

### Ansible Linux Web Server

Responsible for:

- Linux server configuration
- Nginx deployment
- Security configuration
- Service management
- Automated provisioning
- Idempotency testing

This separation keeps each repository focused while showing how the projects could operate together in a real enterprise environment.

---

## Future Architecture

```text
Digital Bloom Technologies
│
├── DC01
│   ├── Active Directory
│   ├── DNS
│   └── Group Policy
│
├── CLIENT01
│   └── Windows domain workstation
│
└── WEB01
    ├── Linux
    ├── Nginx
    ├── Ansible-managed configuration
    └── Planned Active Directory integration