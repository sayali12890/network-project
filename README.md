# network-project

# 🏨 Hotel Network Design & Implementation Project

## 📌 Project Overview
This project involves designing and implementing a modern hotel network infrastructure using routing, switching, VLANs, and network services. The hotel consists of three floors, each with multiple departments, and the network is designed to ensure secure, efficient, and scalable communication.

## 🏢 Network Structure

### 📍 Floors & Departments

#### 🥇 1st Floor
- Reception → VLAN 80 → 192.168.8.0/24  
- Store → VLAN 70 → 192.168.7.0/24  
- Logistics → VLAN 60 → 192.168.6.0/24  

#### 🥈 2nd Floor
- Finance → VLAN 50 → 192.168.5.0/24  
- HR → VLAN 40 → 192.168.4.0/24  
- Sales/Marketing → VLAN 30 → 192.168.3.0/24  

#### 🥉 3rd Floor
- Admin → VLAN 20 → 192.168.2.0/24  
- IT → VLAN 10 → 192.168.1.0/24  

---

## 🛠️ Network Requirements

- 3 routers (one per floor, placed in server room)
- Routers connected using **Serial DCE cables**
- Inter-router networks:
  - 10.10.10.0/30  
  - 10.10.10.4/30  
  - 10.10.10.8/30  
- 1 switch per floor
- WiFi access for laptops and mobile devices
- Each department has:
  - Separate VLAN
  - Dedicated printer


## ⚙️ Technologies Used

- Cisco Packet Tracer / GNS3  
- VLAN Configuration  
- Inter-VLAN Routing  
- OSPF Routing Protocol  
- DHCP Configuration  
- SSH Remote Access  
- Port Security  


## 🚀 Key Features

- 🔐 Network segmentation using VLANs  
- 🌐 Dynamic routing using OSPF  
- 📡 Wireless connectivity for users  
- 🖨️ Printer access in each department  
- ⚡ Automatic IP allocation using DHCP  
- 🔒 Secure remote access using SSH  
- 🛡️ Port security to restrict unauthorized devices  


## 🔧 Configuration Details

### Routing
- OSPF is used to advertise routes between routers

### DHCP
- Each router acts as DHCP server for its VLANs

### SSH
- Configured on all routers for secure remote login

### Port Security
- Applied on IT switch:
  - Only Test-PC allowed on Fa0/1
  - Sticky MAC enabled
  - Violation mode: Shutdown


## 🧪 Testing

- Test-PC added in IT department
- Used to verify SSH remote login
- Ensure:
  - All VLANs can communicate
  - Routing is successful
  - Devices receive IP via DHCP


## 📊 Expected Outcomes

- Full connectivity between all departments  
- Secure VLAN-based communication  
- Dynamic IP assignment working correctly  
- Remote login via SSH successful  
- Unauthorized access blocked via port security  


## 📚 Applications

- Enterprise network design  
- Hotel and hospitality industry  
- Secure multi-department networks  
- Real-world networking simulation  


## 👩‍💻 Author
- MANE SAYALI


## 📅 Duration
- 2-3 Weeks


## 📌 Conclusion
This project demonstrates practical implementation of networking concepts such as VLAN segmentation, dynamic routing using OSPF, secure remote access, and network protection techniques. It simulates a real-world hotel network infrastructure.

