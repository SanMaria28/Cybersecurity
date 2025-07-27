# Network

Understanding network and subnet, MAC ID, IP Address, difference between IPv4 and IPv6, TCP and UDP.

-----
### What is Network?
A network, specifically a computer network, is a ***system of two or more interconnected computing devices*** (like computers, servers, printers, smartphones) that ***communicate and share data and resources with each other***. These connections can be made using physical wires (such as Ethernet cables or fiber optics) or wireless technologies (like Wi-Fi or cellular signals).
#### Key Points
- Communication follows a set of rules called protocols, such as TCP/IP, which govern how data is transmitted and received across the network.
- Networks can be as small as two connected devices or as large as the global Internet.
- Essential network devices include routers, switches, hubs, and access points, which help manage and direct data flow.
---
### Subnet
A subnet (short for subnetwork) is a ***smaller, logical subdivision of a larger computer network***. It divides a big network into multiple smaller networks called subnets, each with its own range of IP addresses. This subdivision ***makes the network more manageable and efficient by reducing traffic congestion and improving routing***.

The process of dividing one big network into multiple smaller networks is called **subnetting**.

---

### IP Address and MAC Address
|Features  |IP (Internet Protocol) Address |MAC (Media Access Control) Address |
|----------|-------------------------------|-----------------------------------|
|*Definition*|A unique address assigned to each device on a network at the network (Layer 3) level, used for logical identification and communication between networks|A hardware identifier assigned to a network interface card (NIC) at the physical (Layer 2) level, used for identifying devices within the same local network|
|*Format*|Numeric: IPv4 (e.g., 192.168.1.1), IPv6 (e.g., 2001:0db8:85a3::8a2e:0370:7334)|Hexadecimal: 48 bits, usually shown as 6 pairs (e.g., 00:1A:2B:3C:4D:5E)|
|*Assignment*|Assigned by software (manually or dynamically by DHCP) and can change over time|Burned into hardware by the manufacturer, usually permanent but can sometimes be changed in software|
|*Scope*|Used for communication across interconnected networks (local and global)|Used for communication within a local network segment|
|*Uniqueness*|Unique within a given network/subnet, but may repeat globally|Globally unique to each NIC (ideally never repeats)|
|*Visibility*|Used by routers and networking software|Used by switches and network adapters|

----
### IPv4 and IPv6
IPv4 and IPv6 are two versions of the Internet Protocol, with IPv6 designed to succeed IPv4.
|Features  |IPv4 |IPv6 |
|----------|-------------------------------|-----------------------------------|
|*Address Length* |	32 bits (4 numbers, e.g., 192.168.1.1) | 128 bits (8 segments, e.g., 2001:0db8:85a3::8a2e:0370:7334)|
|*Number of Addresses*|About 4.3 billion |About 340 undecillion (3.4 × 10³⁸)|
|*Address Notation*|Dotted decimal (e.g., 192.168.0.1)|Hexadecimal separated by colons (e.g., 2001:db8::1)|
|*Header Size*|20–60 bytes, variable |40 bytes, fixed|
|*Security*|No built-in security (IPSec optional)|IPSec built-in for encryption/authentication|
|*Fragmentation*|Done by sender and routers|Only by sender|
|*Address Classes*|Present (A, B, C, D, E)|No class concept; all addresses are considered equal|
|*End-to-End Integrity*|Not Achievable | Achievable|

#### Why IPv6?
- IPv6 was developed to overcome the address exhaustion of IPv4, offering a vastly larger address space.
- IPv6 addresses are harder to remember but much more future-proof, accommodating the rapid growth of internet devices.
- IPv6 improves built-in security, header efficiency, and supports new networking features, while eliminating NAT in most scenarios.

---
### TCP and UDP
|Features  |TCP (Transmission Control Protocol) |UDP (User Datagram Protocol) |
|----------|-------------------------------|-----------------------------------|
| *Connection*   | Connection-oriented: establishes a reliable connection before data transfer | Connectionless: sends data without establishing a connection |
| *Reliability*| Reliable: guarantees delivery, error-checking, retransmission of lost data | Unreliable: no guarantee of delivery, minimal error-checking |
| *Order of Data* | Ensures packets arrive in order                        | No guarantee of order; packets may arrive out of sequence |
| *Speed*| Slower due to connection setup, acknowledgments, and retransmissions | Faster: minimal overhead, no need for connection set-up  |
| *Error Checking*| Extensive: error detection, retransmission, acknowledgment | Basic: simple checksum, no retransmission              |
| *Overhead*| Higher (header size 20–60 bytes, more processing)     | Lower (header size 8 bytes, simple processing)           |
| *Data Flow*| Stream-based (continuous flow of data)                | Message-based (data sent as independent packets)         |
| *Use Cases*| Web browsing (HTTP/HTTPS), file transfer (FTP), email, remote administration (SSH) | Streaming (audio/video), online gaming, DNS, VoIP        |
| *Broadcasting*| Not supported| Supported|
| *Congestion Control*   | Yes: uses flow and congestion control mechanisms| No congestion control|


- TCP is ideal when reliable and ordered delivery is crucial (e.g., websites, file downloads, emails).
- UDP is chosen when speed and low latency are more important than reliability (e.g., live video/audio streaming, online games, voice calls).

Both protocols serve vital but different roles in modern networking. TCP prioritizes data integrity, while UDP favors efficiency and speed.
