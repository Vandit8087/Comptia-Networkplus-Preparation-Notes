# Wireshark Analysis of TCP Handshake and HTTP Traffic (Day 8 – Phase 1)

## 📖 Overview
This project presents a structured analysis of the **TCP three-way handshake** and **HTTP communication** using Wireshark.  
The exercise was conducted as part of a progressive cybersecurity learning plan (Day 8 – Phase 1) with the goal of reinforcing practical skills in **network protocol analysis**, **packet dissection**, and **technical documentation**.

---

## 🎯 Objectives
- Capture and document the **TCP handshake sequence (SYN, SYN-ACK, ACK)**.  
- Analyze **sequence numbers, acknowledgments, and control flags**.  
- Observe **HTTP requests and responses** at the application layer.  
- Correlate **transport layer mechanisms** with **application layer data transfer**.  
- Produce professional-level reporting, reflecting penetration testing and academic research standards.  

---

## 🛠️ Tools & Environment
- **Wireshark** – Protocol capture and analysis.  
- **Windows 10 (Host)** + **Kali Linux (VM, NAT networking)**.  
- **Traffic Generators**: `curl`, `wget`, and modern browsers.  

---

## 🔬 Methodology
1. Traffic Capture
   - Initiated packet capture on the active interface.  
   - Generated controlled traffic by browsing websites and executing HTTP requests.  

2. Filtering and Inspection  
   - Applied Wireshark filters:  
     - `tcp.handshake` → handshake sequence.  
     - `http` → HTTP request/response exchange.  

3. Handshake Analysis  
   - Verified the **SYN → SYN-ACK → ACK** sequence.  
   - Recorded client/server IPs, ports, sequence numbers, and flags.  

4. HTTP Analysis 
   - Inspected **HTTP methods (GET)**, request headers, and responses.  
   - Validated **server response codes (200 OK, redirects)**.  
   - Examined headers and payload metadata.  


## 📊 Key Insights
- The **TCP 3-way handshake** establishes reliable stateful communication, confirmed by synchronized sequence/ACK numbers.  
- HTTP traffic flows in plaintext over TCP, making it fully visible in Wireshark.  
- Wireshark enables precise visibility into **headers, methods, and status codes**, vital for network diagnostics and security assessments.  
- Reinforces the need for encrypted communication (TLS/HTTPS) to prevent data interception.  


## 📘 Learning Outcomes
- Deeper understanding of the interaction between **Transport (Layer 4)** and **Application (Layer 7)** protocols.  
- Improved ability to isolate, filter, and interpret packet data.  
- Professional documentation practice, bridging **technical analysis with penetration testing reporting**.  

