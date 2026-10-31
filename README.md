# Secure Hybrid Data Center Network Architecture
### Cisco AICTE Virtual Internship Program 2026 | Networking

![Cisco Networking Academy](https://img.shields.io/badge/Cisco-Networking%20Academy-blue)
![Internship](https://img.shields.io/badge/Internship-AICTE%202026-00A6D6)
![Domain](https://img.shields.io/badge/Domain-Network%20Security-red)
![Tool](https://img.shields.io/badge/Simulation-Cisco%20Packet%20Tracer-green)

##  Project Overview

This project focuses on designing a **Secure Hybrid Data Center Network Architecture** as part of the Cisco AICTE Virtual Internship Program 2026.

Modern enterprises increasingly rely on hybrid infrastructure, where applications and services operate across private data centers and public cloud environments. This creates security challenges involving unauthorized access, insecure communication, network vulnerabilities, and lateral movement between interconnected systems.

The objective of this project is to design a secure, scalable, and manageable enterprise network architecture that protects critical infrastructure while allowing authorized communication between different network segments.

The network topology is developed and simulated using **Cisco Packet Tracer**.

##  Problem Statement

Design a secure hybrid data center network architecture that:

- Enables secure communication between private data centers and public cloud environments.
- Implements network segmentation to isolate applications and critical resources.
- Restricts unauthorized communication between network segments.
- Provides secure access to enterprise resources for remote faculty and employees.
- Implements identity and access management principles.
- Minimizes the risk of lateral movement if an application or network segment is compromised.
- Maintains availability, scalability, and manageable network infrastructure.

##  Project Objectives

1. Design a structured enterprise network topology.
2. Implement network segmentation and controlled communication.
3. Establish appropriate routing and network access policies.
4. Apply security mechanisms to restrict unauthorized traffic.
5. Understand secure connectivity between distributed infrastructure.
6. Evaluate the architecture against common network security threats.
7. Develop a scalable network design following the principle of least privilege.

##  Architecture and Design Approach

The proposed architecture follows a layered security approach:

| Layer | Responsibility |
|---|---|
| Network Layer | Routing and inter-network communication |
| Segmentation Layer | Separation of departments, applications and resources |
| Access Control Layer | Restricting unauthorized network traffic |
| Perimeter Security | Controlling inbound and outbound communication |
| Identity Layer | Authentication and authorization |
| Monitoring Layer | Network visibility and security analysis |

### High-Level Architecture

```text
                    INTERNET
                       |
                PERIMETER SECURITY
                       |
                ENTERPRISE NETWORK
                       |
              NETWORK SEGMENTATION
                       |
          +------------+------------+
          |            |            |
       SEGMENT A    SEGMENT B    SEGMENT C
          |            |            |
       Devices      Servers      Applications
          |            |            |
          +------------+------------+
                       |
                CONTROLLED ROUTING
                       |
              PRIVATE DATA CENTER
                       |
              SECURE CLOUD CONNECTIVITY
                       |
                  PUBLIC CLOUD
```

*Note: This is a conceptual architecture. Refer to the included Packet Tracer file for the actual simulated topology.*

##  Security Concepts

### 1. Network Segmentation

Network segmentation divides a large enterprise network into smaller, isolated logical networks.

Benefits:
- Limits unauthorized communication.
- Reduces the attack surface.
- Restricts lateral movement.
- Helps contain security incidents.
- Separates critical infrastructure from general user networks.

### 2. Access Control

Access control mechanisms regulate communication between network devices and resources.

The design follows a default-deny approach wherever applicable: only explicitly authorized traffic should be permitted.

### 3. Secure Network Connectivity

Secure connectivity is essential when applications and services communicate across different infrastructure environments.

The architecture considers:
- Secure communication channels.
- Controlled routing between networks.
- Restricted access to critical resources.
- Protection of sensitive information in transit.

### 4. Identity and Access Management (IAM)

IAM ensures that users and administrators receive only the permissions necessary to perform their tasks.

Important principles:
- Role-Based Access Control (RBAC).
- Multi-Factor Authentication (MFA).
- Least-privilege access.
- Separation of administrative privileges.
- Authentication and access logging.

### 5. Lateral Movement Prevention

Lateral movement occurs when an attacker compromises one system and attempts to access other systems within the network.

The architecture aims to reduce this risk through:
- Network isolation.
- Traffic filtering.
- Access restrictions.
- Controlled inter-segment communication.
- Continuous security monitoring.

##  Technologies and Tools

| Technology | Purpose |
|---|---|
| Cisco Packet Tracer | Network topology design and simulation |
| Cisco Networking Devices | Enterprise network infrastructure |
| Networking Protocols | Communication and routing |
| Network Security Controls | Traffic filtering and access restrictions |
| Hybrid Cloud Concepts | Private data center and public cloud connectivity |

##  Testing and Validation

The network design should be evaluated using the following scenarios:

| Test Scenario | Expected Outcome |
|---|---|
| Communication between authorized devices | Successful connectivity |
| Access to restricted network segments | Blocked |
| Unauthorized inter-network communication | Denied |
| Access to protected resources | Restricted to authorized users |
| Network connectivity testing | Successful where routing and policies permit |

Testing can be performed using Packet Tracer simulation mode, ping, traceroute, and device configuration inspection.

##  Hybrid Cloud Security Considerations

Although the Packet Tracer topology provides a network simulation environment, the original problem also involves cloud-native security.

The proposed architecture considers the following technologies for a real-world deployment:

- **VPCs:** Isolated virtual networks for cloud applications.
- **Security Groups:** Workload-level traffic restrictions.
- **Network ACLs:** Subnet-level traffic filtering.
- **IPsec Site-to-Site VPN:** Encrypted communication between private data centers and public cloud.
- **IAM:** Centralized identity and permission management.
- **Kubernetes Network Policies:** Pod-level communication restrictions.
- **SIEM:** Centralized security monitoring and threat detection.

These are architectural considerations, not claims of deployment within the Packet Tracer simulation.

##  Project Files

```text
Secure-Hybrid-Data-Center-Network/
│
├── AKRITI_SINHA_KIET_PACKET_TRACER_FILE.pkt
│
└── README.md
```

##  How to Run the Project

1. Install Cisco Packet Tracer on your computer.
2. Clone or download this repository.
3. Locate the `.pkt` project file.
4. Open the file using Cisco Packet Tracer.
5. Explore the network topology and device connections.
6. Inspect device configurations and network security policies.
7. Use Simulation Mode to observe network communication.
8. Perform connectivity tests to validate the configured network.

##  Key Learnings

Through this project, I explored:

- Enterprise network architecture and design.
- Network segmentation and access control.
- Secure communication between network segments.
- Hybrid cloud security concepts.
- Network security principles and threat mitigation.
- The importance of defense in depth.
- Designing scalable and manageable network infrastructure.

##  Future Enhancements

The project can be extended through:

- Integration with AWS VPC and cloud security groups.
- Implementation of Site-to-Site IPsec VPN.
- Centralized authentication using AAA/RADIUS.
- IDS/IPS integration for threat detection.
- SIEM integration using Wazuh or Splunk.
- Kubernetes namespace isolation and network policies.
- Automated network configuration and security validation.

##  Acknowledgement

I sincerely thank **Cisco Networking Academy, AICTE, the Ministry of Education, and the Cisco AICTE Virtual Internship Program 2026 partners** for providing this opportunity to explore networking concepts and work on an enterprise-focused network security problem.

This project was developed as part of my internship learning journey from **June to August 2026**.

---

**Author:** Akriti Sinha  
**Institution:** KIET Group of Institutions, Delhi-NCR, Ghaziabad  
**Program:** Cisco AICTE Virtual Internship Program 2026  
**Domain:** Networking & Cybersecurity  
**Project Tool:** Cisco Packet Tracer

 If you find this project interesting, feel free to explore the repository and share your feedback!
