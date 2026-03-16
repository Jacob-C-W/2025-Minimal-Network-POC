# VLANs

**Management, Internet of Things, Guest, Users**

NATIVE  01

    Not configured unless device requires Native traffic seperate from MGMT. 

MGMT    10

    All infrastructure will sit on the MGMT VLAN and SSH traffic will be implict deny. If management is accessible on HTTP/HTTPS that traffic will also be implicit deny.

USER    20

    All internal user traffic will fall here. 

GUEST   30

    Guest will be segmented into their own VLAN and client isolation controls will be applied. Furthermore, no traffic will leave the Guest VLAN except to reach internet. 

IOT     40

    Internet of Things traffics will be segmented like Guest, with client isolation applied where possible and no cross VLAN traffic.

DEAD    999

    All unused ports will be placed in the DEAD VLAN, all DEAD VLAN traffic will be black holed to prevent unauthorized access. 
#
## Wireless
**Wireless traffic will be handled on a segmented +100 VLAN**

    USER    120
    GUEST   130
    IOT     140

#

VLANs will be managed by access-list on the Core. 

# 

Potentially do a VLAN 25 for VPN-USERS

Potentially do a VLAN 45 and VLAN 145 for SECURITY or BUILDING devices that need seperation from IoT, but may need client isolation disabled. 