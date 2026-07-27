*This project has been created as part of the 42 curriculum by kmarrero.*

# NetPractice

## Description

NetPractice is a networking project from the 42 curriculum designed to introduce the fundamental concepts of computer networks through a series of practical exercises.

The project consists of 10 progressively more difficult levels where the objective is to correctly configure a virtual network. Each level requires identifying and fixing networking issues by assigning the correct IP addresses, subnet masks, gateways, and routes so that hosts can successfully communicate.

Rather than focusing on command-line configuration, NetPractice emphasizes understanding how networks function and developing the ability to reason about network topology and connectivity.

## Objectives

- Understand IPv4 addressing.
- Learn how subnet masks divide networks.
- Understand how hosts communicate within and across networks.
- Learn the purpose of default gateways.
- Understand the role of routers and switches.
- Develop troubleshooting skills for common network configuration problems.

---

# Instructions

## Running the training interface

Launch the training interface using:

```bash
./run.sh
```

or follow the instructions provided by the project if using the web interface supplied by 42.

## Solving the exercises

Each level presents a network with one or more configuration problems.

To complete a level:

1. Analyze the network topology.
2. Configure the missing or incorrect network parameters.
3. Verify that every required device can communicate correctly.
4. Export the completed configuration.

## Exporting configurations

After successfully completing a level, export the configuration using the interface's **Export** option.

Repeat this process for all 10 levels.

## Submission

The repository must contain:

- This `README.md` file.
- **10 exported configuration files**, one for each completed level.

All exported configuration files must be placed **at the root of the repository** before submission.

Example:

```
README.md
level1.export
level2.export
level3.export
...
level10.export
```

---

# Resources

## Networking Concepts

This project covers the following networking fundamentals:

| Concept | Description |
|---------|-------------|
| **TCP/IP Addressing** | Every device connected to a network requires a unique IP address to communicate. IPv4 addresses are 32-bit numbers typically written in dotted decimal notation (e.g., `192.168.1.10`). |
| **Subnet Mask** | Defines which portion of an IP address identifies the network and which identifies the host. Devices must belong to the same subnet to communicate directly without a router. |
| **CIDR Notation** | A compact way of representing subnet masks using a prefix length (e.g., `/24` instead of `255.255.255.0`). It indicates how many bits belong to the network portion of the address. |
| **Network Address** | The first address of a subnet. It identifies the entire network and cannot be assigned to a host. |
| **Broadcast Address** | The last address in a subnet. Packets sent to this address are delivered to every host on the local network. |
| **Host Address** | Any valid IP address assigned to a device within a subnet. It must be unique inside that network. |
| **Default Gateway** | The router interface that forwards packets to destinations outside the local network. Without a valid default gateway, communication is limited to the local subnet. |
| **Router** | Device responsible for connecting different networks and forwarding packets according to routing information. Routers make communication between separate subnets possible. |
| **Switch** | Device that connects devices within the same local network. It forwards Ethernet frames based on MAC addresses, allowing efficient communication between hosts. |
| **OSI Model** | A conceptual networking model composed of seven layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application. NetPractice mainly focuses on Layers 2 and 3. |
| **Layer 2 (Data Link)** | Responsible for local network communication using MAC addresses. Switches operate primarily at this layer. |
| **Layer 3 (Network)** | Responsible for logical addressing and routing using IP addresses. Routers operate at this layer. |
| **Local Area Network (LAN)** | A network where devices communicate directly without crossing a router, provided they belong to the same subnet. |
| **Routing** | The process of selecting the correct path for packets to reach a destination network through one or more routers. |
| **Packet Forwarding** | The action performed by routers to send packets from one interface to another based on the destination IP address. |
| **Network Troubleshooting** | The process of identifying configuration errors such as incorrect IP addresses, subnet masks, gateways, or routing that prevent successful communication. |

## Official Documentation

- 42 NetPractice subject
- RFC 791 – Internet Protocol (IPv4)
- RFC 950 – Internet Standard Subnetting Procedure
- RFC 1122 – Requirements for Internet Hosts

## Networking References

- Cisco Networking Academy
- Cloudflare Learning Center
- MDN Web Docs – Networking
- IBM Networking Documentation

## AI Usage

Artificial Intelligence was used only as a learning aid.

Specifically, AI was used to:

- Clarify networking concepts.
- Explain subnetting and IP addressing.
- Review theoretical questions.
- Improve the project's documentation.
- https://www.youtube.com/@PowerCertAnimatedVideos

The network configurations and solutions submitted for each level were completed manually after understanding the underlying networking concepts.

---

## Skills Developed

- Logical problem solving
- Network analysis
- IPv4 subnetting
- Basic routing concepts
- Reading network diagrams
- Understanding communication between hosts
- Diagnosing network connectivity issues

---
