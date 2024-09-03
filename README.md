# Fundamentals of Computer Networks (FRC) - Practical Project 2021/22

## Department of Information Sciences and Technologies

### Project Overview

This practical project, part of the **Fundamentals of Computer Networks (FRC)** course, involves designing and testing a medium-sized enterprise network using the Cisco Packet Tracer simulator. The main objective is to give students a hands-on understanding of the technologies and protocols used in creating enterprise networks.

### Objectives

- Design and implement a medium-sized enterprise network.
- Perform functional tests to validate the network's operation.
- Apply concepts of VLANs, STP, DHCP, and routing protocols (static and dynamic).
- Document the project with screenshots and configuration analysis.

### Project Structure

1. **Introduction and Objectives**:  
   The goal is to understand and apply network technologies in a simulated enterprise scenario using Cisco Packet Tracer, including planning, implementation, and functional testing.

2. **Network Characteristics**:
    - **Branches and Departments**: The company Xpto, Lda has four branches (Lisbon, Porto, Faro, and Ponta Delgada), each with specific departments.
        - **Lisbon**:
            - Technical Department (DTEC-LX) for 40 workstations.
            - Human Resources Department (RH-LX) for 20 workstations.
            - WiFi network supporting up to 100 simultaneous devices.
            - Server Network (SRV) with 10 servers (DHCP, HTTP).
        - **Porto, Faro, and Ponta Delgada**:
            - Technical Department supporting 20 workstations.
            - Human Resources Department supporting 10 workstations.

3. **Separation and Interconnection of Branches and Departments**:
    - Each branch will be interconnected using switches, with the number of switches depending on the size of the branch.
    - In Lisbon, physical redundancy between switches will be implemented to support Layer 2 switching.
    - A dedicated switch and one or more Access Points (APs) will support the WiFi network.
    - Each branch will have a router for interconnecting with other branches, forming a ring topology:
        - Lisbon connects to Porto and Faro.
        - Porto connects to Lisbon and Ponta Delgada.
        - Ponta Delgada connects to Porto and Faro.
        - Faro connects to Lisbon and Ponta Delgada.

4. **VLANs**:
    - Implement VLANs to enhance network security and traffic separation. Each department will be assigned its own VLAN.

5. **Network Design and Equipment Selection**:
    - Identify the types and quantities of equipment needed based on the described requirements.
    - Implement the physical network design in Packet Tracer, using different switches and PCs for each department and branch.

6. **Layer 2 Redundancy and Spanning Tree Protocol (STP)**:
    - Design a redundant Layer 2 network for the Lisbon branch using STP.
    - Analyze the resulting spanning tree and test connectivity.

7. **Address Space Planning**:
    - Use the private network `10.10.16.0/22` for machines and gateways.
    - Use private inter-router networks (`192.168.1.x/30`) for router interconnections.

8. **Router Configuration**:
    - Configure router interfaces and sub-interfaces for local and inter-branch communications.
    - Implement both static and dynamic routing (RIP) configurations.

9. **Functional Testing**:
    - Perform connectivity tests between PCs in the same and different VLANs.
    - Configure DHCP and HTTP services and verify their operation.
    - Conduct tests to observe ARP, DHCP, and RIP protocol behavior.

10. **Documentation**:
    - Include relevant Packet Tracer screenshots and explanations in the project report.


