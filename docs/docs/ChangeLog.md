## 2026-06-06

### Raspberry PI Zeor PI-Hole Deployment Completed

Changes:
- Configured static IP
- Disabled Wi-Fi
- Installed Pi-hole
- Added OISD blocklist
- Verified DNS service
- Configured SSH access

Lessons Learned:
- Raspberry Pi OS Bookworm uses NetworkManager.
- Static IPs are configured through nmcli.
- Verify DNS operation with pihole status and pihole -g.
