
# CCNA Project 03 - Enterprise ACL Security

## Project Overview

This project demonstrates the implementation of **Extended Access Control Lists (ACLs)** in an enterprise network using Cisco Packet Tracer. The objective is to secure communication between departments by applying access control policies while maintaining normal network operations.

The network consists of three departments connected through a Cisco router and Cisco switches. VLANs are used to separate departments, Router-on-a-Stick enables inter-VLAN routing, DHCP provides automatic IP address assignment, and Extended ACLs enforce the organization's security policy.

---

## Network Topology

* Cisco Router 2911
* Cisco Switch 2960 (SW1)
* Cisco Switch 2960 (SW2)
* VLAN 10 - HR Department
* VLAN 20 - Finance Department
* VLAN 30 - IT Department
* DHCP Server configured on Router
* Router-on-a-Stick for VLAN 10 & VLAN 20
* Separate Layer 3 Interface for VLAN 30

---

## IP Addressing

| Department | VLAN    | Network         | Gateway      |
| ---------- | ------- | --------------- | ------------ |
| HR         | VLAN 10 | 192.168.10.0/24 | 192.168.10.1 |
| Finance    | VLAN 20 | 192.168.20.0/24 | 192.168.20.1 |
| IT         | VLAN 30 | 192.168.30.0/24 | 192.168.30.1 |

---

## Security Policy

| Source  | Destination | Result |
| ------- | ----------- | ------ |
| HR      | Finance     | Allow  |
| HR      | IT          | Allow  |
| Finance | HR          | Deny   |
| Finance | IT          | Allow  |
| IT      | HR          | Deny   |
| IT      | Finance     | Deny   |

---

## Technologies Used

* Cisco Packet Tracer
* Cisco IOS
* VLAN Configuration
* IEEE 802.1Q Trunking
* Router-on-a-Stick
* DHCP
* Inter-VLAN Routing
* Extended Access Control Lists (ACLs)

---

## Features Implemented

* VLAN Segmentation
* Dynamic IP Address Assignment using DHCP
* Inter-VLAN Routing
* Extended ACL Configuration
* Enterprise Network Security Policy
* Network Verification using Ping Tests
* Cisco IOS Troubleshooting

---

## Verification Performed

* Verified VLAN communication.
* Verified DHCP IP assignment.
* Verified Router-on-a-Stick operation.
* Verified ACL rule matching.
* Tested permitted and denied traffic between departments.
* Verified gateway connectivity.
* Verified ACL hit counters using **show access-lists**.

---

## Skills Demonstrated

* Cisco Switching
* Cisco Routing
* VLAN Design
* DHCP Configuration
* Inter-VLAN Routing
* Access Control Lists
* Enterprise Network Security
* Cisco IOS CLI
* Network Troubleshooting

---

## Future Improvements

* Named ACLs
* Standard ACLs
* OSPF Routing
* NAT/PAT
* SSH Remote Management
* Port Security
* EtherChannel
* HSRP
* Firewall Integration
* AAA Authentication

---

## Author

Developed as part of a CCNA Networking Portfolio to demonstrate enterprise networking and security skills using Cisco Packet Tracer.
