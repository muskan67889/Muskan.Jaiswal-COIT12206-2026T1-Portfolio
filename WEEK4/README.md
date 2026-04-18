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

## Testing
I tested connectivity using ping between different subnets hosts and confirmed successful communication through the router.

I learned how routing tables control network traffic and how routers forward packets between different subnets.
