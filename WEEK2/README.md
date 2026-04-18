## Task1
To learn different ways of setting static IP addresses in Linux using GNS3.
What I did:
I created a GNS3 project called Setting-IP-[12315138]. I added 4 Linux hosts and 1 switch and connected them in a LAN using the network 10.1.1.1/24.
I set IP addresses using three methods:
Host 1 and Host 2: Used GNS3 Configure menu to assign static IPs
Host 3: Edited /etc/network/interfaces file and restarted networking
Host 4: Used command ip address add to set IP manually

Command I used was ip address show

## Result
All four hosts were successfully assigned IP addresses and verified using the command above.

## Learned
I learned different ways to configure IP addresses and the difference between permanent and temporary IP settings.

## Task 2: Testing Network Connectivity and Delay with Ping

To test network connectivity and measure delay using the ping command.
What I did:
Pinged Host B from Host A:
ping -c 5 10.1.1.X
Result: Successful connection and RTT (round-trip time) was displayed.
Pinged a wrong IP address:
ping 10.1.1.999
Result: No response and packet loss was shown.
Ping with options:
ping -c 3 -s 80 -i 2 10.1.1.X
Result: Changed packet count, size, and interval and observed different results.
