# Week 4 | Internetworking

## Task 1. View Routing Table

I used Get-NetRoute -InterfaceIndex 8 powershell command to view the routing table for the network adapter on my own computer. The routing table is listed below.

![RoutingTable](./images/RoutingTable.png)

##### Description of rows in the routing table 

1. 255.255.255.255/32 - Send direct
2. 224.0.0.0/4 - Send direct
3. 10.0.0.255/32 - Send direct
4. 10.0.0.11/32 - Send direct
5. 10.0.0.0/24 - Send direct
6. 0.0.0.0/0  - send to 10.0.0.1                                                                                                                                                                                    

## Task 2. IP Network Design

(a)

Note: I did this part by myself without partner.

IPv4 Addressing:

LAN 1: 29.30.1.0/24

LAN 2: 28.40.1.0/24

WAN: 10.1.1.0/30


| Device Name  | Interface | IPv4 Address  | Subnet Mask |
| ------------- | ------------- | ------------- | ------------- |
| PC1  | LAN 1  | 29.30.1.2  | 255.255.255.0 |
| PC2  | LAN 1  | 29.30.1.3  | 255.255.255.0 |
| PC3  | LAN 1  | 29.30.1.4  | 255.255.255.0 |
| PC4  | LAN 2  | 28.40.1.2  | 255.255.255.0 |
| PC5  | LAN 2  | 28.40.1.3  | 255.255.255.0 |
| Router 1  | LAN 1  | 29.30.1.1  | 255.255.255.0 |
| Router 1  | WAN  | 10.1.1.1  | 255.255.255.252 |
| Router 2  | LAN 2  | 28.40.1.1  | 255.255.255.0 |
| Router 2  | WAN  | 10.1.1.2  | 255.255.255.252 |

(b)
Note : Network Diagram original file has been attached as Taskb.drawio

[Taskb.drawio](./images/Taskb.drawio.io)

![Taskb.drawio](./images/Taskb.drawio.png)



(c)

Router 1:
| Destination  | Next Hop |
| ------------- | ------------- |
| 29.30.1.0/24  | direct  |
| 28.40.1.0/24  | 10.1.1.2  |
| 10.1.1.0/30  | direct  |
| 0.0.0.0/0  | 10.1.1.2  |

Router 2:
| Destination  | Next Hop |
| ------------- | ------------- |
| 29.30.1.0/24  | 10.1.1.1  |
| 28.40.1.0/24  | direct  |
| 10.1.1.0/30  | direct  |
| 0.0.0.0/0  | 10.1.1.1  |


## Task 3. IP Address Lookup

Two difffernt online IP address lookup websites give different IP adddress as 220.240.202.42. But my real IP address is 10.0.0.11.
However, its identyfy location correctly.

Test 01

![googlip](./images/googlip.png)

Test 02

![iplokup](./images/iplokup.png)

My real IP addrsss in my laptop. 

![MyIP](./images/MyIP.png)


