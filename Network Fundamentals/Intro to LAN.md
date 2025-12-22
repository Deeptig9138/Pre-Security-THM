# Intro to LAN

---

## 🧩 Task 1: Introducing LAN Topologies

### 🌐 Local Area Network (LAN) Topologies

Over the years, various network designs have been experimented with and implemented. In networking, a **topology** refers to the **design or layout of a network**. Each topology has its own advantages and disadvantages.

### ⭐ Star Topology

In a **star topology**, all devices are individually connected to a **central networking device** such as a **switch or hub**.

![star topology](https://github.com/Deeptig9138/Pre-Security-THM/blob/main/screenshots/Star-Topology.png)

#### ✅ Advantages
- Highly **reliable**
- **Scalable** – easy to add new devices
- Commonly used in modern networks

#### ❌ Disadvantages
- **Expensive** due to extra cabling and central hardware
- Increased **maintenance** as the network grows
- If the central device fails, communication stops

> Despite the risk, central devices are usually robust, reducing failure chances.


### 🚌 Bus Topology

In a **bus topology**, all devices share a single backbone cable.

![bus topology](https://github.com/Deeptig9138/Pre-Security-THM/blob/main/screenshots/bus-topology.png)

#### ✅ Advantages
- **Cost-efficient**
- Easy to set up
- Minimal cabling required

#### ❌ Disadvantages
- Prone to **bottlenecks**
- Difficult to troubleshoot
- **Single point of failure** – if the backbone breaks, the whole network fails

### 🔁 Ring Topology

In a **ring topology**, devices are connected in a loop, passing data around the ring.

![ring topology](https://github.com/Deeptig9138/Pre-Security-THM/blob/main/screenshots/ring-topology.png)

#### ✅ Advantages
- Less cabling required
- Easier troubleshooting (single data direction)
- Less prone to bottlenecks

#### ❌ Disadvantages
- Inefficient data paths
- A single faulty device or cable can break the entire network

### 🔀 What is a Switch?

A **switch** is a networking device used to connect multiple devices (PCs, printers, servers) within a LAN using Ethernet.

![switch](https://github.com/Deeptig9138/Pre-Security-THM/blob/main/screenshots/switch.jpg)

- Available in 4, 8, 16, 24, 32, or 64 ports
- Sends data **only to the intended device**
- Reduces unnecessary network traffic
- More efficient than hubs/repeaters

Switches and routers can be interconnected to improve **redundancy** and reliability.

### 🌍 What is a Router?

A **router** connects **multiple networks** and forwards data between them.

![router](https://github.com/Deeptig9138/Pre-Security-THM/blob/main/screenshots/router.png)

- Uses a process called **routing**
- Determines the best path for data
- Essential for connecting LANs to the Internet

### 🧪 Practical

An interactive lab demonstrates how LAN topologies fail under different conditions.  
Break the LAN topologies to retrieve the flag.

#### ✅ Answers
- **LAN stands for:** Local Area Network  
- **Router function verb:** Routing  
- **Central device in LAN:** Switch  
- **Cost-efficient topology:** Bus Topology  
- **Expensive topology:** Star Topology  
- **Flag:** `THM{TOPOLOGY_FLAWS}`  

---

## 🧩 Task 2: A Primer on Subnetting

### 🧠 What is Subnetting?

**Subnetting** is the process of dividing a large network into **smaller subnetworks**.  
Think of it like slicing a cake—each department gets its own piece.

Subnetting helps networks:
- Identify where data should go
- Improve organization and efficiency

### 🧮 Subnet Masks

- A subnet mask is a **32-bit number**
- Made of **four octets (0–255)**
- Used to divide network and host portions of an IP address

### 📌 IP Address Roles in Subnetting

| Type | Purpose | Example |
|-----|--------|--------|
| **Network Address** | Identifies the network | 192.168.1.0 |
| **Host Address** | Identifies a device | 192.168.1.100 |
| **Default Gateway** | Sends data to other networks | 192.168.1.254 |

### 🔐 Why Subnetting Matters

Subnetting provides:
- **Efficiency**
- **Security**
- **Control**

Example:  
A café may have:
- One subnet for staff and internal devices  
- One subnet for public Wi-Fi users  

#### ✅ Answers
- **Dividing a network:** Subnetting  
- **Bits in subnet mask:** 32  
- **Octet range:** 0–255  
- **Start of network:** Network Address  
- **Device identifier:** Host Address  
- **Network exit device:** Default Gateway  

---

## 🧩 Task 3: ARP (Address Resolution Protocol)

Devices use two identifiers:
- **IP Address** (logical)
- **MAC Address** (physical)

**ARP** maps IP addresses to MAC addresses.

### 🔄 How ARP Works

Each device maintains an **ARP cache**.

ARP uses two messages:
- **ARP Request** – Broadcast asking who owns an IP
- **ARP Reply** – Response containing the MAC address

Once received, the mapping is saved for future communication.

#### ✅ Answers
- **ARP stands for:** Address Resolution Protocol  
- **Packet asking for IP owner:** Request  
- **Physical identifier:** MAC Address  
- **Logical identifier:** IP Address  

---

## 🧩 Task 4: DHCP

**DHCP (Dynamic Host Configuration Protocol)** automatically assigns IP addresses to devices.

### 📡 DHCP Process

1. **DHCP Discover** – Device looks for a DHCP server  
2. **DHCP Offer** – Server offers an IP address  
3. **DHCP Request** – Device accepts the offer  
4. **DHCP ACK** – Server confirms assignment  

#### ✅ Answers
- **Packet to get IP:** DHCP Discover  
- **Packet to accept IP:** DHCP Request  
- **Final packet:** DHCP ACK  

---

## 🧠 Key Takeaways

- Network **topologies** impact cost, performance, and reliability  
- **Switches** efficiently manage LAN traffic  
- **Routers** enable communication between networks  
- **Subnetting** improves security and network organization  
- **ARP** bridges logical and physical addressing  
- **DHCP** automates IP management and reduces configuration errors  

---

## 🏁 Summary

This room builds the foundation of networking knowledge required for cybersecurity.  
Understanding LAN topologies helps identify infrastructure weaknesses. Subnetting enforces segmentation and security boundaries. ARP and DHCP explain how devices identify themselves and communicate automatically. Together, these concepts form the backbone of both offensive and defensive security operations and are critical for analyzing, attacking, and securing modern networks.
