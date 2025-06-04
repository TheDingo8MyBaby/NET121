# Networking Concepts
> Network+ N10-009 Module 1
## Topics
- Networking Overview
- OSI and DOD Model
- Networking Appliances, Applications and Functions
- Ports, Protocols, Services and Traffic Types
- Wireless Transmission Media
- Wired Transmission Media and Transceivers
- Network Topologies, Architectures and Types
- IPv4 Network Addressing
- Modern Network Environments

-----
## Networking Overview
### What is a Network?
- Two or more computers connected together
- The computers can be any type of computing device
- The connection can be wired or wireless
### Why have a Network?
- Share data
- Remote communication
- Share resources
	- Data
	- Files
	- Services
	- Printers
- Distribute a computing workload
	- Sensor - Monitor
	- Client - Server
	- Multiple facilities working together
- Cost effectiveness and reliability
### How Computer Communicate on a Network
- Both Sides Need:
	- Applications that want to talk to each other
	- Common Protocol (TCP/IP)
	- Network Interface to connect to network
	- Transmission Media (Wired or Wireless)
### Client / Server Model
- 1 Device wants a service, while 1 Device wants to offer the service
	- Usually a dedicated computer acts as the Server
- Client initiates the connection
- Server waits for clients to connect
	- Can accept or reject the connection attempt
	- Usually based on if the server offers the service the client is asking for
- "Client" and "Server" can refer to:
	- The device itself
	- A process on the device

-----
## Common Terminology
### IP Address
- A number that identifies a node on the network
	- Analogous to a phone number
- Can be changed
	- User configures a different address in network settings
	- Device automatically obtains a new address when connected to a different network
- A device can have more than one IP address
	- One per interface
	- Alternate IP addresses on the same interface
- Each IP address must be unique on the network so there is no conflict
> Examples: IPv4 - `192.168.1.10`  |  IPv6 - `2601:140:8780:43f0:2d1e:9ebb:92f0:d6e9`
### MAC Address
- The physical address of the network interface
	- Also known as the "Burned In Address" (BIA)
	- Does not change
		- The operating system can temporarily override it
- Assigned by the NIC (Network Interface Card) vendor
- One per interface
- Analogous to a cell phone MEID or IMEI number, or a device serial number
> Examples: `BC-85-56-F3-13-02`  |  `BC:85:56:F3:13:02`  |  `BC85.56F3.1302`
### Source and Destination
- Source is the node that is transmitting/sending at that moment
- Destination is the intended recipient of the transmission
- A Client and Server take turns transmitting to each other
	- Thus they alternate between being source and destination
### Protocol
- Set of rules or "language" for communication
- Can exist at any level/layer of networking
- A host will use several protocols to make a connection on the network
### Port
- A number that represents an application (process) on the network
	- From `0 - 65535`
		- `0 - 1023` - Used by well-known services
		- `1024 - 49151` - "registered" (requested) by a service
		- `49152 - 65535` - assigned to client applications like browsers, file and print clients, database clients, etc...
- Assigned by the operating system
	- Can be requested by the service / application
- Every process (both client and server) that accesses the network has its own unique port number on that device
	- You cannot have two processes share the same port on the same IP address
> Example: ![[Pasted image 20250604134459.png]]
### Socket
- A socket is a port that is in use
- It is a combination of protocol, IP address, and port
- This combination uniquely identifies the connection on the network
> Example: ![[Pasted image 20250604134744.png]]

-----
## Networking Overview Review
### Review
- Networking requires four basic components:
	- An application that needs to use the network
	- A protocol to use on the network
	- A network interface to connect to the network
	- Some kind of wired or wireless transmission media
- A port is a number that represents a process on the network
- Server processors listen for incoming connections on well known port numbers
- Client processes are assigned a temporary port by the operating system so they can make connections to servers
- Source is the device that is transmitting at that moment
- Destination is the device that is receiving at that moment
- A client and the server take turns being source and destination as they communicate
- An IP address is a logical address that is temporarily assigned to a device on the network
- A MAC address is the physical address that is "Burned In" to the network interface by the manufacturer
- A socket is a port in use - a combination of IP address, protocol (TCP or UDP), and port
