# Lab 01: Two LANs Connected by One Router

## Goal
Connect two separate networks through a single router and confirm devices on different LANs can communicate.

## Topology
1 router, 2 switches, 4 PCs. See topology.png.

## IP Addressing
| Device | Interface | IP Address | Gateway |
|--------|-----------|------------|---------|
| Router0 | Gi0/0 | 192.168.1.1 | - |
| Router0 | Gi0/1 | 192.168.2.1 | - |
| PC0 | NIC | 192.168.1.10 | 192.168.1.1 |
| PC2 | NIC | 192.168.2.10 | 192.168.2.1 |

## Result
PC0 successfully pinged a PC on the other LAN. See ping-test.png.

## Problem I fixed
A PC was using the router's IP address, which caused a duplicate address conflict and 100% packet loss. Giving each device a unique IP fixed it.

## Tools
Cisco Packet Tracer
## Topology
![Topology](Screenshot%20(275).png)

## Ping Test
![Ping test](Screenshot%20(276).png)

## Router Configuration
![Router config 1](Screenshot%20(277).png)
![Router config 2](Screenshot%20(278).png)
