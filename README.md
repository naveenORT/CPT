
Multilocation Enterprise Network Design Using Cisco Packet Tracer

Designed and implemented a multi-location, inter-networking strategy for a small and stable organization. This organization currently has 5 locations. Corporate headquarters is located in Boston and Mumbai. The company is placed at 3 other locations, which are New York, London and Beijing 

• Every office  has 250 employees with 85% of redundancy (For IP addresses).
• Boston and Mumbai offices have Finance, HR and Technical departments.
• Other locations have HR and Technical departments.
• All IP addresses inside departments are assigned by DHCP server.
• The DHCP server for the Boston and Mumbai is present in the Boston’s Technical department and for other 3 locations DHCP server is present in Mumbai’s technical department.
• Finance departments will be accessed by any other departments, but Finance can access any other department.
• Two Finance departments can access each other.
• All other departments should be able to access each other
• Used OSPF as the routing protocol. There are 5 offices, implement the area concept of OSPF and configure every office in separate area for example: Boston-Area 1, Mumbai- Area2, Beijing- Area3, London-Area 4 and New York- Area5 and Backbone network as area 0.

• Implemented HSRP for Boston and Mumbai office. Change the Hello timer to 2s, hold timer to 6s.
• Implemented VLAN’s for each department. Setted VLANs used in the Networks as the VLANs allowed on trunk.
• Changed the Native VLAN on the Trunk to the one used for HR department.
• Implemented Rapid STP and switch redundancy for London and New York office.
• Enabled Port fast and BPDU guard on all the ports that are connected to the host machine.
• Implemented Frame Relay to improve the data rate.
• Defended MAC flooding attack in the HQ locations
• Area Border Router (ABR) in Boston will access all other locations ABR but not reverse. Technical department from Boston alone has an access to ABR of Boston

• Implemented a multi-layer switch in the Beijing location, this multilayer switch should carry inter-VLAN routing.
• Configure EtherChannel with LACP as the protocol on NY.
