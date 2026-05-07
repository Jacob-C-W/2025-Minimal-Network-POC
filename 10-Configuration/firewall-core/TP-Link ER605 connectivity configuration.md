# TP Link ER605 

## Getting Started

Broadband's initial config guide, for reference:
https://support.simplybroadband.co.nz/instruction/tp-link-er605


#
### DNS

PDNS will be NextDNS so login and create a free account and use the IP they provide. 

*Key IPs are generally **45.90.28.232 and 45.90.30.232**, though the network utilizes a broad 45.90.28.0/24 and 45.90.30.0/24 subnet*

Alternatively, OpenDNS IPs are **208.67.222.222 and 208.67.220.220**, they will still require an account for management, but provide PDNS regardless, however controls may be locked behind pricing. 

#
### VLANS

Refer back to our 05-Design/vlans.md document. 

#
### Segmentation

Prevent east-west traffic. 

No VLAN should have SSH access to VLAN 5 MGMT, except maybe data unless admin PCs are also on 5 MGMT.
10 Data and 110 Wireless Data should not have access to each other.
15 Server access should be regulated to specific users with credentials and access via 10 and 110.
            - 20 Guest/IoT
            - 120 Wireless Guest/IoT