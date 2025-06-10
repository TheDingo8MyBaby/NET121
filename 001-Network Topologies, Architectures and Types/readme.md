# 001 - Network Topologies, Architectures and Types

- Topologies
- Three-tier Hierarchical Model
- Collapsed Core
- Spine and Leaf
- Traffic Flows
- Network Topologies, Architectures and Types Review
> Network+ N10-009 Module 1
## Topologies
- Describes the layout of a network
- Determines how devices connect and communicate
- Topologies are either physical or logical
	- Physical - actual physical layout/physical connections between devices on a network
	- Logical - how data moves from one device to another
> *Physical and logical topologies need not be the same*
### Point-to-Point
- Only two nodes on a link
> **Examples;**
	- WAN link between two locations
	- Line-of-sight wireless between two buildings
	- Uplink/trunk link between two switches
	- *Two PCs connected by a crossover cable*
### Star
- Network devices are connected to a central device/node called a hub (can be a switch, WAP, or network hub)
- Nodes communicate across the network by passing data through the hub
> **Also known as;**
	- Hub-and-Spoke
	- Point-to-multipoint (WANs or wireless)
- Advantage:  If one device or link malfunctions, the remainder of network still functions
- Disadvantage:  If the hub fails, the whole network goes down

![Pasted image 20250610112646.png](https://raw.githubusercontent.com/TheDingo8MyBaby/NET121/refs/heads/main/001-Network%20Topologies%2C%20Architectures%20and%20Types/Images/Pasted%20image%2020250610112646.png)
### Mesh
- Nodes are connected to more than one node
	- Redundancy
	- Fault tolerance
- Can be though of as a redundant star
> **Two types of mesh topologies;**
> - Full Mesh:  Every node connects to every other node
	- Full redundancy
	- Expensive, but good for backbone (core) network
> - Partial Mesh:  Some nodes have links to more than one node
	- Is less expensive with less redundancy
	- *Good for devices that connect to backbone network*

![Pasted image 20250610123743.png](https://raw.githubusercontent.com/TheDingo8MyBaby/NET121/refs/heads/main/001-Network%20Topologies%2C%20Architectures%20and%20Types/Images/Pasted%20image%2020250610123743.png)
### Hybrid
- Any combination of the various topologies to create a larger network

![Pasted image 20250610123842.png](https://raw.githubusercontent.com/TheDingo8MyBaby/NET121/refs/heads/main/001-Network%20Topologies%2C%20Architectures%20and%20Types/Images/Pasted%20image%2020250610123842.png)

-----
## Three-tier Hierarchical Model
### What is the Three-Tier Hierarchical Model?
- A network design framework that organizes a network into three logical layers

| **Tier**     | **Description**                                                                                       |
| ------------ | ----------------------------------------------------------------------------------------------------- |
| Core         | - Datacenter Backbone<br>- High-speed switching<br>- Connect to campus core or edge router            |
| Distribution | - VLAN Routing<br>- Policy<br>- Redundancy for Access layer<br>- Traffic aggregation                  |
| Access       | - Connectivity for end devices (clients and servers)<br>- VLAN membership<br>- PoE<br>- Port Security |
### Classic Cisco Three-Tier Model

![Pasted image 20250610124508.png](https://raw.githubusercontent.com/TheDingo8MyBaby/NET121/refs/heads/main/001-Network%20Topologies%2C%20Architectures%20and%20Types/Images/Pasted%20image%2020250610124508.png)
