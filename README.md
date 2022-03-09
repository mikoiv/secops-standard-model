# Security operations standard model

The model describes capabilities that build a complete SecOps service for an organization. 

![Image](secops_standard_model_capabilities.png)

The capabilities are aligned with NIST Cybersecurity Framework functions. This is a relatively loose alignment, the main reasoning for using CSF here is to make the everything easier to group and visualize.

# 0. Supporting functions

# 1. Identification capabilities

## 1.1. Attack surface management

Goal: 
* Understand your assets and create a continuously updating visibility to all high-risk systems

MVP:
* Start with assets available to the public or to partners. 
* Document your assets: domains, IP addresses, service addresses.
* Document your attack vectors: internet-connections, DMZs, partner site-to-site connections, VPNs.
* Start monitoring: scan for new or changed assets, scan for open ports and services, scan for vulnerabilities.

Next steps:
* Evaluate commercial attack surface management services if you want. 

## 1.2. Vulnerability management

Goal:
* Identify and fix vulnerabilities in your assets. 

MVP:
* Sign-in for vulnerability bulletins relevant to your assets and systems.
* Build some technical reporting capability for vulnerabilities, either from an assessment or scanning tool or at minimum based on patch-level reporting.
* Ensure your vulnerability reporting cover your critical applications, infrastructure systems and end-user environment.
* Focusing on internet-visible assets is not enough, as internal systems may also be vulnerable via several vectors such as e-mail.
* If you have a formal change management process, ensure it enables you to do quick vulnerability fixing (via emergency changes, standard changes or other method).

Next steps:
* Evaluate commercial vulnerability assessment tools.

## 1.3. Threat intelligence

Goal:
* Have the capability to recieve threat indicators and find out if you are affected.

MVP:
* Understand which of your existing security tools contain external indicators for threats, such as IPS.
* Know how to create custom indicators in your security toolkit, in case you one day need to do this. 

Next steps:
* Evaluate if you would benefit from an automated threat intelligence platform. 

## 1.4. Testing

## 1.5. Disclosure

Goal: 
* Be prepared to receive vulnerability disclosures.

MVP:
* Discuss internally how you would react to a disclosure contact. 
* Look into security.txt https://securitytxt.org

# 2. Protection capabilities

## 2.1. Security policy management

Goal: 
* Create and manage security policies that define guardrails for your entire IT environment.

MVP:
* Identity risk policies, including conditional access.
* Infrastructure platform resource allowlisting and denylisting.
* Network firewall policies, UTM policies, ACLs.

Next steps:
* Application allowlisting and denylisting for workstations and servers.

## 2.2 Patch management

## 2.3 Threat protection

## 2.4 Data protection

# 3. Detection capabilities

## 3.1. Use case development

Use Case development is the capability to identify what threats needs to be monitored and how are detection and response done. 

Example Use Case lifecycle:
1. Define threat scenario.
2. Define alerting, detection and response process. 
3. Write new playbook if necessary. 
4. Test alerting and detection accuracy. 
5. Deploy the use case.
6. Evaluate and refine.

Example Use Case onboarding maturity model:

* Stage 1: Use cases with low false positive rates, low complexity, repeatable response activities.
* Stage 2: Use cases with medium false positive rate, analysis and decision-making usually required during response activities.
* Stage 3: Use cases with high false positive rates, baselining and customisation needed before onboarding, detailed analysis capabilities needed during response activities.

## 3.1. Data collection

* The Data Collection capability covers identification, collection and lifecycle management for security data.
* Data collection practices:
    * Define data sources
    * Define data collection patterns
    * Define data collection toolkit
    * Define enrichment patterns
    * Define data lifecycle

* Common data sources:
    * Email transport & mail protection systems 
    * Endpoint protection, antivirus systems
    * Collaboration systems
    * Identity & access management systems
    * Vulnerability scanners 
    * Attack surface management systems
    * Linux OS logs   
    * Windows OS logs (Event logs, Sysmon)
    * Web server, App server logs 
    * Application whitelisting systems
    * CASB 
    * DNS
    * DHCP
    * Data islands / Snowflake systems 
    * Jump boxes / Bastion hosts
    * VPN gateways 
    * Application Delivery systems
    * Network connections / flows
    * Database logs 
    * Firewalls, IDS/IPS systems
    * Proxy systems 
    * Web Application Firewalls
    * DDoS protection systems / scrubbers 
    * DLP systems

## 3.1. Security analytics

* The capability covers monitoring, analysis and threat detection based on collected security data. 
* Traditionally the core technical component of analytics is Security Information and Event Management (SIEM) tools.
* Security Orchestration, Automation, and Response (SOAR) platforms are linked to analytics but the core SOAR functionality is in Incident Response.

## 3.1. Threat hunting

## 3.1. Incident detection

* The Incident Detection capability ensures security findings are processed in a way that enables the detection of security incidents that need response activities.
* Incidents can be detected via
    * Automation (Use Case development + Security Analytics combined)
    * Manual input from security operations (Threat hunting)
    * Manual input from IT operations (Service desk, IT ops teams etc)
    * Manual input from external parties (Vendors, contractors etc)

# 4. Response capabilities

## 4.1. Incident response

* Incident Response is the capability to ingest events from Incident Detection and make sure analysis, response and recovery activities are done in a timely manner, even with large volumes or complex threats.

* Keys to operational efficiency in incident response:
    * Current trends and community knowledge advocate to avoid tiers.
    * If you must have tiers, make sure there are no process silos and blockers when moving incidents between tiers.
    * Ensure response team availability and resourcing. 
    * Understand the IT and business environment, organisational culture, processes, ongoing transformation projects.
    * Continuous communication with stakeholders, whether internal teams or external parties.

* Define the following
    * Response process
    * Playbooks
    * Common toolkit

## 4.2. Forensic analysis 

MVP:
* Know who you can contact if you need forensic work.

## 4.3. Incident reporting



# Licensing

Attribution-NoDerivs CC BY-ND

This license lets others reuse the work for any purpose, including commercially; however, it cannot be shared with others in adapted form, and credit must be provided to me.

https://creativecommons.org/licenses/by-nd/4.0/
