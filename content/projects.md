---
title: "Projects"
date: 2026-06-07
draft: false
---

## Technical Projects

Source code and live deployments below.

---

### BISD Campus Vulnerability Scanner

**Tech:** Python, Debian LXC, WinRM, SNMP, LDAP, concurrent scanning

Network vulnerability scanner for Brenham ISD covering 10 school campuses. Identifies missing patches, unencrypted protocols, and policy violations across Windows/Linux/network infrastructure.

- **Platform:** Debian LXC container on Proxmox cluster
- **Scope:** WinRM security, SNMP configuration, LDAP binding, patch levels
- **Status:** Production scanning, monitoring service planned for school start 2026
- **Features:**
  - Multi-campus concurrent scanning
  - Credential-based authentication testing
  - Policy compliance checking
  - Automated report generation

---

### waynemcknight.com — Professional Resume Site

**Tech:** Hugo + Congo theme, GitHub Pages, custom CSS, Markdown

Personal professional site hosting resume and project documentation. Uses Congo's prose-focused theme with custom CSS widening for readability.

- **Repo:** [waynemcknight-code/waynemcknight.com](https://github.com/waynemcknight-code/waynemcknight.com)
- **Live:** [waynemcknight.com](https://waynemcknight.com)
- **Features:**
  - Full resume with 30+ years IT experience
  - Professional layout with Tailwind CSS overrides
  - GitHub integration for project links
  - Automated deployment via GitHub Pages

---

### BISD Infrastructure Documentation

**Tech:** Proxmox, Ceph, VMware ESXi, Active Directory, Cisco UC, Python automation

Architecture and operational documentation for Brenham ISD's multi-campus infrastructure.

**Virtualization & Storage:**
- Proxmox VE cluster with Ceph hyper-converged storage (EPYC-based)
- VMware ESXi hosts retained for Cisco Unified Communications (CUCM Pub/Sub, Unity, InformaCast)
- Proxmox Backup Server for centralized backup strategy
- ZFS pool management with post-outage hardening (reservations, ZED alerting)

**Identity & Networking:**
- Active Directory with Group Policy management across campuses
- Google Workspace for Education integration
- Cisco Meraki switching/wireless with VLAN segmentation
- Cisco CUCM and Cisco CUBE for VoIP infrastructure

**Automation & Monitoring:**
- Python-based monitoring and alerting
- Backup verification automation
- Operational tooling for incident response
- Video surveillance under FBI CJIS Security Policy

---

## Deployment

- GitHub Pages for static sites
- Proxmox LXC for vulnerability scanner
- GitHub Actions for automated builds and deployments
