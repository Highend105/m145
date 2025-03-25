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

interface/bridge/vlan/print
/interface bridge vlan edit number=X tagged

/ip dhcp-server setup