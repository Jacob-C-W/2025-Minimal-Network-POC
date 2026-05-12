# 2025 Minimal Network POC
## Placeholder ReadMe.md

**Managed Small Scale Network 2025 Proof of Concept**

A complete, affordable, and secure network blueprint designed for small offices (10–30 users, 30–100 endpoints) that can be deployed in homes or light commercial environments.

## Project Overview

Over several weeks I designed, documented, and planned a full-stack minimal network from the ground up. The goal was to create a practical, repeatable blueprint that prioritizes **security, segmentation, manageability, and cost-effectiveness** while meeting real-world small-business needs.

### What Was Built (Documentation + Design)

- **Governance & Policy** (00-Governance folder)  
  Created policies for backups (3-2-1 rule), network hardening, segmentation, guest/IoT isolation, monitoring, DNS, VPN usage, power management, and cable standards.

- **Network Design** (05-Design folder)  
  Defined core architecture (collapsed core firewall/router), VLAN strategy, wireless design, Docker services, data retention, inventory, and NextDNS integration.

- **Configuration Guides** (10-Configuration folder)  
  Detailed setup for TP-Link ER605 firewall, Netgear managed switch, GL.iNet Opal VPN companion, Ubuntu Server with Docker, Zabbix monitoring, phpIPAM, and Nextcloud.

- **Additional Work**  
  Goal & requirements documentation, AI-assisted testing notes, and deployment checklists.

## Key Security & Design Highlights

- Strict network segmentation (Management, User, Guest, IoT) with wireless equivalents (+100 VLANs)  
- Client isolation on Guest & IoT networks  
- NextDNS for encrypted, filtered DNS with logging  
- Stateful firewall rules and east-west traffic control  
- Tailscale VPN for secure remote access  
- Hardening checklist based on CISA guidance  
- 3-2-1 backup strategy with quarterly reviews  
- Docker-based services on Ubuntu for easy management and isolation  

This POC proves that a highly secure and manageable network can be built with consumer/prosumer hardware while following enterprise-grade principles.

## Why This Matters

This project gives me (and anyone using it) a ready-to-deploy template that balances usability with strong security — exactly what small organizations need in 2025 and beyond.
