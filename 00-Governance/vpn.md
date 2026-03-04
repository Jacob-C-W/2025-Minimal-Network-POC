# VPN Policy

- VPN doesn't grant full LAN access
    - VPN access is only to approved internal LAN.
- Role Seperation
    - Admins and users should be seperated.
- MFA must be applied where able.
- VPN access should be supported by more than just passwords
    - Incorperate more controls. IE: certs, URL filtering, etc. where feasilble. 
- All unecessary features on the VPN should be disabled. 
- Management interfaces must not be exposed to public internet. 
- Cryptography should be modern and secure.
- VPN configurations must be monitored and maintained over time. 
- Remote access must respect network segmentation:
    - Guest networks remain isolated
    - IoT remains isolated
    - VPN users receive access only to approved zones/services
- VPN access must be monitored and logged.
- VPN solution must be kept up to date.
- All configurations should be backed up according to policy.



**Sources:** [NSA, CISA Release Guidance on Selecting and Hardening Remote Access VPNs](https://www.nsa.gov/Press-Room/News-Highlights/Article/Article/2791320/nsa-cisa-release-guidance-on-selecting-and-hardening-remote-access-vpns/),[NIST SP 800-46 Rev. 2](https://csrc.nist.gov/pubs/sp/800/46/r2/final?utm_source=chatgpt.com),