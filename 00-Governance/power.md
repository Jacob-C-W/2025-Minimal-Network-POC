## Policy objective is **risk reduction**

Topics:

    - UPS
    - Wattage (AC/DC)
    - Ground/Bond
    - Surge Protection
    - Breaker seperation
    - Power Supply

Commercial Standard: 
- All network and telecom equipment shares a properly bonded, coordinated grounding path tied into the building’s electrical grounding system:

All permanently installed network equipment must be connected within a coordinated grounding and bonding scheme tied back to the premises electrical grounding system; 

- Installations must follow code and manufacturer instructions;
- Any rack, cabinet, patch panel, or surge protective device added to the environment must be evaluated for bonding needs; 
- And any new or changed work should be performed or reviewed by a qualified electrician or low-voltage professional where required by code.

**Grounding and bonding are not the same thing:** grounding helps stabilize voltage and limit imposed voltage from lightning or surges, while bonding creates an effective fault-current path so protective devices can operate properly.

- Use properly grounded electrical outlets
- Use listed surge protection where appropriate
- Avoid improvised rack grounding methods
- Bond metal racks or cabinets when installing structured cabling or rack-mounted gear
- Coordinate any serious grounding work with electrical code requirements 

*Network reliability depends partly on electrical discipline, not just good IT hardware.*

*Where required, installation and verification will be performed by qualified personnel.*

- Survey and inspect all power related equipment annually to avoid potential electrical fires or other equipment disaster scenarios. 
#
Power Supplys, surge strips, surge suppressors, and UPS devices are compensating controls in an electrical system. 
#
Power Supply
- Place the equipment in an area that accommodates the power consumption and component heat dissipation specifications.
- Be sure that your power supply meets the site DC power or AC power requirements of the network equipment.
- When you connect power to installed equipment, do not make this connection through an extension cord or power strip.
- If your switch includes more than one power supply, connect each power supply to a different, independent power source.
    - If a power source fails, it will affect only the switch power supply to which it is connected. If all switch power supplies are connected to a single power source, the entire switch is vulnerable to a power source failure.
- In regions that are susceptible to electrical storms, plug your system into a surge suppressor.

#
Uninterruptible Power Supply
- Absorb relatively small power surges.
- Smooth out noisy power sources.
- Continue to provide power to equipment during line sags.
- Provide power for a period of time after a blackout has occurred.
#
Surge Devices:
- Surge suppressors and surge protectors both guard electronics against voltage spikes, but they differ in capacity and application. 
- Surge suppressors generally handle higher loads in industrial settings. 
- Surge protectors are more common, offering moderate protection for home/office electronics.
- Surge arrestors exist at the service entrances and protect against surges external from the electrical system, like lightning strikes. However, their protection level usually leaves still enough residue electrcity to harm household electronics. 
- SPD, or surge protection device, is a low voltage head end system used to take high voltage input and regulate it down to a safe level for household electronics. 

#
*Always follow applicable industry standards.*
#
For more information, see the following ANSI/TIA/EIA standards:

    ANSI/TIA/EIA-568-A—the six subsystems of a structured cabling system
    ANSI/TIA/EIA-569-A—design considerations
    ANSI/TIA/EIA-606—cabling system administration
    ANSI/TIA/EIA-607—commercial building grounding and bonding requirements
#
**Sources:** [ExtremeNetworks Site Preperation](https://documentation.extremenetworks.com/wired/5520/GUID-1EED548C-1A26-4EF5-AE03-5F4A2D03E2FE.shtml), [Difference between Surge Protection Devices and Surge Arrester](https://www.chintglobal.com/au/en/about-us/news-center/blog/difference-between-surge-protection-devices-and-surge-arrester.html), [SPD, Surge Suppressor, And Surge Arrester Differences](https://www.britecelectric.com/blog/spd-surge-suppressor-and-surge-arrester-differences/)