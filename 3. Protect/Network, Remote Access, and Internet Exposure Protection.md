---
icon: triangle-right
order: 30
---
### Goals

The company network is the path into devices, servers, cloud platforms, printers, cameras, Wi-Fi, remote access tools, and business applications.

If the network is flat, exposed, unmanaged, or full of old rules, attackers have more room to move. A weak firewall rule, exposed remote desktop service, old VPN account, public admin panel, or forgotten test site can become the opening point for a larger incident.

This section defines how the company protects its network, remote access paths, Wi-Fi, firewalls, routers, exposed services, internet-facing systems, and network management interfaces.

The goals are simple: know what is connected, know what is exposed, reduce unnecessary access, and make remote access safer.

## Step 1: Assign Network Ownership

Start by assigning clear ownership.

The company should have a named person or provider responsible for the firewall, Wi-Fi, VPN, remote access, public IP addresses, domain exposure, and network equipment. This may be an internal IT lead, MSP, network provider, or technical manager.

**The company should determine who owns:**

- Firewall administration
- Wi-Fi administration
- VPN and remote access
- Public IP addresses
- Domain and subdomain exposure
- Network device firmware
- Firewall rule changes
- Vendor remote access
- Branch office or home office network controls

If a network system has no owner, it will usually become outdated, misconfigured, or forgotten.

## Step 2: Create a Network and Exposure Register

Create a simple register of the company’s network and internet-facing systems.

This does not need to be complex. A spreadsheet is acceptable.

Record each firewall, router, switch, Wi-Fi controller, VPN system, public server, cloud gateway, public IP, domain, subdomain, and exposed service.

For each item, record the system name, owner, location, public IP or domain, open ports, business purpose, admin access, MFA status, firmware version, logging status, configuration backup status, last review date, main risk, and next action.

This register helps the company find forgotten firewall rules, old VPN access, exposed test systems, public admin panels, and systems that nobody officially owns.

## Step 3: Draw a Simple Network Map

Create a basic map showing how the network is arranged.

The map should show the internet connection, ISP modem, firewall, switches, Wi-Fi networks, servers, cloud connections, VPNs, guest networks, vendor access paths, public services, and important internal zones.

It should also show sensitive areas such as finance systems, HR systems, servers, backup systems, admin systems, and any cloud or hosted environments.

The map does not need to look like an enterprise architecture diagram. It needs to be accurate enough for the company to answer:

- What connects to what?
- What is exposed to the internet?
- Where do remote users enter?
- Where do vendors enter?
- Where are the sensitive systems?
- Where are guest, personal, or IoT devices separated?

If the company cannot draw the network simply, it probably does not understand the network well enough.

## Step 4: Review the Firewall

The firewall is one of the company’s main control points.

Review the firewall configuration carefully. Check that admin accounts are named, MFA is enabled where supported, firmware is current, remote administration is not exposed to the public internet, and configuration backups are stored safely. Then review the rules.

Every inbound firewall rule should have a clear business reason, owner, source, destination, port, protocol, creation date, and review date. Temporary rules should have expiration dates.

Challenge old rules and remove rules that are no longer needed. Restrict broad rules. Replace unsafe exposure with safer access methods.

**Pay special attention to:**

- Public RDP
- Public SSH
- Public database ports
- Public NAS access
- Public backup consoles
- Public admin panels
- Old vendor access rules
- Temporary support rules that were never removed
- Rules allowing traffic from anywhere

A firewall rule without an owner should be treated as a problem.

## Step 5: Remove Direct Exposure to Admin Interfaces

Management interfaces should not be open to the internet.

Check firewalls, routers, switches, VPN appliances, NAS devices, hypervisors, backup consoles, camera systems, printers, website hosting panels, cloud admin consoles, and RMM tools.

Admin access should normally be limited to a VPN, trusted admin network, zero trust access tool, or approved management path. MFA should be enabled where available.

Do not expose an admin page because it is convenient. That convenience can become the attacker’s entry point.

## Step 6: Protect Remote Access

Remote access must be controlled tightly.

List every method people use to connect from outside the office. Include VPN, remote desktop, SSH, remote support tools, RMM platforms, ZTNA tools, vendor portals, cloud admin consoles, and emergency access methods.

For each one, check that users have named accounts, MFA is enabled, former users are removed, vendor access is approved, logging is enabled where available, and access is limited to what the user needs.

Remote access should not automatically mean access to the entire network.

The company should remove shared remote access accounts. Vendor accounts should be named, approved, time-limited where possible, and reviewed regularly.

## Step 7: Replace Unsafe Remote Desktop Exposure

Remote Desktop Protocol should not be exposed directly to the internet.

If public RDP exists, treat it as urgent. Remove it or replace it with a safer access method.

Better options include VPN with MFA, ZTNA (Zero Trust Network Access), Remote Desktop Gateway, bastion hosts, just-in-time access, controlled vendor portals, or cloud provider access brokers.

The same logic applies to public SSH, public database access, public NAS access, and exposed admin portals. If the service does not need to be public, remove it from public exposure.

## Step 8: Secure VPN Configuration

VPNs should be reviewed as high-risk systems.

Require MFA for all VPN users. Remove shared accounts. Remove former employees and old vendors. Review split tunneling. Limit VPN users to the networks and systems they actually need. Keep client software and VPN appliances updated.

VPN logs should be enabled where possible. Admin access to the VPN console should be limited and protected.

A VPN should not be treated as a trusted door that opens into everything. It should be a controlled access point.

## Step 9: Segment the Network

A flat network gives attackers more room to move.

The company should separate systems into practical zones where possible. Start with simple separation before trying to build something complicated.

**At minimum, consider separating:**

- Employee devices
- Servers
- Guest Wi-Fi
- Printers and IoT devices
- Cameras and NVRs
- Backup systems
- Admin systems
- Development or test systems
- Public-facing systems
- Finance and HR systems

Even basic separation between staff devices, guest Wi-Fi, servers, and IoT is better than one flat network where everything can reach everything else.

## Step 10: Protect Wi-Fi

Wi-Fi should be managed like a business system, not a convenience.

Use WPA2 or WPA3. Disable WPS. Separate guest Wi-Fi from business systems. Change default SSIDs and default admin passwords. Keep Wi-Fi controller firmware current. Remove old networks. Review shared Wi-Fi passwords regularly.

Guest Wi-Fi should not reach internal file shares, printers, servers, cameras, admin interfaces, or business applications.

If the company has warehouses, showrooms, branch offices, or shared office spaces, review those wireless networks too. They are often weaker than the main office network.

## Step 11: Maintain Network Devices

Firewalls, routers, switches, VPN appliances, Wi-Fi controllers, and ISP modems need maintenance.

Check default passwords, admin accounts, firmware, remote management, management network access, logging, configuration backups, end-of-life status, and vendor access.

Disable Telnet. Use SSH or HTTPS management where available. Disable UPnP where possible. Secure or disable SNMP. Restrict management interfaces to admin networks.

Network devices are often missed because they do not look like ordinary computers. Attackers know this.

## Step 12: Use Secure DNS and Web Filtering

DNS filtering helps block known malicious destinations before users connect.

Use it to block phishing domains, malware domains, command-and-control domains, and other known dangerous destinations. Where practical, apply it to office users and remote users.

This does not replace endpoint protection, email filtering, or security awareness. It is another layer.

Good options include Quad9, NextDNS, DNSFilter, Cloudflare Gateway, Pi-hole, AdGuard Home, and Technitium DNS Server.

## Step 13: Review Public IPs, Domains, and Subdomains

The company should know what it exposes to the internet.

Review public IP addresses, domain names, subdomains, DNS records, cloud public IPs, hosted systems, SSL/TLS certificates, old websites, staging systems, APIs, VPN portals, and vendor-hosted systems using the company domain.

Look for names such as: vpn.company.com, remote.company.com, admin.company.com etc.

Every public-facing service should have a business owner and technical owner. Anything unknown should be investigated.

## Step 14: Run External Exposure Checks

Perform regular checks from outside the company network.

Only scan systems the company owns or has written permission to test.

External checks should look for open ports, exposed services, public admin panels, weak TLS settings, missing security headers, risky DNS records, poor email security records, public cloud storage, public databases, forgotten subdomains, and vulnerable internet-facing systems.

Useful tools include Nmap, Greenbone Community Edition, Nuclei, Hardenize, Internet.nl, SSL Labs, Security Headers, Shodan, Censys, SecurityTrails, and cloud security tools such as Prowler, ScoutSuite, and Steampipe.

Do not wait for an attacker or search engine to find forgotten exposure first.

## Step 15: Reduce Internet-Facing Services

After exposure is identified, reduce it.

For each public service, decide whether to keep it public, restrict it, move it behind a WAF, move it behind ZTNA, limit it to trusted IP addresses, or remove it completely.

Common services to remove or restrict include public RDP, public SSH, public database access, public NAS access, public printer access, public camera access, public backup consoles, public admin panels, and forgotten test sites.

The safest exposed service is the one that does not need to be exposed.

## Step 16: Control Vendor and MSP Remote Access

Vendors and MSPs often have powerful access.

Their access should be named, approved, protected with MFA, limited to the systems they need, time-limited where possible, logged where available, and reviewed regularly.

Do not allow permanent vendor access without a named internal owner.

When a project ends, remove the access. When a vendor relationship ends, remove the access. When support access is only needed occasionally, keep it disabled until needed.

Vendor access is still company exposure.

## Step 17: Control Remote Support and RMM Tools

Remote monitoring and management tools can control many devices at once.

Review tools such as AnyDesk, TeamViewer, Splashtop, ScreenConnect, ConnectWise, RustDesk, Chrome Remote Desktop, VNC, RDP, SSH tools, and MSP RMM agents.

Only approved tools should be allowed. Admins should use MFA. Unattended access should be limited. Old agents should be removed. Vendor access should be reviewed. Session logs should be enabled where available.

If attackers compromise an RMM tool, they may compromise the device fleet.

Protect remote support tools as high-value systems.

## Step 18: Review Branch Offices and Home Offices

Small sites often have weak network controls.

Review branch offices, small warehouses, remote offices, and executive home offices where company equipment is used.

Check the router, firewall, Wi-Fi, guest network, default passwords, firmware, remote admin access, VPN, printers, cameras, and any business systems connected at the site.

Small locations are still part of the company attack surface.

## Step 19: Separate Printers, Cameras, and IoT Devices

Printers, scanners, cameras, NVRs, door systems, smart TVs, sensors, and other connected devices should not sit freely on the main business network.

Change default passwords. Keep firmware current. Remove public access. Restrict admin pages. Separate these devices onto guest, IoT, or device networks where practical.

Printers and scanners also need special attention because they may store documents, email addresses, scan destinations, and credentials.

## Step 20: Enable Network Logging and Configuration Backups

Network devices should produce useful logs and have recoverable configurations.

Enable logs for firewall activity, VPN logins, admin logins, configuration changes, IDS/IPS alerts where used, DNS activity where practical, DHCP activity, and Wi-Fi events.

Back up firewall, router, switch, VPN, and Wi-Fi controller configurations after important changes.

Store configuration backups securely. If the firewall fails or is misconfigured, the company should not need to rebuild it from memory.

## Step 21: Monitor Network Health

Network protection is also about keeping the business online.

Track internet uptime, firewall health, VPN capacity, Wi-Fi stability, switch errors, DNS availability, certificate expiry, ISP failover, and critical network links.

This is not only a security issue. If the network fails, the business may stop.

## Step 22: Create a Change Process for Network Rules

Network changes should be recorded.

Every firewall rule, VPN change, port forward, public exposure, vendor access change, DNS change, or remote support exception should have a requester, business reason, owner, approval, start date, test result, and review date.

Temporary changes should have expiration dates.

This prevents emergency changes from becoming permanent exposure.

## Step 23: Document Exceptions

Some exposure may be unavoidable for a time.

Document the system, exposure, business reason, risk, compensating control, owner, approval, and expiration date.

Compensating controls may include MFA, IP restrictions, WAF protection, segmentation, logging, time-limited access, or stronger monitoring.

An exception with no expiration date is not an exception. It is unmanaged risk.

## Step 24: Keep Evidence

Keep proof that network and remote access protections are in place.

Useful evidence includes network maps, firewall rule exports, VPN user lists, public IP lists, port scan results, DNS exports, Wi-Fi settings, device configuration backups, firmware reports, vendor access lists, RMM tool lists, segmentation notes, exception records, and review logs.

If the company cannot prove what is exposed, assume it needs review.

## Step 25: Review Regularly

Network exposure changes over time.

Review internet-facing services monthly. Review firewall rules quarterly. Review VPN users monthly or quarterly. Review vendor access quarterly and after project completion. Review Wi-Fi settings quarterly. Review network device firmware monthly or quarterly. Review public IPs, domains, subdomains, and DNS records monthly or quarterly.

Review sooner after a new office, new vendor, new firewall, new VPN, new website, new cloud system, new remote access tool, incident, or major business change.

# Places Commonly Missed

Commonly missed areas include ISP modems, old port forwards, public RDP, public SSH, public database ports, forgotten VPN users, guest Wi-Fi, printers, cameras, NVRs, old firewalls, unmanaged switches, Wi-Fi controllers, cloud security groups, DNS records, staging sites, RMM tools, remote support tools, domain registrar accounts, backup networks, home office routers, and IoT devices.

These are the places where hidden exposure often sits.

## Recommended Tools and Solutions

|Tool or Solution|Link|Type|Best Use|
|---|---|---|---|
|OPNsense|[OPNsense](https://opnsense.org/)|Open-source with paid support options|Firewall, routing, VPN, IDS/IPS, traffic control|
|pfSense CE|[pfSense](https://www.pfsense.org/)|Open-source community edition and commercial options|Firewall, routing, VPN, network security|
|OpenWrt|[OpenWrt](https://openwrt.org/)|Open-source|Router firmware for supported devices|
|VyOS|[VyOS](https://vyos.io/)|Open-source and commercial options|Routing, firewalling, VPN, network services|
|MikroTik|[MikroTik](https://mikrotik.com/)|Affordable commercial|Routers, switches, Wi-Fi, firewalling for cost-conscious teams|
|Ubiquiti UniFi|[UniFi](https://ui.com/)|Affordable commercial|Wi-Fi, switching, routing, network management|
|WireGuard|[WireGuard](https://www.wireguard.com/)|Open-source|Modern VPN tunneling|
|OpenVPN Community|[OpenVPN Community](https://openvpn.net/community/)|Open-source|VPN access for remote users and site-to-site connections|
|Tailscale|[Tailscale](https://tailscale.com/)|Free tier and commercial|Simple WireGuard-based private network and remote access|
|Headscale|[Headscale](https://github.com/juanfont/headscale)|Open-source|Self-hosted control server compatible with Tailscale clients|
|NetBird|[NetBird](https://netbird.io/)|Open-source and commercial|WireGuard-based zero trust networking and remote access|
|ZeroTier|[ZeroTier](https://www.zerotier.com/)|Free tier and commercial|Virtual networking for remote access and site connectivity|
|Cloudflare Zero Trust|[Cloudflare Zero Trust](https://www.cloudflare.com/zero-trust/)|Free tier and commercial|ZTNA, secure web gateway, access control, DNS filtering|
|Teleport|[Teleport](https://goteleport.com/)|Open-source and commercial|Secure access to SSH, Kubernetes, databases, servers, and applications|
|Apache Guacamole|[Apache Guacamole](https://guacamole.apache.org/)|Open-source|Clientless remote desktop gateway for RDP, VNC, and SSH|
|Pi-hole|[Pi-hole](https://pi-hole.net/)|Open-source|Network-level DNS filtering|
|AdGuard Home|[AdGuard Home](https://adguard.com/en/adguard-home/overview.html)|Open-source|Network-wide DNS filtering and ad/tracker blocking|
|Technitium DNS Server|[Technitium DNS Server](https://technitium.com/dns/)|Free|DNS server with blocking and DNS management features|
|Quad9|[Quad9](https://www.quad9.net/)|Free|Security-focused public DNS resolver|
|NextDNS|[NextDNS](https://nextdns.io/)|Free tier and affordable paid plans|DNS filtering for networks and remote users|
|DNSFilter|[DNSFilter](https://www.dnsfilter.com/)|Commercial|Business DNS filtering and threat blocking|
|Nmap|[Nmap](https://nmap.org/)|Open-source|Authorized port scanning and network discovery|
|Greenbone Community Edition|[Greenbone Community Edition](https://greenbone.github.io/docs/latest/)|Open-source|Vulnerability scanning for networks and systems|
|Nuclei|[Nuclei](https://github.com/projectdiscovery/nuclei)|Open-source|Template-based exposure and vulnerability checks|
|Hardenize|[Hardenize](https://www.hardenize.com/)|Free and paid options|Internet-facing domain, TLS, email, DNS, and web exposure review|
|Internet.nl|[Internet.nl](https://internet.nl/)|Free|Website, email, DNSSEC, TLS, IPv6, and standards testing|
|Shodan|[Shodan](https://www.shodan.io/)|Free and paid options|Internet exposure discovery for public IPs and services|
|Censys|[Censys](https://censys.com/)|Free and paid options|Internet asset discovery and exposure management|
|SecurityTrails|[SecurityTrails](https://securitytrails.com/)|Free and paid options|DNS history, subdomain discovery, and internet asset research|
|Suricata|[Suricata](https://suricata.io/)|Open-source|Network IDS/IPS and network security monitoring|
|Zeek|[Zeek](https://zeek.org/)|Open-source|Network security monitoring and protocol analysis|
|Security Onion|[Security Onion](https://securityonionsolutions.com/software/)|Open-source and commercial support|Network security monitoring, IDS, logs, and investigation|
|ntopng|[ntopng](https://www.ntop.org/products/traffic-analysis/ntop/)|Community and commercial options|Network traffic visibility|
|Zabbix|[Zabbix](https://www.zabbix.com/)|Open-source|Network and infrastructure monitoring|
|LibreNMS|[LibreNMS](https://www.librenms.org/)|Open-source|Network monitoring and device visibility|
|NetBox|[NetBox](https://netboxlabs.com/oss/netbox/)|Open-source|Network source of truth, IPAM, VLANs, devices, and circuits|
|Netdisco|[Netdisco](https://netdisco.org/)|Open-source|Network discovery and switch port mapping|
|Wazuh|[Wazuh](https://wazuh.com/)|Open-source|Security monitoring, configuration assessment, and log visibility|
|OpenCanary|[OpenCanary](https://opencanary.readthedocs.io/)|Open-source|Low-interaction honeypot for detecting suspicious internal activity|

## Practical Tool Stack for SMEs

#### Very small company:

Use a business-grade firewall, separated guest Wi-Fi, MFA-protected remote access, DNS filtering, and basic exposure checks with Nmap, Hardenize, Internet.nl, SSL Labs, and Security Headers.

#### Cost-conscious office network:

Use OPNsense or pfSense, UniFi or MikroTik, WireGuard or Tailscale, Pi-hole or AdGuard Home, and Zabbix or LibreNMS for monitoring.

#### Self-hosted or technical company:

Use OPNsense, WireGuard, NetBox, Greenbone, Nuclei, Suricata, Zeek, Security Onion, and Wazuh.

#### Cloud-heavy company:

Use Cloudflare Zero Trust, Tailscale or NetBird, Prowler, ScoutSuite, Steampipe, Censys, Shodan, and cloud-native security tools.

#### Multi-site company:

Use business firewalls, site-to-site VPN, centralized DNS filtering, NetBox, Zabbix, LibreNMS, and configuration backups.

#### Higher-risk environment:

Use ZTNA, MFA everywhere, stronger segmentation, IDS/IPS, Security Onion, Suricata, Zeek, external exposure monitoring, and tighter vendor access controls.

# Network Protection Register Template

**The company should maintain a simple register with these fields:**

- Network asset
- Owner
- Location
- Public exposure
- Public IP or domain
- Open ports
- Admin access
- MFA status
- Firmware or version
- Logging status
- Configuration backup status
- Network zone or VLAN
- Main risk
- Exception status
- Last review date
- Next action

## Expected Outputs from This Section

**At the end of this section, the company should have:**

- A named owner for network, remote access, and internet exposure protection.
- A network and exposure register.
- A simple network map.
- Reviewed firewall rules.
- Removed or restricted unsafe inbound access.
- Protected network management interfaces.
- Secure VPN or ZTNA remote access.
- No direct public RDP exposure.
- MFA on remote access.
- Network segmentation.
- Separated guest Wi-Fi.
- Secured network devices.
- DNS filtering where appropriate.
- A list of public IPs, domains, and subdomains.
- External exposure scan results.
- Reduced public-facing services.
- Controlled vendor and MSP remote access.
- Controlled RMM and remote support tools.
- Remote office network checks.
- IoT and printer network controls.
- Network logging enabled.
- Configuration backups stored.
- A network change process.
- An exception register.
- Evidence folder.
- Regular review schedule.

## Objectives

Do not leave the network as a mystery.

The company should know what is connected, what is exposed, who can connect remotely, who manages the equipment, and which services are reachable from the internet.

A company should leave this section able to say:

“We know our public exposure. We know our firewall rules. We know our remote access paths. We know our network zones. We know our vendor access. We know which services must be public and which should be removed.”

That is network, remote access, and internet exposure protection.


---
