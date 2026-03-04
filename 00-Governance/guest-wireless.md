# Guest Network Policy

# Benefits of a Guest Network
    For hosting Guests
- Inherent seperation from LAN.
- Enchanced security and privacy.
- Good for hosting; helpful for contractors.

# Top security risks of unsecured guest Wi-Fi
    Unprotected guest Wi-Fi exposes several risks:
- Data theft – Attackers intercept unencrypted traffic or steal credentials.
- Malware distribution – Compromised devices can spread malicious payloads across the network.
- Man-in-the-middle (MITM) attacks – Unencrypted connections allow traffic tampering.
- Unauthorized network access – Guests bridging into internal systems can exfiltrate sensitive data.
- MAC spoofing – Attackers impersonate authorized devices to bypass controls.
- Compliance violations – Lack of logging and retention can result in regulatory penalties.
- Bandwidth abuse – Uncontrolled usage degrades performance for employees and critical services.
- Reputation damage – Visitors losing trust in unsafe Wi-Fi experiences.

# Compensating Controls
    Proper configuration can secure the network and the guests
- Guest will be forced to use WPA3 with a secure generated password
- Guest will be seperated from the Network and individually segmented (client isolation).
- Guest will have to use a Captive Portal with logging and Terms of Service
- Guest will have limited bandwidth to prevent abuse (QoS/Traffic Limiter)
- Guest will not have access to disreputable or risky sites (web filtering and access lists)
- Due to the Guest network's security posture it will also not share a password with any other service.
    - Due to password complexity it will also be shared via a physical QR code in the residence to ensure security and accessibility.


**sources:**
[Securing guest Wi-Fi: Key risks and best practices for 2026](https://www.cloudi-fi.com/blog/guest-wifi-security-best-practices),[Guest Wi-Fi - ITSAP.80.023](https://www.cyber.gc.ca/en/guidance/guest-wi-fi-itsap80023), [Top Five Requirements
for Guest Wi-Fi Access](https://docs.broadcom.com/doc/top5-guest-wi-fi-access-en)