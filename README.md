# Corporate Network Simulation with Cisco Packet Tracer

## Project Overview

This project simulates a full corporate network environment using **Cisco Packet Tracer**, including multiple VLANs, inter-VLAN routing, firewall security, and external network connectivity. It is designed to demonstrate practical **network design, configuration, and security skills** commonly required in enterprise IT and cybersecurity roles.

The network consists of:

- **4 Departments (VLANs):** HR, IT, Sales, DMZ  
- **Layer-3 Core Switch** for inter-VLAN routing  
- **Cisco ASA Firewall** with NAT and ICMP inspection  
- **Edge Router** connecting to a simulated Internet host  
- **End-to-End Connectivity** from internal PCs to the Internet  

---

## Skills Demonstrated

This project highlights expertise in:

### **Networking**
- VLAN creation and management for department segmentation  
- Layer-3 switch configuration for **inter-VLAN routing**  
- Trunk and access port setup for secure and efficient network design  
- Default gateway configuration for multiple subnets  

### **Firewall & Security**
- Cisco ASA firewall configuration with:
  - **Inside/Outside interfaces**
  - **Security levels**
  - **Network Address Translation (NAT)**
  - **ICMP inspection** for reliable connectivity testing  
- VLAN segmentation to isolate sensitive network areas (e.g., DMZ)  
- Implementation of ACLs for controlled access  

### **Routing**
- Static and default route configuration on ASA and edge router  
- End-to-end traffic flow from internal VLANs to a simulated Internet network  

### **Testing & Troubleshooting**
- ICMP (ping) testing between VLANs, firewall, edge router, and Internet host  
- Troubleshooting NAT, firewall rules, and inter-VLAN routing issues  
- Validation of end-to-end connectivity and network reliability  

---

## Network Topology

- **Core Switch:** Layer-3 switch routing traffic between VLANs 10, 20, 30, 40, and 99  
- **ASA Firewall:**  
  - Inside interface (VLAN 1) connected to core switch  
  - Outside interface (VLAN 2) connected to edge router  
- **Edge Router:** Provides simulated Internet connectivity  
- **Internet Host:** 203.0.114.5, default gateway = edge router G0/1  

*Screenshots of topology, ASA configuration, and VLAN setup included in `/images`.*

---

## How to Run the Project

1. **Open the Packet Tracer file:** `CorporateNetworkProject.pkt`  
2. **Verify VLAN configuration:** Ensure each PC is assigned to the correct VLAN.  
3. **Check IP configuration:** Confirm that SVIs on the core switch, ASA, and edge router have the correct IP addresses.  
4. **Test connectivity:**
   - Internal VLAN to VLAN pings (e.g., HR ↔ IT ↔ Sales ↔ DMZ)  
   - Core Switch ↔ ASA inside interface  
   - PCs → ASA outside → Edge Router → Internet host  
5. **Optional:** Inspect firewall NAT translations and ACLs using ASA CLI.  

---

## Key Takeaways

- **Network Design:** How to structure a corporate network with multiple VLANs and a DMZ  
- **Routing & Switching:** Layer-3 inter-VLAN routing and trunk/access port configuration  
- **Firewall Security:** ASA setup with NAT, ICMP inspection, and controlled external access  
- **Practical Troubleshooting:** Diagnosing connectivity issues and resolving routing or NAT problems  
- **Professional Documentation:** Preparing a network project ready for demonstration or resume use  

## GitHub Repository Structure

