
sh  /etc/openvswitch/init.sh  (to open vswitch)
ovs-vsctl set port eth1 tag=491
ovs-vsctl show






## Pingng host2 from host 1
![images]

1 to 4


  In host 1:







Task 2:

ovs-vsctl set port eth0 trunks=[] (switch)
(router)
ip  link add link eth0 name eth0.491 type vlan id 491 
ip  link add link eth0 name eth0.492 type vlan id 492

ip address add 10.10.1.1/24 dev etho.491
ip address add 10.10.2.1/24 dev etho.492

ip link set dev eth0.491 up
ip link set dev eth0.492 up



Now we are able to ping a host in another network (h1🡪h4)




