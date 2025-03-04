# Cisco Aufgabe 6

Switch# configure terminal
Switch(config)# hostname S1
S1(config)# exit


S1# configure terminal
S1(config)# line console 0
S1(config-line)# password letmein
S1(config-line)# login
S1(config-line)# exit
S1(config)# exit


S1> enable
S1# configure terminal
S1(config)# enable password c1$c0
S1(config)# exit


S1# config t
S1(config)# enable secret itsasecret
S1(config)# exit


S1# config t
S1(config)# service password-encryption
S1(config)# exit


S1# config t
S1(config)# banner motd "This is a secure system. Authorized Access Only!"
S1(config)# exit


S1# copy running-config startup-config


S1# configure terminal
S1(config)# interface vlan 1
S1(config-if)# ip address 192.168.1.253 255.255.255.0
S1(config-if)# no shutdown
S1(config-if)# exit


S1# configure terminal
S1(config)# ip default-gateway 192.168.0.1
S1(config)# exit


![](Screenshot_1.png)