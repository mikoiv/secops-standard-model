# Security operations standard model

The model describes capabilities that build a complete SecOps service for an organization. 

![Image](secops_standard_model_capabilities.png)

The capabilities are aligned with NIST Cybersecurity Framework functions. This is a relatively loose alignment, the main reasoning for using CSF here is to make the everything easier to group and visualize.

# 1. Identification capabilities

## 1.1. Attack surface management

Goals: understand your assets and create a continuously updating visibility to all high-risk systems

MVP:
* Start with assets available to the public or to partners. 
* Document your assets: domains, IP addresses, service addresses.
* Document your attack vectors: internet-connections, DMZs, partner site-to-site connections, VPNs.
* Start monitoring: scan for new or changed assets, scan for open ports and services, scan for vulnerabilities.

Next steps:
* Evaluate commercial attack surface management services if you want. 

# 2. Protection capabilities

## Security policy management

Goals: create security policies that define guardrails for your entire IT environment:
* Identity risk policies, including conditional access
* Application allow- and denylisting
* Platform resource type allow- and denylisting
* Network firewall policies, UTM policies, ACLs

MVP:

# 3. Detection capabilities

# 4. Response capabilities

# Licensing

Attribution-NoDerivs CC BY-ND

This license lets others reuse the work for any purpose, including commercially; however, it cannot be shared with others in adapted form, and credit must be provided to me.

https://creativecommons.org/licenses/by-nd/4.0/
