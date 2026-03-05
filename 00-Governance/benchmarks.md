# Benchmarks

Below are researched industry standard, benchmarks, and guidelines as well as definitions for those standards. These are to be best met as possible. 

# Overview
When feasible always strive for the Four Nines SLA - (99.99% Connectivity).
#
    Micro business
    1-10 people
    1000-5000$, basic router, a few access points, simple firewall. 
#
    Small Business
    10-50 people
    5000-15000$
    Business grade router, managed switches, multiple access points, dedicated server.
#
# Small Business Router Comparison Guide 
    Entry-Business
    25-50 Max Devices
    1500 sq.ft coverage
    basic QoS, VPN server
    150-300$
#
    Growing-Business
    50-100 Max Devices
    3000 sq.ft coverage
    advanced QoS, dual-wan, VLAN support
    300-700$
#
    Future Proof
    100+ Max Devices
    5000 sq.ft coverage
    high-throughput, advanced security, robust management
    700$
*[Network Setup for Small Business: Expert Guide to Get Started](https://adaptiveis.net/blog/network-setup-for-small-business/)*
#
# Micro versus Small Business
Micro Standards
- Basic Router allows connectivity between WAN and LAN. Does NAT at the edge. Provides basic DHCP and DNS forwarding. 
- Simple firewall is a stateless firewall that blocks and allows access based on URL, Port, and Protocol with limited other features. 
- Basic QoS is any method that helps the network remain usable and stable when a client or device is consuming too much bandwidth. Usually a fairness model. 
- VPN Server, service that permits remote authenticated, encrypted, policy controlled access into internal network and reosurces. 

Small Standards
- Business grade router is a standard set by the needs of the business according to policy. 
- Advanced QoS is application aware performance guarantees. Controls based on traffic type, policy, priorities, and more telemetry than Basic QoS.
- Dedicated server is an organization server seperate from customers that hosts org services. 
- High Throughput is a Gig routing and NAT speeds.
- Advanced Security features:
    - IPS
    - identity based controls
    - URL/DNS/category filtering
    - segmentation policies and enforcement
    - MFA
    - etc. 
- Robust management: 
    - Centralized management access
    - Role Seperation (admin/read-only)
    - Configuration backup and restore features
    - Logging and Telemtry capabilities
    - Update and maintenance processes
#
Sources: [What is a Dedicated Server?](https://aws.amazon.com/what-is/dedicated-server/?utm_source=chatgpt.com), [Set up your small business network](https://learn.microsoft.com/en-us/troubleshoot/windows-client/networking/set-up-your-small-business-network), [Network Setup for Small Business: Expert Guide to Get Started](https://adaptiveis.net/blog/network-setup-for-small-business/),  
[NIST SP 800-41 Rev. 1](https://csrc.nist.gov/pubs/sp/800/41/r1/final?utm_source=chatgpt.com), 
[Compare Traffic Policy and Traffic Shape to Limit Bandwidth](https://www.cisco.com/c/en/us/support/docs/quality-of-service-qos/qos-policing/19645-policevsshape.html?utm_source=chatgpt.com)
[NIST SP 800-77 Rev. 1](https://csrc.nist.gov/pubs/sp/800/77/r1/final),
[QoS: Classification, Policing, and Marking on LAC Configuration Guide, Cisco IOS XE Fuji 16.9.x](https://www.cisco.com/c/en/us/td/docs/ios-xml/ios/qos_lac/configuration/xe-16-9/qos-lac-xe-16-9-book/qos-class-lac.html?utm_source=chatgpt.com),
[NIST SP 800-46 Rev. 2](https://csrc.nist.gov/pubs/sp/800/46/r2/final?utm_source=chatgpt.com),
[NIST SP 800-128](https://csrc.nist.gov/pubs/sp/800/128/upd1/final?utm_source=chatgpt.com),