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
