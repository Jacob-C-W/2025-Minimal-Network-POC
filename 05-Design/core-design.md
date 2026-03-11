# Design

# Equipment

## Core
At the top of our design the edge where the LAN meets the internet will be the Firewall/Router, our Core. 

It will leverage several technologies to ensure fast, reliable, and secure speeds. 
- Secure
    - Enforced PDNS (NextDNS with Url Filtering)
    - Stateful firewall
    - VLANs and segmentation
- Fast and reliable
    - Non Carrier DNS
    - Basic QoS
#
*Technically collapsed core.*

<!-- Only if Tailscale is being used with a non compatible Core. -->
## Remote Access (VPN Companion)
 - Dedicated Tailscale node
    - Exit node or Advertise Routes
    - Leverages Stateful firewall to police
    - Cloud based policy controls

## Switch
- Managed
- VLAN tagging and passing. 

## Server
- Ubuntu Server OS
- Mini PC, HP Elite Desktop or Lenevo ThinkCentre
- Docker
- (8gb-16gb) Ram min.

## Wireless
- Multiple radios (SSIDs)
- VLAN support
- Client Isolation
- Managed
- WPA3
- Captive Portal Support

## UPS 
- Estimate wattage requirements and slightly exceed them on UPS solution
- AVR minimum, In Line preferred (InLine also needs AVR)
    - AVR - Volage Regulation
    - In Line, power constantly filtered through battery

# Architecture

## Layout

Internet connects to Core, Core handles core and distribution responsibilities, combines firewall and router role. 
#
*On a seperate interface of the Core, or on an isolated interface on the switch the VPN companion device hangs providing RMA.*
#
Core connects to managed switch which is the access layer. Switch passes on the VLANs provided by the Core to all endpoints and infrastructure. 

Server, Access points, and clients hang off the switch, wireless clients hang off the access points. Access points are trunked. 

## VLANs
VLAN outline:
 - Management
 - IoT
 - Guest
 - Data

 Seperate wireless vlans for: IoT, Guest, Data, Security

 *Jump by 5s to leave space for future expansion, wireless just add a hundred or multiply by 10 if able.*

    Example, VLAN 10 IoT and VLAN 110 WirelessIoT.


