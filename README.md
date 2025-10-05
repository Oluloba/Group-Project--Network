# University Network Design and Implementation Project

## Project Overview
This project objective is for design and implementation of a scalable and secure network infrastructure for a large institution with two campuses located 20 miles apart.  
The network supports administrative operations, academic departments, and student labs, ensuring efficient communication, security, and accessibility.

The simulation was designed in **Draw.io** and implemented using **Cisco Packet Tracer**.

---

## Network Structure
### **Main Campus**
- **Building A:** Management, HR, Finance, and Faculty of Business  
  - VLANs 10–40  
  - DHCP-enabled via router-based server
- **Building B:** Engineering and Art Faculties  
  - VLANs 50 and 60  
- **Building C:** Student Labs and IT Department  
  - VLANs 70 and 80  
  - Hosts internal Web Server and DMZ

### **Smaller Campus**
- **Faculty of Health and Sciences**  
  - VLAN 90  
  - Static addressing and WAN connectivity to main campus

---

## Key Configurations
### **Routing**
- **RIPv2** configured for internal router communication between campuses  
- **Static route** used for external email server 

### **DHCP**
- Configured on the **Main Campus router** for Building A VLANs  
- Excluded addresses reserved for routers, switches, and servers

### **Security** 
ACLs implemented to:
  - Block unauthorized access between sensitive VLANs (e.g., Finance ↔ HR)
  - Restrict external access to DMZ services only

---

## Tools Used
- **Cisco Packet Tracer** – Network simulation and configuration  
- **Draw.io** – Network topology diagram  
- **Git & GitHub** – Version control and documentation  
 

---

## Testing Summary
- Successful **end-to-end connectivity** across campuses  
- Dynamic IP addresssing via DHCP and inter-VLAN routing.  
- Confirmed **ACL security** through controlled access testing. 
- External connectivity to cloud email server verified via static route

---

## Project report by
**Oluwatobi Aladejare**  
Cybersecurity 
AltSchool – 2024/2025  

---

## License
This project is for academic and demonstration purposes only. Redistribution or commercial use requires permission.

