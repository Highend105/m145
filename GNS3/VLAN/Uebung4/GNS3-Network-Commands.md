# Commands für Netzwerk Einrichtung
Folgend sind die Commands für die Einrichtung vom Netzwerk dokumentiert:


/interface vlan
add interface=ether2 vlan-id=10 name=ether2_vlan10
add interface=ether2 vlan-id=20 name=ether2_vlan20
add interface=ether2 vlan-id=30 name=ether2_vlan30


/ip address
add address=192.168.10.1/24 interface=ether2_vlan10
add address=192.168.20.1/24 interface=ether2_vlan20
add address=192.168.30.1/24 interface=ether2_vlan30


/interface bridge port add bridge=bridge1 interface=ether2
/interface bridge vlan set numbers=0 tagged=ether8,ether2 untagged=ether4
interface/bridge/vlan/print


/ip dhcp-server setup