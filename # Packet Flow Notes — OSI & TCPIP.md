# Packet Flow Notes — OSI & TCP/IP Model

## Real Scenario
A user opens:

https://www.youtube.com

The browser sends traffic through:
- Switch
- Router
- ISP
- Internet
- YouTube Server

---

# Data Flow Through OSI Layers

## Layer 7 — Application Layer
Protocols:
- HTTP
- HTTPS
- DNS

Example:
Browser creates HTTPS request.

---

## Layer 6 — Presentation Layer
Handles:
- Encryption
- Compression
- Encoding

Example:
TLS/SSL encryption for HTTPS.

---

## Layer 5 — Session Layer
Creates communication session between:
Client ↔ Server

---

## Layer 4 — Transport Layer
Protocol:
- TCP
- UDP

Example:
HTTPS uses TCP Port 443.

Source Port Example:
49152

Destination Port:
443

PDU:
Segment

---

## Layer 3 — Network Layer
Protocol:
IP

Example:
Source IP: 192.168.1.10
Destination IP: 142.250.x.x

Routers operate here.

PDU:
Packet

---

## Layer 2 — Data Link Layer
Protocol:
Ethernet

Uses:
MAC Addresses

Example:
Source MAC: PC MAC
Destination MAC: Router MAC

Switches operate here.

PDU:
Frame

---

## Layer 1 — Physical Layer
Data becomes:
Bits

Transmitted using:
- Ethernet cable
- Wi-Fi
- Fiber optic

PDU:
Bits

---

# Encapsulation Process

Application Data
↓
TCP Segment
↓
IP Packet
↓
Ethernet Frame
↓
Bits

---

# Important Ports

| Protocol | Port |
|---|---|
| HTTP | 80 |
| HTTPS | 443 |
| DNS | 53 |
| SSH | 22 |
| FTP | 20/21 |

---

# Device and OSI Layer Mapping

| Device | Layer |
|---|---|
| Switch | Layer 2 |
| Router | Layer 3 |
| Firewall | Layer 3/4+ |

---

# Key Takeaways

- Switches use MAC addresses.
- Routers use IP addresses.
- TCP provides reliable delivery.
- HTTPS uses Port 443.
- DNS resolves domain names to IP addresses.
- Encapsulation adds headers at each layer.