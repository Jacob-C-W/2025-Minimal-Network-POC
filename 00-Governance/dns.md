# DNS and URL Filtering Policy


Reccomended by CIS to use DNS Filtering Services and to maintain and enforce Network Based URL Filters, which can be done jointly. 

URL Filtering over Cloud Hosted DNS is a common practice today. 

*It is extremely difficult to maintain and manage a self hosted instance of DNS unless you are an enterprise entity. Failure to maintain DNS will lead to a massively increased attack vector and severe consequences.*

I wasn't able to find strong policy on using Cloud DNS policy. 

**Use a Protective DNS system.** DNS systems were not built to handle threats of the modern cyberscape and PDNS is a new technology incorperating greater security to compensate for threats. 

Block unauthorized DNS queries and requests. Stop all DNS traffic not directed towards the approved system. 

Account for architecture. Ensure policy applies to all wired, wireless, and VPN devices. 

#
    Free PDNS Options: NextDNS, OpenDNS.

- NextDNS only supports 300k queries a month which is not enough for a small business, only micro businesses and homes could function off of that. However, when queries run out it still works, but it runs like a classic DNS not a PDNS solution. 

- OpenDNS is free, but Umbrella is their enterprise grade product. 

#

**Source:** [CIS Controls 9: Email and Web Protections - 9.2 Use DNS Filtering Services](https://cas.docs.cisecurity.org/en/latest/source/Controls9/?utm_source=chatgpt.com#92-use-dns-filtering-services), [Selecting a Protective DNS Service](https://media.defense.gov/2025/Mar/24/2003675043/-1/-1/0/CSI-Selecting-a-Protective-DNS-Service-v1.3.PDF), 