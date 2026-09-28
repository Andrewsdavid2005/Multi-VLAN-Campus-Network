# Multi-VLAN Campus Network 🚀

A medium-level enterprise campus networking project designed and
implemented using Cisco Packet Tracer.

The project demonstrates VLAN segmentation, inter-VLAN routing,
DHCP, EtherChannel, STP, SSH, DNS, HTTP services, and network
troubleshooting.

---

## 📌 Project Overview

This project simulates a campus network with multiple departments
using separate VLANs.

The network provides:

- Department-based VLAN segmentation
- Inter-VLAN communication
- Automatic IP address assignment
- Link aggregation using EtherChannel
- Spanning Tree Protocol
- Secure SSH device management
- DNS services
- HTTP web services
- Network troubleshooting and fault injection

---

## 🌐 Network Topology

The network consists of:

- 1 Cisco 2911 Router
- 2 Cisco 3560 Layer 3 Switches
- 3 Cisco 2960 Access Switches
- 8 PCs
- 1 Server

### Network Architecture

```text
                         R1
                          |
                   10.255.10.0/30
                          |
                       L3-SW1
                     ║ ║
                EtherChannel
                     ║ ║
                       L3-SW2
                    /     |     \
                  SW1    SW2    SW3
                 / | \   / \   / | \
               PC1 PC2 PC3 PC4 PC5 PC6 PC7 PC8
                                      |
                                    Server
