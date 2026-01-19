# Enterprise Zero Trust Network
Self-directed cybersecurity apprenticeship: Zero Trust, networking, identity, VPN, logging, attacks, and defense.

This repository documents my self-directed cybersecurity apprenticeship where I am building an enterprise-style Zero Trust environment from the ground up.

## Phase 1 — Foundations (Completed)
In Phase 1 I learned and practiced:

- Linux network visibility (interfaces, routing, packet capture)
- Subnetting and segmentation concepts
- Firewall trust boundaries and attack surface awareness
- Identity fundamentals using RADIUS (basis of 802.1X / NAC)
- VPN and encrypted tunnel fundamentals
- System logging and SOC/SIEM visibility

## Phase 2 — Enterprise Segmentation & Firewall (In Progress)  
Design and deploy an enterprise-style segmented network enforced by a stateful firewall using Zero Trust principles.

**Session 1–2 Accomplishments:**
- Built a multi-interface pfSense firewall.
- Created isolated security zones:
  - WAN (Attacker / Untrusted) – 10.10.50.0/24  
  - LAN (User) – 10.10.10.0/24  
  - OPT1 (Server) – 10.10.20.0/24  
  - OPT2 (Management) – 10.10.30.0/24  
- Implemented:
  - Static IP addressing for infrastructure zones
  - DHCP for user endpoints
  - ZFS-backed firewall installation
  - Interface-level segmentation and routing
- Enforced all inter-zone traffic through a single policy control point (pfSense).

**Skills Being Developed:**
- Internal segmentation firewall design  
- Zero Trust network architecture  
- Routing and trust boundary enforcement  
- Enterprise IP addressing strategy  
- SOC visibility through controlled choke points  

**Outcome So Far:**  
> I have deployed a multi-zone enterprise firewall enforcing Zero Trust segmentation between untrusted, user, server, and management networks, replicating real-world security architecture used in corporate and government environments.

## Next Phases
- Phase 3: Attack the environment (simulate real threats)
- Phase 4: Defend, detect, and document (SOC detections + reporting)
