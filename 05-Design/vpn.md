# Tailscale Implementation

- Dedicated Exit Node or Route Advertiser, all traffic over VPN will be sourced and controlled by the VPN Device's IP. 
- All traffic will come from that designated VPN device.
- It will be a companion device to the firewall, so it will be subject to the firewall's rules.
- Policy will be configured in Tailscale's cloud access lists. 

Companion device will likely be a Raspberry Pi 3, due to the cost being low and the role being resource light. 