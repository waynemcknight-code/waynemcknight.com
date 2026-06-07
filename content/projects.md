---
title: "Projects"
date: 2026-06-07
draft: false
---

## Technical Projects

Work generated in collaboration with Claude AI. Source code and live deployments below.

---

### aiether.info — Accountability & Investigation Site

**Tech:** Hugo + Congo theme, GitHub Pages, Playwright, RSS automation

A documentation-focused site for publishing civil rights litigation patterns, government accountability failures, and public records analysis. Built with automated RSS republishing of Corruption Watch TX and custom Playwright-based backfill for missing articles.

- **Repo:** [waynemcknight-code/aiether.info](https://github.com/waynemcknight-code/aiether.info)
- **Live:** [aiether.info](https://aiether.info)
- **Features:**
  - Six federal civil rights cases against Colorado County documented with full case details
  - Monell pattern evidence compilation
  - TCJA compliance failure tracking
  - TPIA/AG ruling documentation
  - Automated RSS cron for Corruption Watch TX
  - Playwright script for article backfill and HTML parsing

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

### Memory System for Legal Case Management

**Tech:** Markdown, YAML frontmatter, Git, structured memory organization

A persistent, session-independent memory system for tracking complex legal matter details, timelines, defendants, and investigative threads.

**Features:**
- Categorized memory files (user, project, feedback, reference)
- [[cross-linking]] between related memories
- MEMORY.md index for quick lookup
- Automatic context loading across Claude AI sessions
- Temporal accuracy (absolute dates instead of relative)

**Active Cases:**
- McKnight v. Colorado County Jail (§1983/Monell civil rights matter)
- BISD pentest scanner deployment
- aiether.info documentation projects

---

## Infrastructure & Platforms

**Primary Development Environment:** TheAlien (GPU-equipped Debian system)
- Ollama for local LLM inference (llama3.2, qwen2.5-coder)
- Git/GitHub SSH configured for automated commits
- HOTAS controller + xCloud setup for stress-testing during heavy compute

**Deployment:**
- GitHub Pages for static sites (waynemcknight.com, aiether.info)
- Proxmox LXC for vulnerability scanner
- GitHub Actions for automated builds and deployments

---

## Code Generation Approach

All projects in this portfolio were built collaboratively with Claude AI using:
- **Iterative design:** requirements clarification → architecture → implementation → testing
- **Local-first computation:** Ollama for token-efficient prototyping, Claude for complex reasoning
- **Version control:** Every commit documented and reversible
- **Security-first:** Private keys, credentials, sensitive data never committed to public repos

