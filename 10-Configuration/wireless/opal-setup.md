    Default 192.168.8.1
    https://192.168.8.1/cgi-bin/luci/

    Static IP on WAN as 10.10.x.x

    Plug Ins Update

    Apps

    luci
    luci-ssl
    luci-ssl-openssl
    iw
    htop
    luci-app-uhttpd

    More Settings
    Advanced
    Install Luci

    Reset WAN int as DHCP because ip conflict logic

    More Settings
    LAN IP
    10.10.x.x

    Then, 
    set WAN int as 10.10.x.x again

    Create the interface as an unmanaged int with eth0.X bridged to the radio network. For testing IOT on Radio1.2 (which was 2.5 guest) is easiest. 
    Then, advanced settings, bring up on boot, and firewall setting should be tied to LAN. 

    Next
    Network, Switch, add vlans. 
    don't add MGMT, VLAN2 is setup to surogate itself as MGMT when it goes to the uplink but acts as 2 for internal operations. 
    Add VLANS,
    make sure they have tagged on CPU and on WAN!
    Done.

    Next we need to configure the wireless networks now tied to our VLANs.
    Enable if needed
    Transmit power auto, 
    Mode Access Point, not WDS!

    Also for IOT under wireless and advanced settings isolate clients for security. 

    The only other thing is disable the block config access from wan rule or make a custom rule to allow our private network.  

    At then end, GIVEN WE ARE BEHIND A FIREWALL, change the WAN firewall zone to accept input, and viola. DNS, Console traffic, everything should work-albeit everything is open so do some hardening from the upstream firewall and backup the GL.iNet OPAL.

    Under backup generate backup tar file and also restore from that same menu. 

    **Due to hardware limitations this device only supports two SSIDs, so it is reccomended to host a GUEST and DATA vlan!**
    - Guest: Guests, Internet of Things, Untrusted devices and users.
    - Data: Trusted users and systems that need access to internal resources. 