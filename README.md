# AdGuard Home on Dell Wyse 5070

## Project Overview

In this lab, I am using a Dell Wyse 5070 as a small home-lab server.

The first step is installing Proxmox VE. After Proxmox is working, I will deploy AdGuard Home and connect it to my segmented network.

AdGuard Home will eventually provide DNS filtering for the following networks:

- Trusted Home VLAN
- IoT VLAN
- Guest VLAN
- Production services

This project builds on my network-segmentation lab, but it is being documented as a separate GitHub project.

## Hardware

| Device | Purpose |
|---|---|
| Dell Wyse 5070 | Proxmox host |
| 64 GB internal storage | Proxmox and lightweight services |
| TP-Link ER605 | Router and DHCP |
| TP-Link TL-SG108E | Managed switch |
| TP-Link EAP610 | Wireless access point |

## Planned Deployment

```text
Dell Wyse 5070
└── Proxmox VE
    └── AdGuard Home
