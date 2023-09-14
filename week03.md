# Week 3 | Network Technologies

## Task 1. View ARP Table


![physical](./images/physical.png)

ARP Table for your primary physical interface (network adapter) on my computer.

The MAC addresses  discovered as “Reachable " is  38-94-ED-11-74-E7

![ArpTable](./images/ArpTable.png)


## Task 2. Draw Network Diagrams

#### a) A switched LAN with one switch and four PCs

Note : Original file has been attached as switched-lan-a.drawio.drawio 

![switched-lan-a.drawio](./images/switched-lan-a.drawio.png)

#### b) A switched LAN that has four PCs connected to one switch, four PCs connected to another switch, and those two switches are connected to a third switch in star topology. In total, there are eight PCs and three switches.

Note : Original file has been attached as switched-lan-b.drawio.drawio 

![switched-lan-b.drawio](./images/switched-lan-b.drawio.png)

## Task 3. Analyse Ping Packet Capture

#### (a) Captured data packets in Wireshark

![packet1](./images/packet1.png)


![packet2](./images/packet2.png)


![packet3](./images/packet3.png)


![packet4](./images/packet4.png)


#### b) Network Diagram

![network_diagram_w3.drawio](./images/network_diagram_w3.drawio.png)


#### c) ARP packets

 ARP packets are used to identify the MAC address for systems's IP address which has been given.

 The ARP request message is broadcasted by the source device to the LAN network and that message will is received by all the other devices in the local network.

#### d) Packet Diagram for the 1st ARP Packet
 Note : 1st ARP Packet diagram original file has been attached as ARPpacketdiagram.drawio 
##### 1st ARP Packet details bellows


![1stARP](./images/1stARP.png)


##### 1st ARP Packet Diagram bellows

![ARPpacketdiagram](./images/ARPpacketdiagram.png)

#### e) The first two ICMP packets


##### 1st ICMP Packet details bellows

* Source : 192.168.56.1
* Destination : 192.168.56.2
* Protocol : ICMP
* Type : ping Echo request(8)
* Length : 74 bytes
* Ethernet : 14 bytes
* IP : 20 bytes
* ICMP : 40 bytes (Data 32 bytes)


![ICMP01](./images/ICMP01.png)


##### 2nd ICMP Packet details bellows

* Source : 192.168.56.2
* Destination : 192.168.56.1
* Protocol : ICMP
* Type : ping Echo reply(0)
* Length : 74 bytes
* Ethernet : 14 bytes
* IP : 20 bytes
* ICMP : 40 bytes (Data 32 bytes)


![ICMP02](./images/ICMP02.png)

#### f) Packet diagram for the first ICMP packet

Note : 1st ICMP Packet diagram original file has been attached as ICMPpacketdiagram.drawio


![1stICMP](./images/ICMPpacketdiagram.png)


## Task 4. Learning Reflection

**List of tools that I have used up to week 03**
1. PowerShell
2. VirtualBox
3. FileZilla Client
4. Wireshark
5. GitHub


I think **GitHub** is the most useful tool outside of the unit. Because it has many features such as  open Source Software, conduct code reviews, resiliency and availability, security, and scalability

## Extra Resources
1. https://afteracademy.com/blog/what-is-arp-and-how-does-it-work/
2. https://learnduty.com/articles/icmp-explained-and-packet-format/
3. https://moodle.cqu.edu.au/mod/page/view.php?id=3361710
