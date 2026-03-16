# Server Infrastructure

The enviorment requires server infrastructure to fulfill monitoring requirements and provide necessary business services. 
#
Due to market fluctuations the price of RAM and Disk have multiplied and supply has swindled resulting in a market rise where old equipment from 2023 is now four times the price in 2026.

The cheapest hardware for this will be an older refurbished Lenovo Think Centre (or HP Elite Desktop) as a Mini PC. A few years ago these could sell for 50$ each, today it's much closer to 100$.
#
*Old used Dell Optiplex Desktops can go for around 50-60$ and will meet and even exceed our minimum server baseline.*
#
For ease of use, capability, and cost the operating system will be Ubuntu Server.
- Ubuntu Server lacks a Desktop Enviorment, which is the UI found on most desktops and is a resource intenseive service.
- Ubuntu is a popular Linux platform with plenty of community support and can meet the majority of any Linux server's needs.
- Ubuntu is naturally designed to mirror Windows as an accesible OS platform for most users. 
#
Ontop of Ubuntu Server, Docker will host services in containers, isolating services and streamlining deployment and recovery. 

The services needed are telemetry for equipment uptime and troubleshooting.

- Zabbix can be stood up easily in a seperate docker folder. It is a robust but complex Network Monitoring Solution.
    - Web Zabbix
    - Server Zabbix
    - Post Gres Database
    - Zabbix Agent
- phpIPAM, also in a seperate folder, is a better platform for inventory and IP management than Excel and is free. It's also easy to setup and use, although it is old.
    - Web phpIPAM
    - Server phpIPAM
    - mariaDB database
- Uptime Kuma is a dedicated uptime monitoring platform and will be the main source of telemetry for outages and meeting the 99.999% (five-nines) standard. 
- Nextcloud provides a local cloud as a Network Attached Storage solution. 
    - May need an external database, if so seperate into a different folder and deploy alongside mariaDB
- Vaultwarden will support strong password management internally.
#
Based on the containers and OS the estimated minimum would be:
    
    4-core N100/N150
    8 GB RAM