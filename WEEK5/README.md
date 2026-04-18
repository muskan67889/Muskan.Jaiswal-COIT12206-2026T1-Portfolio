Overview
We need 4 linux Host to connect to 1 open swtich. All the hosts are successfullt communicated using ping before VLAN configuration.

## Task 1 Topology
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/topology1.png?raw=true)


## Pinging Host 2 from host 1
1[images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/host2fromhost1.png?raw=true)

## Pinging Host 1 to Host 4
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/host%201to4.png?raw=true)

## We Used
sh  /etc/openvswitch/init.sh  (to open vswitch)
ovs-vsctl set port eth1 tag=491

![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/VSCTL.png?raw=true)

 ## In host 1:
  ![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/host1.png?raw=true)
  
Arp table observation
- Hosts only leared Mac addresses of device within the same VLAN
- NO ARP entries for hosts in different VLANs

## Output of ovs-vsctl show

VLANs sucessfully isolated the network into separate broadcast domains.
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/topology2.png?raw=true)


## Task 2:
In this task we need to configure a router to enable communication between VLANs.
same setup as task 1 we jst need to add one Linux Router to eth0 of switch

![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/topology2.png?raw=true)


ovs-vsctl set port eth0 trunks=[] (switch)
(router)
ip  link add link eth0 name eth0.491 type vlan id 491 
ip  link add link eth0 name eth0.492 type vlan id 492

ip address add 10.10.1.1/24 dev etho.491
ip address add 10.10.2.1/24 dev etho.492

ip link set dev eth0.491 up
ip link set dev eth0.492 up

![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/t2router1.png?raw=true)


Now we are able to ping a host in another network (h1 to h4)
![images](https://github.com/muskan67889/Muskan.Jaiswal-COIT12206-2026T1-Portfolio/blob/main/WEEK5/t2h1toh2.png?raw=true)







