---
icon: triangle-right
order: -10
---
### Goals


**Identify how business processes, applications, services, data, users, assets, vendors, cloud resources, network paths, and third-party providers depend on each other, so the company understands what breaks when one component fails, changes, is compromised, or becomes unavailable.**

This section connects the previous inventories. It is not just a vendor list, and it is not itself the risk assessment but is the supporting documentation for it as the relationship map underneath the cybersecurity playbook. 

### Task:

- Map the relationships between systems, users, data, vendors, cloud services, integrations, and business processes. 
- This shows what breaks if a key system, supplier, account, or service becomes unavailable or compromised.


## Main Steps in the Identify Dependencies Process


Create a clear map of what each critical business function, application, data set, user group, and vendor depends on, so the company understands what could break operations if one component fails or changes.

The point is not to document every minor relationship but rather to identify the dependencies that matter.

## 1. Define the critical business functions first

Start with the business activities that must keep running.

**Examples:**

- Order processing  
- Customer support  
- Payroll  
- Finance and payments  
- Sales operations  
- Website/e-commerce  
- Production or service delivery  
- Email and communications  
- Backup and recovery  
- Compliance reporting

Answer the key question: **What business functions would cause serious disruption if they stopped working?**

This prevents the team from wasting time mapping low-value dependencies.

## 2. Map the systems, data, people, and vendors each function relies on

For each critical business function, identify the required components.

**Capture:**

- Applications and services  
- Data sources  
- User groups or roles  
- Devices or infrastructure  
- Cloud services  
- Vendors or third parties  
- Network/internet requirements  
- Identity/login requirements  
- Backup or recovery requirements

**Example:**

**Payroll depends on:** HR system, payroll provider, bank portal, finance approver, employee records, MFA, email, internet access, and payroll backup records.

Answer the key question: **What must be available for this function to work?**

## 3. Link dependencies back to owners and existing inventories

Each dependency should connect back to an existing record where possible.

**Link it to:**

- Application/service inventory  
- Asset inventory  
- Data inventory  
- User/account inventory  
- Vendor list  
- Cloud resource list  
- Network records  
- Backup records

**Each dependency should have:**

- Business owner  
- Technical owner  
- Vendor/contact owner, if external  
- System or data owner  
- Last validated date

Answer the key question: **Who owns this dependency, and where is the authoritative record for it?**

This is the step that stops the dependency map from becoming random notes.

## 4. Flag critical gaps and single points of failure

Now identify the relationships that need attention later during Assess, Protect, Respond, or Recover.

**Flag:**

- No owner  
- No documented workaround  
- One vendor supports multiple critical functions  
- One identity provider controls access to everything  
- One internet link supports the whole office  
- One cloud region hosts all production systems  
- One backup service supports all recovery  
- One admin or service account controls a critical system  
- One spreadsheet or manual process supports a major workflow  
- Unknown or unvalidated dependency

Answer the key question: **Which dependencies would create serious disruption if they failed?**

## 5. Validate and maintain the dependency map

Review the dependency map with business owners, IT, finance, operations, and vendor managers.

**Ask:**

- Is this dependency real?  
- Is it still active?  
- Who owns it?  
- What breaks if it fails?  
- Is there a workaround?  
- Is the vendor/contact information current?  
- Has anything changed since the last review?

**Update the map when:**

- A new application is introduced  
- A vendor is added or removed  
- A business process changes  
- A new integration is created  
- A cloud resource is added  
- A critical account or service account changes  
- DNS, domain, certificate, backup, or identity systems change  
- A system is retired

**Recommended process:**

- Quarterly review for critical dependencies.  
- Annual review for the full dependency map.  
- Immediate update after major system, vendor, or process changes.

Answer the key question: **Is the dependency map still accurate enough to support decisions?**


## Recommended open-source or affordable tools

|Tool|Best use|Why it fits|Watch-out|
|---|---|---|---|
|[GLPI](https://www.glpi-project.org/en/cmdb-software/)|Lightweight CMDB, assets, relationships, impact view|Useful as a central system of record for assets, software, services, tickets, ownership, and relationship tracking. GLPI also has impact/relationship management features for visualizing relationships between assets.|Good for SMEs, but only works if the data model is kept clean.|
|[iTop](https://www.itophub.io/)|CMDB, service catalog, relationship mapping|iTop is open source and designed to manage configuration items and their relationships in a flexible CMDB.|Better for dependency mapping than a simple spreadsheet, but requires disciplined configuration.|
|[CMDBuild](https://www.cmdbuild.org/en/homepage)|Custom CMDB and workflow-driven dependency management|CMDBuild is open source and lets organizations configure custom asset-management applications, workflows, reports, dashboards, and connectors.|Powerful but heavy. Bad fit if no one can administer the model.|
|[NetBox](https://netboxlabs.com/products/netbox/)|Network, infrastructure, IPAM, DCIM source of truth|Strong for mapping network/infrastructure dependencies: sites, racks, devices, IP addresses, VLANs, circuits, virtual assets, and network topology.|Excellent infrastructure source of truth; not a full business-process dependency tool.|
|[Backstage](https://backstage.io/docs/features/software-catalog/)|Internal software and service catalog|Tracks ownership and metadata for software components such as services, websites, libraries, and data pipelines. Its catalog supports entity relationships.|Best for development teams. Overkill for a purely non-technical SME.|
|[OpenMetadata](https://open-metadata.org/)|Data catalog, data ownership, lineage, governance|Useful for mapping data dependencies and ownership across databases, dashboards, pipelines, and other data assets.|Data-focused. Not a general CMDB.|
|[DataHub](https://datahub.com/)|Data catalog and lineage|Useful for mapping where data originates, how it transforms, and where it is consumed.|More suitable for data teams than small companies with only shared drives.|
|[CloudQuery](https://www.cloudquery.io/docs/platform/features/asset-inventory)|Cloud asset and cloud dependency inventory|Provides unified inventory of cloud resources across connected integrations, including AWS, GCP, Azure, and other synced providers.|Cloud-focused. Needs someone comfortable with data queries and cloud metadata.|
|[Steampipe](https://steampipe.io/)|SQL queries across cloud, SaaS, code, logs, and APIs|Useful for querying infrastructure and service metadata directly.|Query layer, not a polished management workflow.|
|[LibreNMS](https://www.librenms.org/)|Network discovery and monitoring|Can automatically discover network devices using protocols such as CDP, FDP, LLDP, OSPF, BGP, SNMP, and ARP.|Good for network visibility; not a business dependency register.|
|[Zabbix](https://www.zabbix.com/)|Monitoring, discovery, trigger dependencies|Zabbix supports network discovery rules and trigger dependencies, which can help model operational monitoring dependencies.|Monitoring logic is not the same as a management dependency map.|
|[Uptime Kuma](https://github.com/louislam/uptime-kuma)|Simple self-hosted service availability list|Good low-friction tool for maintaining a list of important endpoints and uptime checks.|Better for service visibility than full dependency modeling.|
|[Nmap](https://nmap.org/)|Network discovery and service enumeration|Free and open-source utility for network discovery, inventory support, service checks, and security auditing.|Use carefully and only with authorization. It finds services; it does not explain business dependencies.|
|[Portainer CE](https://github.com/portainer/portainer)|Container and orchestration visibility|Portainer Community Edition manages Docker, Swarm, Kubernetes, ACI environments, containers, images, volumes, and networks.|Useful for container dependencies, not SaaS or vendor mapping.|
|[OWASP Dependency-Track](https://owasp.org/www-project-dependency-track/)|Software supply chain and SBOM dependency tracking|Dependency-Track is an OWASP component-analysis platform that uses SBOMs to help identify and reduce software supply-chain risk.|This is for software components and libraries, not business-process dependencies.|
|[Dependency-Track project site](https://dependencytrack.org/)|SBOM-based component dependency management|Useful for tracking application component dependencies and transitive software supply-chain relationships.|Requires SBOM generation and development workflow integration.|
|[diagrams.net](https://www.diagrams.net/)|Manual dependency diagrams|Good free/low-cost option for drawing business process maps, system maps, and dependency diagrams.|Manual diagrams go stale unless tied to a review process.|
|[Mermaid](https://mermaid.js.org/)|Text-based dependency diagrams|Useful for version-controlled diagrams in Markdown, Git, or documentation systems.|Requires comfort with text syntax; not a database of record.|
|[Neo4j Community Edition](https://neo4j.com/deployment-center/)|Graph database for complex dependency relationships|Useful when relationships matter more than tables, such as “what depends on this service?” or “what breaks if this vendor fails?”|Powerful, but likely excessive for most SMEs unless they have technical staff.|

## Practical stack recommendations

#### For a small non-technical SME, use:

- **Spreadsheet or GLPI + diagrams.net + Uptime Kuma + vendor contract list.**

This is enough to start. The mistake would be pretending the business needs a complex CMDB before it can even name its critical dependencies.

#### For a normal SME with basic IT capability, use:

- **GLPI or iTop + LibreNMS or Zabbix + Uptime Kuma + NetBox for network/IP records.**

GLPI or iTop becomes the dependency register. LibreNMS/Zabbix helps discover and monitor infrastructure. NetBox keeps network truth clean.

#### For a cloud-heavy SME, use:

- **CloudQuery + Steampipe + GLPI/iTop + provider-native exports.**

CloudQuery gives inventory. Steampipe gives query power. GLPI/iTop stores ownership, business process mapping, and review status.

#### For a software-development company, use:

- **Backstage + OWASP Dependency-Track + DataHub/OpenMetadata + CloudQuery.**

Backstage maps internal services and ownership. Dependency-Track maps software component dependencies. DataHub/OpenMetadata maps data lineage. CloudQuery maps cloud resources.

#### For an infrastructure-heavy company, use:

- **NetBox + LibreNMS/Zabbix + GLPI/iTop.**

NetBox owns infrastructure truth. LibreNMS/Zabbix discovers and monitors. GLPI/iTop links infrastructure to business services, owners, vendors, and impact.

#### For a more mature organization, use:

- **iTop or CMDBuild + NetBox + CloudQuery + DataHub/OpenMetadata + Dependency-Track + graph visualization.**

This is the fuller model. It is also easy to overbuild. The rule should be: do not deploy more tooling than the organization can maintain.

## Suggested dependency inventory fields

**Use these fields in the playbook or spreadsheet:**

- Dependency ID  
- Source item  
- Source type  
- Dependent item  
- Dependent type  
- Dependency direction  
- Dependency category  
- Description  
- Business process supported  
- Application/service involved  
- Asset involved  
- Data involved  
- User/account dependency  
- Vendor/provider involved  
- Cloud provider/account/project  
- Network dependency  
- Identity dependency  
- Backup dependency  
- Criticality  
- Failure impact summary  
- Workaround available  
- Business owner  
- Technical owner  
- Vendor contact  
- Contract/SLA reference  
- Review frequency  
- Last validated date  
- Next review date  
- Status  
- Notes

**For vendor dependencies, add:**

- Vendor name  
- Service provided  
- Internal owner  
- Data handled  
- Systems supported  
- Business process supported  
- Contract owner  
- Renewal date  
- Support contact  
- SLA/response terms  
- Exit or replacement option  
- Last vendor review date

**For technical dependencies, add:**

- Protocol/API  
- Port/service  
- Integration method  
- Authentication method  
- Service account/API key  
- Certificate dependency  
- DNS dependency  
- Environment: production, staging, development  
- Monitoring link  
- Backup/recovery link


## Suggested minimum fields

- Dependency ID  
- Business function  
- Dependency name  
- Dependency type  
- Application/service involved  
- Data involved  
- Vendor involved  
- User/account dependency  
- Asset/cloud/network dependency  
- Business owner  
- Technical owner  
- Criticality  
- Failure impact summary  
- Workaround available  
- Authoritative inventory link/reference  
- Last reviewed date  
- Status


## Useful dependency queries/views

**Your spreadsheet or CMDB should support these views:**

- Critical dependencies with no owner  
- Business processes with no mapped backup dependency  
- Applications depending on one vendor  
- Applications depending on one identity provider  
- Applications with sensitive data and external integrations  
- Cloud resources with no linked application or owner  
- Service accounts linked to unknown applications  
- Vendors supporting critical systems  
- Upcoming vendor, certificate, domain, or license renewals  
- Internet-facing services with unclear dependencies  
- Applications with no documented workaround  
- Dependencies not reviewed in the last 90 or 180 days  
- Retired systems still appearing as dependencies  
- Manual spreadsheet or email-based dependencies supporting critical work



## Summary of the Steps

**Identify Dependencies Process**

1. **Define critical business functions** that must keep operating.
    
2. **Map required systems, data, users, vendors, cloud resources, network paths, and identity services** for each function.
    
3. **Connect each dependency to an owner and existing inventory record** where possible.
    
4. **Flag single points of failure, unknown dependencies, ownerless dependencies, and missing workarounds.**
    
5. **Validate and maintain the dependency map** through owner review and change triggers.
    


## Summary

**The Identify Dependencies step maps the most important relationships between business functions, applications, data, users, assets, vendors, cloud resources, and infrastructure. The purpose is to understand what each critical function depends on, who owns those dependencies, and which relationships could create disruption if they fail.**

---

