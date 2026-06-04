# RBellotte-HomeLab
How I set up my Cyber Security home lab.

## Overview

## Security Notice

All IP addresses, hostnames, credentials, VPN configurations, cryptographic keys, and sensitive infrastructure details have been sanitized or redacted before publication.

This repository documents my personal cybersecurity homelab.

The purpose of this lab is to gain hands-on experience with:

- Linux administration
- Raspberry Pi infrastructure
- Pi-hole DNS filtering
- VPN technologies
- Network monitoring
- Documentation and change management

---

## Current Infrastructure

### Router

- Netgear Nighthawk RAX43

### Raspberry PI5 PI-Hole

Primary infrastructure node.

Hardware:
- Raspberry Pi 5
- 8 GB RAM
- 512 GB NVMe

Services:
- Pi-hole
- DHCP
- SSH

Network:
- Static IP: 192.168.xxx.xxx
- Ethernet only

### Raspberry PI Zero PI-Hole

Secondary infrastructure node.

Hardware:
- Raspberry Pi Zero W

Planned Services:
- Secondary Pi-hole
- DNS failover

Planned Network:
- Static IP: 192.168.xxx.xxx

---

## Future Projects

- VPN deployment
- Infrastructure monitoring
- Grafana
- Prometheus
- VM Server
- Security tooling

---

## Lessons Learned

### Raspberry Pi Networking

Modern Raspberry Pi OS uses:

- Netplan
- NetworkManager

Static IP configuration is performed using:

nmcli

rather than:

/etc/dhcpcd.conf

on newer installations.
