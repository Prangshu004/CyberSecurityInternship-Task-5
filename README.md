
# 🌐 Cybersecurity Internship – Task 5

## 📌 Task Title:
**Capture and Analyze Network Traffic Using Wireshark**

---

## 🧠 Objective:
To gain hands-on experience in capturing live network packets using Wireshark and analyzing the captured traffic to identify key network protocols such as TCP, DNS, and HTTP. This task is crucial for understanding network behavior and troubleshooting using packet inspection.

---

## 🛠️ Tools Used:
- **Wireshark** (Version: 4.x or latest)
- **Operating System:** Linux or Windows
- **Active Internet Connection**

---

## 🧪 Experiment Steps:

### 🧩 Step 1: Install and Open Wireshark
- Launched Wireshark and selected the active network interface (e.g., `wlan0` or `eth0`).

### 🧩 Step 2: Start Packet Capture
- Clicked **Start** to begin capturing packets.
- Performed network activity (e.g., opened websites, pinged servers).

### 🧩 Step 3: Stop Capture
- Stopped capture after ~60 seconds using the red square button.

---

## 🔍 Protocols Identified:

| Protocol | Use Case                         | Packet Count (approx) |
|----------|----------------------------------|------------------------|
| **TCP**  | Connection-oriented communication | 300+                   |
| **DNS**  | Domain resolution requests        | 20–40                  |
| **HTTP** | Web page requests                 | 15–30                  |

Captured and confirmed presence of at least three unique protocols during the session.

---

## 🔎 Filtering and Analysis:

### ✅ 1. **TCP Packets**
**Filter used:**
```wireshark
tcp
```
### ✅ 2. **DNS Packets**
**Filter used:**
```wireshark
dns
```
Detected A and AAAA record queries for domain lookups.

### ✅ 2. **HTTP Packets**
**Filter used:**
```wireshark
http
```
Displayed GET and response headers for visited websites.

### 🔐 Security Insights:

- Most traffic is routed over TCP, showing it's widely used for reliable communication.
- DNS queries are frequent and unencrypted, making them vulnerable to eavesdropping or spoofing.
- HTTP traffic is readable and unprotected (unlike HTTPS), revealing sensitive details like URLs or headers.

### 🧠 Concepts Learned:

- How to perform live packet capture using Wireshark
- Applying protocol filters to isolate traffic types
- Basics of TCP/IP communication
- Understanding of DNS resolution and HTTP traffic
- Identifying the role of each protocol in real-time network activity

### 🙋‍♂️ Author:

Name: Prangshu Das

Role: Cybersecurity Intern

Task Date: 30th June 2025
