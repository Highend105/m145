# Aufgabe 10 - Cisco

### 1. Wenn ein PC in VLAN 10 eine Broadcast-Nachricht sendet, welche Geräte empfangen sie?

Nur Geräte in VLAN 10 (**PC1, PC4, PC7**) erhalten die Broadcast-Nachricht.  
Switches leiten Broadcasts nicht über VLAN-Grenzen hinweg weiter.

### 2. Wenn ein PC in VLAN 20 eine Broadcast-Nachricht sendet, welche Geräte empfangen sie?

Nur Geräte in VLAN 20 (**PC2, PC5, PC8**) erhalten die Broadcast-Nachricht.

### 3. Wenn ein PC in VLAN 30 eine Broadcast-Nachricht sendet, welche Geräte empfangen sie?

Nur Geräte in VLAN 30 (**PC3, PC6, PC9**) erhalten die Broadcast-Nachricht.

### 4. Was passiert, wenn ein PC in VLAN 10 eine Nachricht an einen PC in VLAN 30 sendet?

Das Frame wird vom Switch verworfen, da VLANs den Layer-2-Verkehr isolieren.  
Ohne einen Router (Layer-3-Gerät) ist keine Kommunikation zwischen VLANs möglich.

### 5. In Bezug auf die Ports: Was sind die Kollisionsdomänen auf dem Switch?

Jeder Switch-Port ist eine eigene Kollisionsdomäne.  
(Heutige Switches arbeiten im **Full-Duplex-Modus**, sodass Kollisionen selten sind, aber technisch gesehen bleibt jeder Port eine eigene Kollisionsdomäne.)

### 6. In Bezug auf die Ports: Was sind die Broadcast-Domänen auf dem Switch?

Jedes VLAN bildet eine eigene **Broadcast-Domäne**:

- **VLAN 10** = 1 Broadcast-Domäne  
- **VLAN 20** = 1 Broadcast-Domäne  
- **VLAN 30** = 1 Broadcast-Domäne  

Ohne VLANs wäre der gesamte Switch eine einzige **Broadcast-Domäne**.