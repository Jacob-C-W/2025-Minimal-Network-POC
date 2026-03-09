# DMZ Exception due to Wireless Limitations

If we wanted to do an untrusted zone on a seperate firewall interface for Access Points we would have to double the access points and RF noise with seperate access points, which isn't practical. 

    We will manually segment and isolate IoT and Guest traffic without a DMZ. 

1. We will enable client isolation on the GL.iNet wireless access points for Guest and IoT WLANs. 

2. Access rules will prevent cross VLAN talk for both Guest and IoT. 

3. URL filtering lists (via DNS) and custom rules on the firewall will be applied to regulate both networks strictly.

Furthermore, a DMZ would double our most expensive component, the Core (Firewall/Router). One can be added but that will not be a requirement to start. I may add guidance on that after first publish. 