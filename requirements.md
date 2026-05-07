# Requirements

1. Connectivity
2. VLAN segmentation
3. Guest Network
4. IoT Network
5. Remote Access over VPN
6. Non Carrier Assigned DNS
7. Backup and Restoration Steps
8. Hardening checklist

#
# Tracker

    Governance: 

1. Connectivity [x]
2. Segmentation [x] 
    - (zone, acl, isolation, and segmentation) 
3. Guest Network [x]
4. IoT Network [x]
5. Remote Access over VPN [x]
6. Non Carrier Assigned DNS [x]
7. Backup and Restoration Steps [x] (rule-of-three and data retention)
8. Hardening checklist [x]
#
    Design:
1. Core Design [x]
2. Core Analysis (Firewall router assessment) [x]
3. Docker (server) [x]
4. DNS (nextdns) [x]
5. Wireless [x]
6. Inventory [x]
7. Data Retention [x]
8. VLANs [x]
9. VPN [x]
10. AND MANY MORE...
    Configuration:
1. TP Link ER605
2. NetGear Managed Switch
3. GL.iNet OPAL
4. Ubuntu Server [x]
    1. Services [x]
    2. Zabbix [x]
    3. phpIPAM [x]
    4. Nextcloud [x]
5. Tailscale
6. NextDNS
#
    Deploy!!!

    For deployment to work we need:

    - Internet connectivity from ISP
        - AT&T Fiber
    Firewall-core built: 
        - PDNS
            - NextDNS setup on core and rules applied via webgui. 
            - Track and log suspiscious and foreign traffic. 
        - VLANs
            - 5 MGMT
            - 10 Data
            - 110 Wireless Data
            - 15 Server
            - 20 Guest/IoT
            - 120 Wireless Guest/IoT
        - QoS ???
        - Stateful Rules
            - East West VLAN rules
            - SSH access limited
            - Log and monitor any flagged traffic, compare with PDNS
                - Create new rules as needed, Quarterly review reccomended. 
    Switch built:
        - VLAN tagging
        - Port assignment 
    VPN Companion Device built:
        - Tailscale installed on companion device
        - Exit node OR Route advertisement
    Wireless APs built:
        - Luci installation
        - VLAN tagging on switch menu
        - Radio configuration (wireless component)
        - Add ALC exception for management over the uplink on LAN. 
    Server built:
        - Ubuntu setup process 
        - Docker Compose setup
        - Docker compose files
            - Nextcloud
            - phpIPAM
            - Services
            - Zabbix
        - DAS
            - Auto external mount (linux)
            - External storage config in Nextcloud



