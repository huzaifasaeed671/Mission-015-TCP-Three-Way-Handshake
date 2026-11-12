# Mission 015 – TCP Three-Way Handshake Analysis

## Overview
This project demonstrates the TCP three-way handshake and connection termination through practical network traffic analysis using Wireshark.

The investigation follows a TCP connection established between a Windows client and `example.com`, examining how TCP establishes a reliable connection before TLS communication begins.

## Objectives
- Capture TCP traffic using Wireshark.
- Identify SYN, SYN-ACK, and ACK packets.
- Understand TCP connection establishment.
- Observe TLS communication over TCP.
- Analyze TCP connection termination using FIN and ACK flags.

## Lab Environment
- **Operating System:** Windows
- **Packet Analyzer:** Wireshark
- **Website:** example.com
- **Protocol:** TCP / TLS 1.3

## Connection Details

| Field | Value |
|---|---|
| Client IP | 192.168.1.12 |
| Server IP | 104.20.23.154 |
| Client Port | 57598 |
| Server Port | 443 |

## Key Findings
The capture identified the three stages of TCP connection establishment:

1. SYN – The client initiated the connection.
2. SYN-ACK – The server acknowledged the request and responded.
3. ACK – The client acknowledged the server's response.

After the handshake, TLS communication took place. The capture also showed FIN and ACK packets involved in connection termination.

## Evidence
The `Screenshots` folder contains packet-level evidence of:
- TCP SYN
- TCP SYN-ACK
- Complete three-way handshake
- TLS communication
- TCP connection termination

## Documentation
See **TCP-Handshake-Analysis.pdf** for the complete technical report, packet observations, and screenshots.

## Tools Used
- Wireshark
- Windows Command Prompt
- curl
- nslookup

## Learning Outcome
This practical exercise improved my understanding of TCP connection establishment, packet flags, sequence and acknowledgment numbers, TLS communication, and connection termination.

---

**Project:** Mission 015 – TCP Three-Way Handshake Analysis  
**Focus:** Network Traffic Analysis
