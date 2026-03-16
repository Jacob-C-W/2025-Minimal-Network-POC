# Inventory and Hardware List

The Core (Firewall and Router)

Managed Switch

Dedicated Server (Mini PC)

NAS (DAS as NAS)

Access Points

UPS with AVR or InLine

Patch panel

Ethernet Wall Plates

Surge Protectors

Cat6 Cables

# 

First impressions 
*Shooting from the hip*

1. TP Link ER605 Core
    - plus dedicated VPN companion device: Raspberry Pi or converted GL.iNet OPAL for Tailscale. 
2. Managed 8-Port NetGear Switch
3. HP Elite Desktop
    - Server infrastructure will be containerized via Docker
    - Running Linux, Ubuntu Server
4. DAS as NAS
    - Leverage a storage bay over USB, preferably USB C.
    - Nextcloud on Docker, over the LAN
5. GL.iNet OPALs, one per 20-25 users and within 10m of -80db frequency range. 
6. In Line AVR Amazon UPS, or AVR Gituroso UPS 
7. Cable management Vendor?
8. Cable management Venor?
9. Amazon basics surge protectors
10. Cable Vendor?


In another design we run a TP Link ENV

ER605 Core
EAP110 Access Points
TL-SG108E Switch
Raspberry Pi 3 Tailscale (VPN) Companion device

Conversely we run a...

GL.iNet Brume 2 Core
GL.iNet OPAL Access Points
Managed Netgear 8 port Switch


Server and services...exception due to disk and ram cost skyrocketing from industry and market fluctuation. 
