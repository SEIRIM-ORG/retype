---
icon: chevron-right
order: 100
---
![[x 483 Header 100 Point QA Checklist 1.jpg]]

## Identify Goals

The goal of the **Identify** stage is to create a clear, accurate map of the company’s digital environment so your business knows exactly what must be protected, who can access it, where critical data lives, and what systems or vendors the company depends on.

#### Identify turns cybersecurity from guesswork into visibility

The objective is not to judge risk or design controls. That belongs more to **Assess** and **Protect**. The objective here is to build the factual inventory that all other cybersecurity decisions depend on.


## The main objectives are:

#### 1. Know what assets exist

**Task:**

- Create an accurate inventory of devices, servers, cloud resources, network equipment, and other technology assets. 
- The company should know what it owns, what it uses, where each asset is located, who is responsible for it, and whether it is still active.

#### 2. Know what data exists and where it lives

**Task:**

- Identify business-critical, sensitive, confidential, regulated, and operational data. 
- The company should understand where data is stored, how it moves, who uses it, and which data would cause serious harm if lost, stolen, leaked, or corrupted.

#### 3. Know which applications and services support the business

**Task:**

- List the software, SaaS tools, platforms, databases, websites, APIs, and cloud services the company relies on. 
- This helps expose shadow IT, forgotten systems, duplicate tools, and business-critical platforms that may not be formally tracked.

#### 4. Know who and what has access

**Task:**

- Identify users, administrators, contractors, service accounts, shared accounts, vendor accounts, API keys, and automation identities. 
- The aim is to understand every access point into the environment, especially privileged or unmanaged access.

#### 5. Know the dependencies and connections

**Task:**

- Map the relationships between systems, users, data, vendors, cloud services, integrations, and business processes. 
- This shows what breaks if a key system, supplier, account, or service becomes unavailable or compromised.



### Summary

The Identify stage establishes complete visibility over the organization’s technology environment by documenting its assets, data, applications, services, users, accounts, and operational dependencies. Its purpose is to create the factual foundation needed for risk assessment, protection, detection, response, and recovery.

**Goal:**  
Build a reliable inventory and dependency map of the company’s digital environment.

**Objectives:**  
Identify what the company owns, what data it handles, what systems it uses, who has access, and what internal or external dependencies keep the business running.

If this stage is weak, the rest of the playbook is built on incomplete knowledge and assumptions. You cannot secure assets you do not know exist, protect data you have not located, remove access you have not identified, or recover systems whose dependencies you never mapped.


## 1. Identify Assets

This covers the physical and virtual things the company owns or uses.

Include:

Physical devices, laptops, desktops, servers, mobile devices, printers, routers, switches, firewalls, IoT devices, cloud infrastructure, virtual machines, and storage systems.

Core question:

**What technology assets exist, where are they, who owns them, and are they still in use?**

This is the foundation. If the company does not know what exists, it cannot protect it properly.

## 2. Identify Data

This covers the information the business creates, stores, processes, or shares.

Include:

Customer data, employee data, financial records, contracts, intellectual property, credentials, business documents, backups, regulated data, confidential files, and archived data.

Core question:

**What data do we have, where is it stored, how sensitive is it, and who can access it?**

This should include basic data classification: public, internal, confidential, restricted, or regulated.

## 3. Identify Applications and Services

This covers the software, systems, platforms, and cloud services the company depends on.

Include:

Business applications, SaaS tools, email platforms, accounting systems, CRM systems, ERP systems, websites, APIs, databases, cloud services, backup platforms, security tools, and third-party portals.

Core question:

**What applications and services are used to run the business, and what role does each one play?**

This is where shadow IT often appears. SMEs usually underestimate how many tools employees actually use.

## 4. Identify Accounts and Users

This covers human and non-human access identities.

Include:

Employees, contractors, administrators, shared accounts, service accounts, privileged accounts, API keys, automation accounts, vendor accounts, dormant accounts, and former employee accounts.

Core question:

**Who or what has access to company systems, what level of access do they have, and is that access still justified?**

This deserves its own category because compromised accounts are one of the most common ways attackers get in. Do not bury this under “assets.”

## 5. Identify Dependencies and Connections

This maps how everything depends on everything else.

Include:

Vendor dependencies, cloud dependencies, internet-facing systems, network connections, integrations, APIs, payment processors, email dependencies, supply chain links, managed service providers, outsourced IT, and critical business process dependencies.

Core question:

**What systems, vendors, data flows, and services does the business rely on to operate?**

This is the category that turns a flat inventory into a useful cybersecurity map. Without dependency mapping, the inventory is just a list.