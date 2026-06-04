# Use of OSPF - Multi-Site WAN Lab

## Project Overview

This Packet Tracer lab simulates a fictional company with six branch locations: New York, Florida, Texas, California, Washington, and Illinois.

Each site includes a Cisco 2911 router, a Cisco 2960 switch, and one endpoint PC. The routers are connected using point-to-point WAN links, and OSPF is configured to allow the routers to dynamically learn and advertise routes across the network.

## Objectives

- Configure router hostnames and interfaces using Cisco IOS CLI
- Use /30 subnets for point-to-point WAN links
- Configure /24 LAN networks for each branch site
- Add loopback interfaces for stable OSPF Router ID selection
- Enable OSPF across the routed network
- Verify OSPF neighbor adjacencies
- Confirm dynamic route learning
- Test end-to-end connectivity between PCs

## Technologies Used

- Cisco Packet Tracer
- Cisco 2911 Routers
- Cisco 2960 Switches
- OSPF
- IPv4 Subnetting
- Static endpoint addressing
- Cisco IOS CLI

## OSPF Configuration Used

```bash
conf t
router ospf 1
network 192.168.0.0 0.0.255.255 area 0
end
wr


Verification Commands


show ip interface brief
show ip ospf neighbor
show ip route
show running-config
ping

