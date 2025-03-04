# Cisco Aufgabe 5


| Device       | Interface  | MAC Address    | Switch Interface |
|--------------|------------|----------------|------------------|
| Router0      | Gg0/0      | 0001.6458.2501 | G0/1             |
|              | S0/0/0     | N/A            | N/A              |
| Router1      | G0/0       | 00E0.F7B1.8901 | G0/1             |
|              | S0/0/0     | N/A            | N/A              |
| 10.10.10.2   | Wireless   | 0060.2F84.4AB6 | F0/2             |
| 10.10.10.3   | Wireless   | 0060.4706.572B | F0/2             |
| 172.16.31.2  | F0         | 000C.85CC.1DA7 | F0/1             |
| 172.16.31.3  | F0         | 0060.7036.2849 | F0/2             |
| 172.16.31.4  | G0         | 0002.1640.8D75 | F0/3             |


Questions and Answers

How many copies of the PDU did Switch1 make?
3 Copies  

---


What is the IP address of the device that accepted the PDU?
Switch Interface F0/1

---

What happened to the source and destination MAC addresses?
The destination MAC address is written in the PDU.  

---

How many copies of the PDU did the switch make during the ARP reply?
Only 1 

---

To what IP address does the MAC address entry correspond?
ARP Table Reference 

---

In general, when does an end device issue an ARP request?
| Internet Address | Physical Address  |
|------------------|------------------|
| 172.16.31.3      | 0060.7036.2849    |

![](Screenshot_1.png)