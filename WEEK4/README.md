In this Tuitorial We learned how routing works in Linux and how to view routing tables and enables forwarding

## Overview
I created a GNS3 project called Views-routes-[12315138]. In this I added 3 Linux hosts, 1 Linux router and ! switch. The network was divided into two subnets. I configured static IP addresses for all devices and enabled communication between the two networks.

## Configuration
-Hosts were assigned IP addresses in two different subnets
-Router had IP addresses on both interfaces

-Forwarding was enabled on the router using:

sysctl net.ipv4.ip_forward=1

-Forwarding was disabled on all hosts:

sysctl net.ipv4.ip_forward=0

Command Uses were (ip route show) and (sysctl next.ipv4.ip_forward)

## Topology
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK4/topology.png?raw=true)


## Testing
I tested connectivity using ping between different subnets hosts and confirmed successful communication through the router.

I learned how routing tables control network traffic and how routers forward packets between different subnets.

I imported the OSPF template project and started all nodes. I waited for FRR routers to fully boot.No manual configuration was required because IP addresses and OSPF were already set.

Commond Used:
show ip route
traceroute <destination IP>

While testing I observed routing tables and neighbor relationships between routers. I used traceroute to check the path between the hosts. OSPF automatically recalculated a new path.

I learned how OSPF automatically updates routing paths when a link fails and how routers dynamically find the best route in a network.

## Reflection 
This week helped me understand how routing works in both static and dynamic networks. I learned how routers forward packets between subnets and how OSPF automatically updates routes when network changes occur.

