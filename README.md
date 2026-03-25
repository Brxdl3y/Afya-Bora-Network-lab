**Afya Bora Clinic Network** 

 **Overview**

The **Afya Bora Clinic Network** is a simulated enterprise-grade network built in Cisco Packet Tracer to demonstrate **design, configuration, and troubleshooting skills** at both Layer 2 and Layer 3. It reflects real-world scenarios such as healthcare operations that require **high availability, secure access, and seamless interconnectivity** between departments.

This topology integrates:

🔷**VLAN segmentation** for different clinic departments.

🔷**Inter-VLAN Routing** using both **ROAS** (Router-on-a-Stick) and **SVIs** (Switch Virtual Interfaces).

**Dynamic routing** with OSPF for internal and upstream ISP communication.

**MD5 authentication** for routing protocol security.

**Subnetting strategy** (/26 subnets per department) for efficiency and scalability.

🔷**ACLs** to enforce traffic restrictions between sensitive areas (e.g., restricting Pharmacy from accessing Lab results directly).

🔷**DHCP services** for automatic IP allocation.

**NAT/PAT** for secure Internet access through the ISP router.

**Redundancy** & Failover simulation using FHRP **(HSRP/GLBP concepts)**.

🔷Secure device management **(SSH, strong passwords, MOTD banners)**.


This project not only solves basic connectivity but also demonstrates enterprise-class best practices in **security, redundancy, and scalability**.


**Goals & What this demonstrates** 

**Solid network design fundamentals**: VLAN separation per functional area, SVI inter-VLAN routing on the L3 switch, and clean IP addressing/subnetting.

**Resilience & availability**: HSRP and clear interface descriptions to support troubleshooting and handoffs.

**Security-first mindset**: Management-plane protection (SSH, ACLs), port-security on access ports, ACLs for inter-VLAN access control, and OSPF MD5 authentication on routing adjacencies.

**Operational excellence**: NTP, logging, SNMP read-only for monitoring, interface descriptions, and sample verification commands — all show that you design for operations, not just connectivity.

**Advanced but practical features**: QoS for voice/data segregation, NAT for Internet access, EtherChannel basics, and optional NetFlow templates for traffic analysis.


 **Department VLAN & Subnet Plan**


Department	VLAN ID	Subnet	Gateway

**Reception**	20	10.0.0.64/26	10.0.0.65

**Consultation Room**	10	10.0.0.0/26	10.0.0.252

**Pharmacy**	10	10.0.1.0/26	10.0.0.252

**Emergency Room**	30	10.0.0.128/26	10.0.0.254

**X-Ray** 0	10.0.0.192/26	10.0.0.254

**Laboratory**	10	10.0.3.0/26	10.0.0.252


 **Security Enhancements**

SSH access only (Telnet disabled).

AAA local authentication with encrypted passwords.

Port security on access ports (sticky MACs, violation shutdown).

ACLs to control inter-department communication.

OSPF MD5 authentication to prevent rogue routing updates. 


It’s designed to show that I can handle both **small-scale clinics and enterprise-level networks** with equal sophistication.

AUTHOR: **Bradley Giovanni**  | **CCNA Enthusiast  |  Network Eng  | Network Admin**

EMAIL: **giovanniibradley@gmail.com**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/bradley-giovanniii293)
