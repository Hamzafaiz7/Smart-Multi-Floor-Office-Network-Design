# Smart-Multi-Floor-Office-Network-Design
A Practical Implementation of Switching, VLANs, Trunking, and Inter-VLAN Routing.
 Abstract

This project presents the design and implementation of a scalable and efficient enterprise network using Cisco Packet Tracer. The objective is to simulate a real-world office environment where multiple departments operate within a shared infrastructure while maintaining logical separation and controlled communication. The network leverages VLAN segmentation, trunking mechanisms, and inter-VLAN routing to achieve performance, security, and scalability.

 Problem Statement

Modern organizations require networks that:

Isolate departmental traffic
Reduce broadcast domains
Ensure secure and controlled communication
Optimize resource utilization

This project addresses these requirements by designing a multi-floor office network using industry-standard networking techniques.

 Objectives
To implement logical segmentation using VLANs
To enable communication between switches using trunk links
To achieve inter-VLAN communication using Router-on-a-Stick
To simulate real-world network traffic and validate connectivity
 Network Architecture
🔹 Physical Design
Two switches representing two office floors
One router for inter-VLAN communication
End devices distributed across departments


🔹 Logical Design

Each department is assigned a dedicated VLAN and IP subnet:

Department	VLAN ID	Subnet
HR	10	192.168.10.0/24
Finance	20	192.168.20.0/24
IT	30	192.168.30.0/24
Guest	40	192.168.40.0/24
 Network Implementation
1. Switching

Switches were configured to:

Learn MAC addresses dynamically
Forward frames efficiently
Assign access ports to specific VLANs
2. VLAN Segmentation
VLANs were created on both switches
Each VLAN represents a separate broadcast domain
Ports were assigned based on departmental grouping
3. Trunking
Trunk links were established between switches and router
Multiple VLANs were transmitted over a single physical link
IEEE 802.1Q encapsulation was used for VLAN tagging
4. Inter-VLAN Routing
Router-on-a-Stick approach was implemented
Subinterfaces were configured for each VLAN
Each VLAN was assigned a default gateway
Routing decisions enabled communication between VLANs
 Configuration Overview
VLAN creation and port assignment on both switches
Trunk configuration for inter-device communication
Router subinterface configuration with IP addressing
Host configuration with IP and gateway settings
 Testing and Validation

The network was tested using the following methods:

Ping tests within the same VLAN
Ping tests across different VLANs
Verification of trunk links and VLAN propagation
Observation of packet flow in simulation mode

Results confirmed:

Successful intra-VLAN communication
Successful inter-VLAN communication via router
Proper VLAN tagging and trunk operation
 Project Evidence

The repository includes:

Network topology screenshot
VLAN configuration output
Trunk verification output
Router interface configuration
Ping test results
Simulation mode packet flow
 Discussion

The implementation demonstrates how logical segmentation using VLANs improves network efficiency and security. Trunking enables scalable expansion across multiple switches, while inter-VLAN routing ensures controlled communication between isolated networks. The project reflects real-world enterprise networking practices.

 Learning Outcomes

Through this project, the following skills were developed:

Practical understanding of switching operations
VLAN design and implementation
Trunk configuration and traffic management
Inter-VLAN routing using Router-on-a-Stick
Network troubleshooting and validation
 Repository Contents
Cisco Packet Tracer file (.pkt)
Configuration outputs
Screenshots
Documentation (README)
 Conclusion

This project successfully demonstrates the integration of fundamental networking concepts into a cohesive and functional enterprise network. It highlights the importance of structured design, logical segmentation, and efficient routing in modern network infrastructures.
