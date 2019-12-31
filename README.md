
Multilocation Enterprise Network Design Using Cisco Packet Tracer

Design and implement a multi-location, inter-networking strategy for a small and stable organization. This organization currently has 5 locations. Corporate headquarters is located in Boston and Mumbai. The company is placed at 3 other locations, which are New York, London and Beijing. Design your network considering following constraints.

• Every office should have the 250 employees with 85% of redundancy (For IP addresses).
• You are provided 192.168.xx.0/19 (xx = put last two digits of the NUID) network for your entire organization.
• Use Subnetting to provide network within the above given range.
• Boston and Mumbai offices have Finance, HR and Technical departments.
• Other locations have HR and Technical departments.
• All the IP addresses inside departments should be assigned by DHCP server.
• The DHCP server for the Boston and Mumbai is present in the Boston’s Technical department and for other 3 locations DHCP server is present in Mumbai’s technical department.
• Finance departments shouldn’t be accessed by any other departments, but Finance can access any other department.
• Two Finance departments can access each other.
• All other departments should be able to access each other

Project Design
• High level diagram consisting of basic network infrastructure
• Mention routers, switches, access points, servers and workstations
• Finding out the cost of network equipment along with the Model No. and count of devices
• Consider geographical locations while designing your network.
• Use OSPF as the routing protocol. There are 5 offices, implement the area concept of OSPF and configure every office in separate area for example: Boston-Area 1, Mumbai- Area2, Beijing- Area3, London-Area 4 and New York- Area5 and Backbone network as area 0.
• Set the router ID manually in each OSPF routers.
• Implement HSRP for Boston and Mumbai office. Change the Hello timer to 2s, hold timer to 6s.
• Implement VLAN’s for each department. Set only the VLANs used in the Networks as the VLANs allowed on trunk.
• Change the Native VLAN on the Trunk to the one used for HR department.
• Implement Rapid STP and switch redundancy for London and New York office.
• Enable Port fast and BPDU guard on all the ports that are connected to the host machine.
• Implement Frame Relay to improve the data rate.
• Defend MAC flooding attack in the HQ locations
• Area Border Router (ABR) in Boston can access all other locations ABR but not reverse. A technical department from Boston alone has an access to ABR of Boston

• Implement a multi-layer switch in the Beijing location, this multilayer switch should carry inter-VLAN routing.
• Configure EtherChannel with LACP as the protocol on NY.
