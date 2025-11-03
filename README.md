# multi-building-office-network

This project demonstrates the design and implementation of a scalable enterprise network for a multi-building organization with four distinct departments: Corporate HQ, Sales & Marketing, IT & Engineering, and Operations.

<img width="914" height="255" alt="ccna-project-ss2" src="https://github.com/user-attachments/assets/23a80149-4440-403a-9fe9-c97539a4dae0" />

<img width="950" height="361" alt="ccna-project-ss1" src="https://github.com/user-attachments/assets/5ff78552-9f97-4c5c-ab22-7f8e8955397f" />

Network Architecture
Topology Design

Core Layer: Two 3560-24PS multilayer switches with redundant connections
Distribution Layer: Four 3560-24PS multilayer switches (one per building)
Access Layer: Eight 2960 switches connecting end devices

Buildings and Departments

Building A - Executive, HR, Finance
Building B - Sales, Marketing
Building C - IT, Engineering
Building D - Operations

Technical Implementation
1. IP Addressing Scheme
Management Network

Network: 192.168.1.0/24
Core-SW1: 192.168.1.10
Core-SW2: 192.168.1.11
Distribution Switches: 192.168.1.20-23
Access Switches: 192.168.1.30-60

2. Switch Configuration
Core Switches

Configured with management IPs
Trunk links using 802.1Q encapsulation
OSPF routing enabled
All VLANs created for propagation

Distribution Switches

Layer 3 routing enabled (ip routing)
VLAN interfaces (SVIs) configured as default gateways
OSPF for dynamic routing between buildings
DHCP services for respective VLANs

Access Switches

Port assignments to specific VLANs
Trunk links to distribution layer
Access mode ports for end devices

3. Trunk Configuration
All inter-switch links configured as trunks.

4. VLAN Configuration
VLANs created on all switches and Inter-VLAN also configured.

5. Routing done using OSPF and DHCP enabled across the network.

The project was built on Cisco Packet Tracer.
