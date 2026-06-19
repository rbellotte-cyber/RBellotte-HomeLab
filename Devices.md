# Device Inventory

## Router
### Netgear Nighthawk RAX43
Role:
* Primary router
* Internet gateway

Status:
* Operational
Notes:
* Future migration planned from 192.168.xxx.xxx to 192.168.xxx.xxx
---

## Hostname: Mirum
* Device: Microsoft Surface Pro 11th Edition
* CPU: Snapdragon X 10-Core X1P64100 @ 3.4 GHz
* RAM: 16 GB
* OS: Windows 11 ARM64
* Purpose:
	* GitHub administration
	* Home Lab documentation
	* Future management workstation
--

## Raspberry Pi 5 Pi-hole
Role:
* Primary infrastructure node

Hardware:
* Raspberry Pi 5
* 8 GB RAM
* 512 GB NVMe

Services:
* Pi-hole
* DHCP
* ssh

Network:
* Static IP configured
* Ethernet only

Status:
* Operational

Notes:
* Booting from NVMe
* Wi-Fi disabled
---

## Raspberry Pi Zero W Pi-hole
Role:
* Secondary infrastructure node

  Hardware:
* Raspberry Pi Zero W

Services:
* Pi-hole
* ssh
* Secondary DNS
  
Network:
* Static IP configured
* Ethernet only

Status:
* Operational

Notes:
* OISD installed
* Wi-Fi disabled
* Configured as secondary DNS server and failover service
---

## Raspberry PI 5 (Undefined)

Purpose:
- Infrastructure Services Node

Hardware:
- Raspberry Pi 5
- 8 GB RAM
- 512 GB NVMe
- 2 TB NVMe
- Pironman 5 Max Case

Network:
- Static IP: 192.168.xxx.xxx
- Ethernet Only
- Wi-Fi Disabled

Status:
- Raspberry Pi OS Lite (64-bit)
- SSH Enabled
- Fully Updated  
Notes:
* Currently functioning primarily as a network distribution switch
* Future configuration planned
---

## Future Raspberry Pi 5

Role:
* Undecided

Potential Uses:
* Monitoring
* Grafana
* Prometheus
* Logging
* Infrastructure management

Planned Storage:
* 512 GB NVMe (OS and Services)
* 2 TB NVMe (Data and Backups)

Status:
* Planning Phase
---

## Future VM Server

Hardware:
* Intel i9-10900KF
* 32 GB DDR4 RAM
* RTX 3060 12 GB

Potential Uses:
* Virtualization
* Lab environments
* Security testing
* Monitoring infrastructure

Status:
* Planning Phase
