# 🌐 Networking Fundamentals 

---

## 🧩 Task 1 — What is Networking?

A **network** is simply **things connected together**.

A simple real-life example is your friendship circle — people are connected through shared interests, skills, or interactions.

### 🌍 Networks Exist Everywhere
- City public transportation systems  
- National power grids  
- Postal systems  
- Social interactions with neighbors  

### 💻 Networking in Computing
In computing, networking follows the same idea — but instead of people, **devices** are connected.

Examples of networked devices include:
- Laptops and smartphones  
- Security cameras  
- Traffic lights  
- Smart farming devices  

A network can consist of:
- As few as **2 devices**
- As many as **billions of devices**

Networking is deeply embedded in daily life:
- Weather forecasting  
- Power delivery  
- Traffic control systems  

Because of this, **networking is a core concept in cybersecurity**.

📌 **Key Term**  
**Q:** What is the key term for devices that are connected together?  
**A:** `Network`

---

## 🌍 Task 2 — What is the Internet?

The **Internet** is one **giant network** made up of **many smaller networks**.

### 🧠 Conceptual Example
Alice knows Bob and Jim. She also knows Zayn and Toby — but Bob and Jim don’t speak the same “language” as Zayn and Toby.

Alice acts as the **translator**, enabling communication and forming a larger network.

💡 This is how the Internet works — it connects different networks together.

### 🕰️ A Brief History
- **1960s:** ARPANET project (US Defense Department)  
- **1989:** Tim Berners-Lee invents the **World Wide Web (WWW)**  

This is when the Internet evolved into a platform for storing and sharing information.

### 🌐 Types of Networks
- **Private Networks:** Internal networks (home, office)
- **Public Networks:** Networks connecting private networks (the Internet)

📌 **Question**  
**Q:** Who invented the World Wide Web?  
**A:** `Tim Berners-Lee`

---

## 🖥️ Task 3 — Identifying Devices on a Network

Devices must be **identifiable** to communicate.

### 👤 Human Analogy
Humans have:
- Name (changeable)
- Fingerprints (permanent)

Devices have:
- **IP Address** (changeable)
- **MAC Address** (permanent hardware identifier)

---

## 🌐 IP Addresses

An **IP Address (Internet Protocol Address)** identifies a device on a network **temporarily**.

### 🔢 Structure
- Divided into **four sections**
- Each section is called an **octet**
- Example (IPv4): `192.168.1.77`

### 🌍 Public vs Private IPs

| Device Name | IP Address | Type |
|------------|-----------|------|
| DESKTOP-KJE57FD | 192.168.1.77 | Private |
| DESKTOP-KJE57FD | 86.157.52.21 | Public |
| CMNatic-PC | 192.168.1.74 | Private |
| CMNatic-PC | 86.157.52.21 | Public |

- **Private IPs:** Used within internal networks  
- **Public IPs:** Assigned by ISP, visible to the Internet  

📌 All outgoing traffic appears to come from the **same public IP**.

### 📈 IPv4 vs IPv6

**IPv4**
- 2³² addresses (~4.29 billion)
- Running out of addresses

**IPv6**
- 2¹²⁸ addresses (340 trillion+)
- More efficient
- Solves address exhaustion

## 🧾 MAC Addresses

A **MAC Address (Media Access Control)** is:
- A **physical identifier**
- Assigned at the factory
- 12-character hexadecimal value
- Example: `a4:c3:f0:85:ac:2d`

### 🧪 MAC Spoofing
MAC addresses can be **spoofed** (faked).

⚠️ Poor security designs that trust MAC addresses can be bypassed.

Example:
- Firewalls allowing traffic from admin MAC
- Attacker spoofs admin MAC → gains access

📌 **Questions**

**Q:** What does "IP" stand for? 

**A:** `Internet Protocol`

**Q:** What is each section of an IP address called?

**A:** `Octet`

**Q:** How many sections does IPv4 have? 

**A:** `4`

**Q:** What does "MAC" stand for? 

**A:** `Media Access Control`
  
---

### 🏨 Practical — MAC Spoofing Lab
In a simulated hotel Wi-Fi:
- Alice (paid) has access  
- Bob (unpaid) is blocked  

By spoofing Bob’s MAC to match Alice’s, Bob gains access.

  **Q:** What is the flag after spoofing MAC?  
  **A:** `THM{YOU_GOT_ON_TRYHACKME}`

![PS1](https://github.com/Deeptig9138/Pre-Security-THM/blob/main/screenshots/ps1.png)

---

## 📡 Task 4 — Ping (ICMP)

**Ping** is one of the most fundamental network tools.

### 🧠 How Ping Works
- Uses **ICMP (Internet Control Message Protocol)**
- Sends **echo request**
- Receives **echo reply**
- Measures **latency** (response time)

### 🛠 Syntax
```
ping <IP address or URL>
ping 10.10.10.10
```

---

## 🧪 Practical — Ping Lab

Ping the address 8.8.8.8 to retrieve the flag.

📌 Questions

What protocol does ping use? → ICMP

Syntax to ping 10.10.10.10? → ping 10.10.10.10

**Q:** Flag obtained from pinging 8.8.8.8?

**A:** THM{I_PINGED_THE_SERVER}

![PS2](https://github.com/Deeptig9138/Pre-Security-THM/blob/main/screenshots/ps2.png)

---

## 📝 Key Takeaways

Networks are everywhere — digital and physical

The Internet is a network of networks

Devices are identified using IP and MAC addresses

IPv6 solves IPv4 exhaustion

MAC spoofing can bypass weak security

Ping helps verify connectivity and latency

---

### 🏁 Summary

This room lays the foundation for understanding how devices communicate, how they identify each other, and how basic networking tools work — all of which are critical concepts in cybersecurity, penetration testing, and defensive security.
