# Packet Tracer - Configure DHCP on a Wireless Router

## 📘 Objective

Configure a wireless router to serve as a DHCP server for three wired PCs in Cisco Packet Tracer.

---

## 🧱 Topology Overview

- **1 Wireless Router**
- **3 Generic PCs**
- **3 Ethernet straight-through cables**

Each PC is wired to the router's Ethernet port and receives its IP address dynamically via DHCP.
<img width="1917" height="1013" alt="image" src="https://github.com/user-attachments/assets/62c93c7f-f092-4769-a3c6-c552ba7fac13" />


---

## 🛠️ Configuration Steps

### Part 1: Set Up Network Topology

- Add 3 Generic PCs
- Connect each to the wireless router via straight-through cables

### Part 2: Observe Default DHCP Settings
<img width="1916" height="1023" alt="Packet Tracer 2nd-4" src="https://github.com/user-attachments/assets/638a2306-d95d-49d2-9ab0-bd23d3fb0f87" />


- Default Gateway observed on PC0: `192.168.0.1` (default router IP)

### Part 3: Modify Wireless Router IP

- Change router IP to `192.168.5.1`
- Reconnect and re-obtain DHCP settings on PC0
<img width="1915" height="1023" alt="Packet Tracer 2nd-2" src="https://github.com/user-attachments/assets/a5ce9508-8558-4f7e-a68f-913d9f834885" />

### Part 4: Modify DHCP Range

- Start IP Address: `192.168.5.126`
- Max Users: `75`
- Renew IP addresses on PC0

> 🧪 **PC0 Assigned IP:** `192.168.5.126`

### Part 5: Enable DHCP on PC1 and PC2

> 🧪 **PC1 Assigned IP:** `192.168.5.127`  
> 🧪 **PC2 Assigned IP:** `192.168.5.128` (example)
<img width="1920" height="1022" alt="image" src="https://github.com/user-attachments/assets/9b4a7726-b235-41a9-9270-97244ec1efcc" />

<img width="1916" height="1023" alt="Packet Tracer 2nd-4" src="https://github.com/user-attachments/assets/6a4a33d9-4c23-41c4-be41-a5e21cceaf71" />
### Part 6: Test Connectivity

Run the following commands on PC2:
```bash
ipconfig
ping 192.168.5.1     # Router
ping 192.168.5.126   # PC0
ping 192.168.5.127   # PC1
```
<img width="1920" height="1023" alt="Packet Tracer 2nd-3" src="https://github.com/user-attachments/assets/4050ba06-d06a-40b9-b9f0-4535ce3a95dc" />

Activity Results

<img width="1920" height="1023" alt="Packet Tracer 2nd" src="https://github.com/user-attachments/assets/9d33922e-e85a-4569-a7e0-116afcc5d519" />





