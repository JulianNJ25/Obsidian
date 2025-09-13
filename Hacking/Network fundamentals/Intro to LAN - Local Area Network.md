# LAN Technologies
## "Topology" in Networking
*Topology*: The design or look of the network at hand

## Start Topology
![[Pasted image 20250912192510.png]]
Devices are individually connected via a **central networking device** such as a **switch** or a **hub**. 

The most commonly used thanks to **reliability** and **scalability**. But its the most **expensive**

## Bus Topology
![[Pasted image 20250912192848.png]]
**Single connection** known as a **backbone cable**

Where devices (**leaves**) stem from branches of the main cable

Prone to becoming **slow** and **bottlenecked** if multiple devices are requesting data at the same time

**Easiest** and **cost-efficient**

Data is sent both **left** and **right** from a leaf
## Ring topology
![[Pasted image 20250912223531.png]]
Also known as **token topology**. In where multiple devices are connected directly to each other in a loop

Data is send across the loop until it reaches the destined device, hopping from device to device.

If a device within the loop needs to send data, it will send its own data before sending data from another device that it might have received right before

Less prone to bottlenecks, but if a single cable or device gets broken, the whole loop breaks. Meaning, the whole network goes down

##  Switch
A switch is a middle device within a network, allows multiple devices to connect to it through an **Ethernet cable** into a **switch port**

They **keep track of what device is connected to which port**. This help send packaged directly to the **intended target**, thus reducing network traffic
![[Pasted image 20250912224921.png]]
As the graphic shows, **switches and routers can be connected to one another** 

This increases **redundancy** (reliability) of a network. As **data can take many paths**

If a path is down, it can take another

##  Router
Routers **connect networks and pass data between them** through routing

**Routing** is the process of **data travelling across networks**. Involves creating a **path** between networks, and ensure data transfer
![[Pasted image 20250912231656.png]]

# Subnetting
Networks can be of any size, smaller networks don't even need complex management. But a big enterprise might need more organization.

Subnetting **splits up** a network into smaller pieces, creating **smaller networks in a network** 

A network is like a cake, its of limited space, but everyone in the function can have a piece
![[Pasted image 20250912235001.png]]
Ex: We need to send information to a specific computer in the Accounting Department

### How can we subnet?
**Subnet mask**:
Subnetting is achieved by **splitting up the number of hosts** that can fit the network represented by a number called **subnet mask**

Represented as a **number of 4 bytes (32 bits)** ranging from **0 to 255**. Just like the IP

However, its **NOT the same as the IP** though they might look the same. **IPs** are **tied** to a specific device directly; **Subnet mask** is **not tied** to a specific device, but a **portion of the network**

Subnets use IP addresses in three different ways:
- Identify the network address
- Identify the host address
- Identify the default gateway
![[Pasted image 20250913082709.png]]

#### Why its important?
- Efficiency 
- Security
- Full control
Ex: A Cafe has **two** networks, one for **employees** and one for the **general public** that way employees can have control over cashiers and administration functionalities, while customers can browse the net

# ARP - Address Resolution Protocol
Allows devices to identify themselves on a network

Its what makes **a MAC address associate with an IP address**. Each device on the network will keep a a **log of the MAC addresses associated with other devices**

