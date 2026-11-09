# Wireshark SOC Lab – Network Traffic Analysis

![Wireshark](https://img.shields.io/badge/Tool-Wireshark-blue)
![Cybersecurity](https://img.shields.io/badge/Field-Cybersecurity-red)
![Status](https://img.shields.io/badge/Status-Completed-success)

## About This Project

This repository contains my practical exercises and investigations from the NetworkWalks Wireshark SOC Lab.

The purpose of this lab is to develop practical skills in network traffic analysis, packet inspection, identifying suspicious activities, and investigating potential network attacks.

As part of this exercise, I worked as a SOC Analyst investigating unusual traffic targeting a company's web server.

## Lab Information

| Item | Description |
|---|---|
| Lab Number | Lab 3 |
| Lab Title | Identify the Attacker's IP |
| Platform | NetworkWalks |
| Main Tool | Wireshark |
| Field | Cybersecurity / SOC Analysis |
| Recorded Score | 60/100 |

## Objectives

- Capture network traffic using Wireshark.
- Understand different network protocols.
- Analyze TCP, DNS, and ICMP packets.
- Apply Wireshark display filters.
- Investigate suspicious connections.
- Identify the potential attacker's IP address.

## Tools and Technologies

- Wireshark – Network protocol analyzer.
- Windows – Operating system used for the lab.
- TCP/IP – Network communication protocols.
- NetworkWalks – Practical cybersecurity training platform.

## Practical Investigation

### 1. Network Traffic Capture

Captured network packets and examined the communication between different devices.

### 2. Protocol Analysis

Investigated the following protocols:

- TCP – Transmission Control Protocol.
- DNS – Domain Name System.
- ICMP – Internet Control Message Protocol.

### 3. Packet Filtering

Used Wireshark display filters to investigate network communication.

**Example filters:**

Find traffic from a specific source:

```wireshark
ip.src == 192.168.10.20
```

Find traffic going to a specific destination:

```wireshark
ip.dst == 192.168.10.66
```

Identify TCP SYN/ACK packets:

```wireshark
tcp.flags.syn == 1 && tcp.flags.ack == 1
```

Filter communication between two IP addresses:

```wireshark
ip.src == 192.168.10.20 && ip.dst == 192.168.10.66
```

## Screenshots and Evidence

### Packet Capture

![Packet Capture](Lab-3-Identify-Attacker-IP/screenshots/task-1-packet-capture.png)

### Lab Results

![Lab Results](Lab-3-Identify-Attacker-IP/screenshots/lab-results.png)

## Findings

The investigation involved examining network traffic, identifying communication patterns, and filtering TCP connections.

**Final attacker IP:** To be confirmed from the complete lab investigation.

**Attack type:** To be confirmed after completing the investigation.

## Skills Learned

- Network packet analysis.
- Wireshark display filtering.
- TCP connection analysis.
- DNS and ICMP traffic investigation.
- Basic SOC investigation techniques.
- Identifying suspicious network activities.

## Author

**Ukwizagira Jean Bosco**

Cybersecurity Learner | Aspiring SOC Analyst
GitHub: [Ukwizagira Jean Bosco](https://github.com/jean916)

## Disclaimer

This project was completed for educational purposes using the NetworkWalks cybersecurity training environment. All investigations were conducted in an authorized lab environment.