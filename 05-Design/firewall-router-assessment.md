

# VPN
I will always push for **Tailscale** as a cloud based VPN service that is initially free and can be scaled at a cost to meet business needs. However, they're the new kid on the block and not as widely supported on many quick, easy, and cheap Firewall/Router solutions. 

If you are carrier NAT'd then you cannot run a traditional self hosted VPN server. You will need to rely on a cloud platform, like Tailscale, or you will need to call and likely pay for a dedicated public IP address so self hosted VPN is possible. 

However, Tailscale manages this all for a low to zero cost and takes maintenance and manegement out of the organizations hands. They support policy management and role seperation and I throughly reccomend them. 

Hence, they are why I push our reccomended Firewall/Router solution because of its out-of-the-box support for Tailscale despite other similarly priced competitors.

# The Core (Firewall and Router)

The all in one design of a firewall and router is common in smaller networks. We centralize management and resources into a single platform that then is propagated down to supporting infrastructure.

This leads to a simpler top down design where all rules are enforced in one plane. It is a single source of truth but also a single point of failure.  
#

# Options:
So, I push for an all in one firewall-router solution with tailscale functionality or with a companion device running Tailscale and advertsing routes or acting as an exit node to provide remote access.
#

**GL.iNet Brume 2**
- Unique strengths
    - Tailscale runs on the gateway itself, with a simple appliance-style UI.
    - All remote access policy can be centralized on one box.
    - Built-in DNS filtering path (AdGuard Home / DNS-based lists).
    - Lowest operational overhead.
- Best when
    - Checks every box but doesn't exceed either other solution. Tailscale support built in and all requested features present. 

**TP Link Er605**
- Unique strengths
    - Cheapest, simplest gig-class core for VLAN/DHCP/DNS forward/basic firewall and basic traffic control—easy to standardize.
    - Clean separation of concerns:
    - ER605 = “routing + segmentation brain”
    - companion = “VPN/Tailscale entry point”
    - Easier to keep the core stable: the core router doesn’t change much; remote access evolves on the companion without risking the whole office edge.
    - Best “budget scaling” path: you can keep the same core and upgrade only the companion if VPN needs grow later.
- Summary
    - No native Tailscale support, feature full and still easy adaptation core solution. 

**Asus ExpertWiFi EBG15**
- Unique strengths
    - Most “SMB feature bundle” in one box at consumer-ish pricing:
    - VLAN support, QoS modes, URL/keyword filtering, and vendor-packaged “security features” (IPS-style marketing) and reporting.
    - Better “leader appeal” UI/UX: tends to present as a business product with dashboards, app/web management, and “policy knobs” non-engineers understand.
    - Strong QoS story out of the box (basic → more advanced modes) compared to many cheap routers.
- Summary
    - Commercial grade security and QoS with minimal overhead (the least of all solutions), however little customization and lack of Tailscale support 

#
# Companion Device

[Setup TailScale on GL-SFT1200](https://docs.google.com/document/d/e/2PACX-1vQDYxqF43ty91F8nbpam9W3y54y9yXOMRPuX1J1yfmxiZTKfhiqNTVn9SMxldfx_WaKHSUxduMPIXJJ/pub)

So it is possible to buy a 30$ GLiNet OPAL or 25$ used Raspberry Pi and configure a dedicated exit node for Tailscale for your network. But it will take a bit more know-how and troubleshooting. 

#

## Conclusion
The TP-Link ER605 is the highest value core option, and can work with Tailscale given a 25-35$ companion Raspberry Pi 3 that will advertise routes or serve as an Exit Node. 
