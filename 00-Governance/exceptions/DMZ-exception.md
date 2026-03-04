# DMZ Exception due to Wireless Limitations

If we wanted to do an untrusted zone on a seperate firewall interface we would have to double the access points and RF noise with seperate access points, which isn't practical. 

    We will manually segment and isolate IoT and Guest traffic without a DMZ. 

1. We will enable client isolation on the GL.iNet wireless access points for Guest and IoT WLANs. 

2. Access rules will prevent cross VLAN talk for both Guest and IoT. 

3. URL filtering lists and custom rules will be applied to regulate both networks strictly.