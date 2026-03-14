# Netwerkdiagram

## Overzicht

Internet
   │
   │ WAN: 192.168.1.54
   │
[pfSense Firewall/Router]
   │ LAN: 10.0.0.1
   │
[LAN Switch — 10.0.0.0/24]
   ├── DC01  — 10.0.0.10  (AD · DNS · DHCP)
   ├── FS01  — 10.0.0.20  (File Server)
   ├── CLIENT01 — DHCP    (Windows 11)
   ├── CLIENT02 — DHCP    (Windows 10)
   └── CLIENT03 — DHCP    (Windows 10)

Clients zijn domain-joined aan DC01 (Kerberos authenticatie)
Domein: homelabtechnologies.local
