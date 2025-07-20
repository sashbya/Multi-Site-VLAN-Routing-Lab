# Multi-Site-VLAN-Routing-Lab

## Overview
This lab simulates a multi-site corporate network with VLAN segmentation and inter-VLAN routing. 
It demonstrates key CCNA-level concepts like VLAN configuration, trunking, router-on-a-stick, and inter-router static routing.

## Network Topology
- 3 Routers: R0 (HQ), R1 (Branch 1), R2 (Branch 2)
- 2 Switches: SW1, SW2
- 4 PCs in two VLANS:
  - VLAN 10 - Users
  - VLAN 20 - Admin

Link to Topology picture [here](vlan-roas-topology.png).

## Technology and Competencies
- Cisco Packet Tracer
- VLANs, Trunking (802.11q)
- Subinterfaces (Router-on-a-stick)
- Static Routing between routers

## Key Concepts
 Proper VLAN port assignments per PC
- Trunk ports between routers and switches
- Subinterfaces on routers for VLAN gateway IPs
- Static routing between R0, R1 and R2 to allow cross-VLAN, cross-site communication

## Tests

| Test | Expected Result |
|------|-----------------|
| PC0 → PC1 | Ping succeeds (same switch, different VLANs) |
| PC0 → PC2 | Ping succeeds (same VLAN, different switch) |
| PC1 → PC3 | Ping succeeds (same VLAN, different site) |

## Outcome

All four PCs across two VLANs and two switches can communicate through inter-VLAN routing and inter-site static routes.


## Learnings

- Multi-router routing logic
- VLAN troubleshooting (native VLAN mismatches, access vs trunk mode)
- Modular design simulating real-world network tiers (HQ/Branches)

## Files
