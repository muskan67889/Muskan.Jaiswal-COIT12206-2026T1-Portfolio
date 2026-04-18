Task 1: ARP (IP to Hardware Address Mapping)

I was working on a task where I had to learn about ARP. to find each others  address ARP is used by devices, which are also called MAC addresses.

When I first looked at the ARP table on Host A it was almost empty. This was because Host A had not communicated with any devices yet.

Then I pinged Host B from Host A. After then I checked the ARP table on Host A again. In table I saw an entry. This entry had the IP address of Host B and its MAC address.

The ARP table also shows a status of the device like "REACHABLE" which in simple terms means the device is working, active and has successfully communicated with it recently recently.

Later Host C pinged Host A. I checked the ARP table on Host A again. Found another new entry for Host C.

This helped me understand that ARP tables get updated automatically when devices communicate with each other. If a device does not communicate for some time its entry can be removed from the ARP table.

So I learned how IP addresses are mapped to hardware addresses in a network using ARP.

Task 2: Default Gateways and Routing

In another task I had to create a network with two subnets. These subnets were connected using two routers.

Each subnet had two hosts connected to a switch. The two routers were connected to each other.

I gave IP addresses to all the devices in the network. I also configured the default gateways on the hosts.

In simple words, the default gateway is important because it tells a host where to send the data when it needs to communicate with devices outside its local network.

I also have enabled the IP forwarding on the routers. This allowed them to pass traffic between the two networks.

I did not enable the IP forwarding on the hosts because they do not need to route traffic.

After setting up the network I checked the routing tables. I used the ping command to test the network.

I was able to ping from one subnet to another. This showed that the routing was working correctly.

So I learned how default gateways and routers help devices, in networks communicate with each other.
 
 ## Topology
 ![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/week%206%20muskan.png?raw=true)
 ## Host1
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/host1.png?raw=true)
## Host2
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/host%202.png?raw=true)
## Host3
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/host%203.png?raw=true)
## Host4
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/host%204.png?raw=true)
## HostA
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/host%20A.png?raw=true)
## HostB
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/Host%20B.png?raw=true)
## HostC
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/host%20C.png?raw=true)
## HostD
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/host%20D.png?raw=true)
## Router1
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/router%201.1.png?raw=true)
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/router%201.png?raw=true)
## Router2
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/router%202.png?raw=true)
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK6/router%202.png?raw=true)

