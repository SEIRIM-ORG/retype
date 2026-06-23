
In **CIS RAM**, the difference is mainly about **how much risk-assessment structure and CIS Controls maturity the organization is ready for**.

The blunt version: **Core explains the method. IG1, IG2, and IG3 apply the method at increasing levels of organizational maturity, control coverage, technical capability, and threat exposure.**

CIS currently lists the CIS RAM v2.2 family as including **CIS RAM Core**, plus separate CIS RAM versions and companion workbooks for **Implementation Group 1, Implementation Group 2, and Implementation Group 3**. [CIS RAM](https://www.cisecurity.org/insights/white-papers/cis-ram-risk-assessment-method) describes the method as helping organizations assess risk against the CIS Critical Security Controls. ([CIS](https://www.cisecurity.org/insights/white-papers/cis-ram-risk-assessment-method "CIS RAM (Risk Assessment Method)"))

## 1. CIS RAM Core

**CIS RAM Core** is the foundation. It gives the basic principles and practices of the CIS Risk Assessment Method without tailoring the process to a specific CIS Implementation Group.

Use Core when you want to understand the method itself: how CIS RAM thinks about reasonable security, acceptable risk, impact, expectancy, safeguards, and risk treatment.

It is best for:

Understanding CIS RAM before applying the workbook  
Training internal risk owners  
Building your own customized assessment process  
Explaining the method to executives, auditors, or consultants  
Creating a risk-assessment process that is not strictly limited to IG1, IG2, or IG3

CIS describes Core in earlier CIS RAM material as the “bare essentials” version of CIS RAM, while the IG-specific documents add examples, templates, exercises, workbooks, and deeper guidance for each Implementation Group. ([CIS](https://www.cisecurity.org/insights/blog/cis-risk-assessment-method-ram-v2-1-for-cis-controls-v8 "CIS Risk Assessment Method (RAM) v2.1 for CIS Controls v8"))

**Playbook interpretation:** Core is the methodology layer. It tells you how to think.

## 2. CIS RAM for IG1

**IG1** is the entry-level version. It is aligned to [CIS Implementation Group 1](https://www.cisecurity.org/controls/implementation-groups/ig1), which CIS defines as **essential cyber hygiene**. IG1 includes **56 foundational Safeguards** that every enterprise should apply to defend against common attacks. ([CIS](https://www.cisecurity.org/controls/implementation-groups/ig1 "CIS Critical Security Controls Implementation Group 1"))

IG1 is intended for organizations that are usually small to medium-sized, have limited IT and cybersecurity expertise, and mainly need to keep the business operational. CIS says IG1 safeguards are intended to be implementable with limited cybersecurity expertise and aimed at general, non-targeted attacks. ([CIS](https://www.cisecurity.org/controls/implementation-groups/ig1 "CIS Critical Security Controls Implementation Group 1"))

Use IG1 when the company:

Has no mature risk register  
Has limited cybersecurity staff  
Has limited technical tooling  
Needs basic but defensible cyber hygiene  
Mainly faces common threats like phishing, malware, credential theft, and basic ransomware  
Needs a simple risk-assessment process that does not overwhelm the team

**Playbook interpretation:** IG1 is the SME baseline. It is the right starting point for most small businesses.

## 3. CIS RAM for IG2

**IG2** builds on IG1. It is aligned to [CIS Implementation Group 2](https://www.cisecurity.org/controls/implementation-groups/ig2), which adds **74 additional Safeguards** on top of IG1’s 56. CIS describes IG2 as suitable for organizations with increased operational complexity, enterprise-grade technology, specialized expertise, multiple departments with different risk profiles, and sensitive client or enterprise information. ([CIS](https://www.cisecurity.org/controls/implementation-groups/ig2 "CIS Controls Implementation Group 2"))

CIS RAM for IG2 is more structured than IG1. It is designed for organizations that can assess separate asset classes rather than treating the enterprise as one generic unit. CIS material on CIS RAM for IG2 says it combines qualitative and quantitative analysis and helps automate parts of threat modeling and risk estimation. ([CIS](https://www.cisecurity.org/insights/blog/cis-risk-assessment-method-ram-v2-1-for-implementation-group-2-ig2 "CIS Risk Assessment Method (RAM) v2.1 ..."))

Use IG2 when the company:

Has dedicated IT staff  
Has multiple departments or business units  
Uses more complex infrastructure  
Stores sensitive customer, employee, or business data  
Has regulatory or contractual obligations  
Can perform more detailed control maturity reviews  
Needs to assess risk by asset class, not only at the organization-wide level

**Playbook interpretation:** IG2 is for a growing SME or mid-market company where “basic hygiene” is no longer enough.

## 4. CIS RAM for IG3

**IG3** is the most advanced version. It is aligned to [CIS Implementation Group 3](https://www.cisecurity.org/controls/implementation-groups/ig3), which adds **23 more Safeguards** after IG1 and IG2, reaching the full set of **153 Safeguards** in CIS Controls v8/v8.1. ([CIS](https://www.cisecurity.org/controls/implementation-groups/ig3 "CIS Controls Implementation Group 3"))

CIS describes IG3 organizations as commonly employing security experts across areas like risk management, penetration testing, and application security. IG3 environments often involve sensitive information, regulated functions, public welfare concerns, targeted attacks, and potential zero-day exposure. ([CIS](https://www.cisecurity.org/controls/implementation-groups/ig3 "CIS Controls Implementation Group 3"))

Use IG3 when the company:

Has mature security personnel  
Faces targeted attacks  
Handles highly sensitive data  
Operates critical services  
Has strict regulatory or compliance oversight  
Needs advanced security engineering  
Can analyze attack paths and sophisticated threat models  
Needs to reduce the impact of advanced attacks, including zero-days

**Playbook interpretation:** IG3 is not for a normal small business. If an SME tries to start here, it will probably waste time, create paperwork, and fail execution.

## Practical comparison

|CIS RAM Type|What it is|Best for|Control depth|Risk-assessment maturity|
|---|---|---|---|---|
|[CIS RAM Core](https://www.cisecurity.org/insights/white-papers/cis-ram-risk-assessment-method)|Base methodology|Learning and customizing CIS RAM|Not tied to one IG|Foundational|
|[IG1](https://www.cisecurity.org/controls/implementation-groups/ig1)|Essential cyber hygiene|Small/medium organizations with limited security resources|56 Safeguards|Basic, practical, starter-level|
|[IG2](https://www.cisecurity.org/controls/implementation-groups/ig2)|Expanded protection|Organizations with dedicated IT, sensitive data, multiple departments|IG1 + 74 additional Safeguards|Intermediate, more structured|
|[IG3](https://www.cisecurity.org/controls/implementation-groups/ig3)|Advanced protection|Mature, regulated, high-risk, targeted organizations|IG1 + IG2 + 23 additional Safeguards = 153 total|Advanced, threat-driven, attack-path oriented|

## Which one should an SME use?

For your cybersecurity playbook, the recommendation should be:

**Start with CIS RAM Core to understand the method, then use CIS RAM for IG1 as the default SME risk-assessment pathway. Move to IG2 only when the company has dedicated IT/security capability, sensitive data, regulatory pressure, or multiple business units with different risk profiles. Reserve IG3 for mature, high-risk, regulated, or targeted organizations.**

The weak recommendation would be: “Use CIS RAM.”

The stronger recommendation is: **Use CIS RAM Core as the conceptual method, IG1 as the SME operating baseline, IG2 as the growth-stage path, and IG3 only when the organization’s risk profile justifies advanced security capability.**