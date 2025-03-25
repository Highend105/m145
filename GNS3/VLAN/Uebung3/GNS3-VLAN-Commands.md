# Commands für VLAN Einrichtung
Folgend sind die Commands für die Einrichtung von VLANs bei MikroTik Switches dokumentiert:

 - /interface bridge add name=bridge1 protocol-mode=none vlan-filtering=yes
 - /interface bridge port add bridge=bridge1 comment="VLAN 10 - IT" frame-types=admit-only-untagged-and-priority-tagged hw=no interface=ether2 pvid=10
 - /interface bridge port add bridge=bridge1 frame-types=admit-only-vlan-tagged hw=no interface=ether8
 - /interface bridge vlan add bridge=bridge1 comment="VLAN 10" tagged=ether8 untagged=ether2 vlan-ids=10