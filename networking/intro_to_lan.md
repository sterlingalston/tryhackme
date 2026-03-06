### Local Area Network (LAN) Topologies

- "topology", we are actually referring to the design or look of the network at hand. Let's discuss the advantages and disadvantages of these topologies below.
- ![image](.attachments/f32e3d903972d07141bcbf59f87d8caf80cb4ee8.png)

#### Star Topology 

- devices are individually connected via a central networking device known as a _switch_ or _hub_
- information sent to a device is sent via the central device
- more expensive than any other topology, but more scalable
- more it scales, more maintenance is required
- prone to failure, albeit reduced
- if central device fails, nothing will be sent!
- switches don't usually die often, and when they do you can get a better newer one

#### Bus Topology

- relies on single connection known as _backbone cable_
- "leaf off a tree"
- because on cable, prone to slow and bottlenecked if devices are all simultaneously requesting data
- difficult troubleshooting to identify which device is experiencing issues
- easier and cost-efficient/ cabling and network equipment
- little redundancy -- single point of failure on backbone cable
- ![image](.attachments/e4ed59fdd86a2eab7aa1af28aa8a86bb75045c0e.png)


#### Ring Topology

![image](.attachments/db44ea3338dd2cf6b4c3ce98785024cd997f3fd4.png) 

-  ring topology (also known as token topology)
-  Devices such as computers are connected directly to each other to form a loop, meaning that there is little cabling required and less dependence on dedicated hardware such as within a star topology
-  Interestingly, a device will only send received data from another device in this topology if it does not have any to send itself. If the device happens to have data to send, it will send its own data first before sending data from another device.
- traveling in only one direction, fairly easy to troubleshoot any faults
- but has to visit multiple devices first before reaching intended
- less prone to bottlenecks, unlike bus topology; a fault like a cable cut will result in network breaking

### What is a Switch?

- switch - dedicated devices within a network that are designed to aggregate multiple other devices such as computers, printers, or any other networking-capable device using ethernet
- devices plug into switch ports
- usually found in larger networks (businesses, schools, etc)
- ports of 4,8,16...64
- keep track of what devices is connected to which port
  - this is _unlike a hub_ which will send the same packed to every port
  - reduced network traffic

![image](.attachments/97c3448c33e44ce7282b5a40a7c0b0a36c52f336.png) 

### What is a Router?

- a router's job to connect networks and pass data between them. It does this by using routing (hence the name router!).
- _routing_ is the process of data travelling across networks; creating a path between networks so that this data can be successfully delivered

![image](.attachments/74374b4df1e40165438d43747930b4ed3ffb7f9c.png) 