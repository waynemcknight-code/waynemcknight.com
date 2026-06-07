---
title: "Projects"
date: 2026-06-07
draft: false
---

## Technical Projects

Source code and live deployments below.

---

### Network Infrastructure Vulnerability Scanner

**Tech:** Python, Debian LXC, WinRM, SNMP, LDAP, concurrent scanning

Configurable multi-site network vulnerability scanner. Identifies missing patches, unencrypted protocols, and policy violations across Windows/Linux/network infrastructure. Framework with interactive setup wizard for any organization.

- **Repo:** [waynemcknight-code/network-scanner](https://github.com/waynemcknight-code/network-scanner)
- **License:** MIT (open source, free to use/modify)
- **Deployment:** Docker, LXC, or native Python
- **Features:**
  - Interactive setup.py for site/credential configuration
  - Multi-site concurrent scanning
  - Credential-based authentication testing
  - Policy compliance checking
  - HTML/JSON/CSV report generation
  - Scheduled scanning (cron, Docker, Kubernetes)

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

### Multi-Campus Infrastructure Architecture

**Tech:** Proxmox, Ceph, VMware ESXi, Active Directory, Cisco UC, Python automation

Design and implementation of hyper-converged virtualization infrastructure across multiple campuses.

**Virtualization & Storage:**
- Proxmox VE cluster with Ceph hyper-converged storage (EPYC-based)
- VMware ESXi hosts for specialized workloads (Cisco Unified Communications)
- Proxmox Backup Server for centralized backup strategy
- ZFS pool management with post-outage hardening (reservations, ZED alerting)

**Identity & Networking:**
- Active Directory with Group Policy management across sites
- Google Workspace for Education integration
- Cisco Meraki switching/wireless with VLAN segmentation
- Cisco CUCM and Cisco CUBE for VoIP infrastructure

**Automation & Monitoring:**
- Python-based monitoring and alerting
- Backup verification automation
- Operational tooling for incident response
- FBI CJIS Security Policy compliance (video surveillance)

---

## Deployment

- GitHub Pages for static sites
- Proxmox LXC for vulnerability scanner
- GitHub Actions for automated builds and deployments
