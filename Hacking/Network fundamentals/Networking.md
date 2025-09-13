
Networks involve things that are connected. simple as that

A network involve the connection of only two or million of devices, in the case of computers and cyber security

## What is the internet?
It's a gigantic network that involves millions of small networks

The internet in this case is what allows multiple interconnected networks  to communicate between each other, meaning every device is in some way connected to each other
![[Pasted image 20250911204946.png]]
But how do devices know how to communicate between one another?

## Identifying Devices on a Network

Computers identify quite similar to humans

We have:
- Name                  -> can change/another can have it
- Fingerprints    ->is completely unique

Computers:

| id                                     | description                                                                        |
| -------------------------------------- | ---------------------------------------------------------------------------------- |
| **IP** (internet protocol )address     | identify the host on a network [dynamic] \| assigned when connected to a network   |
| **MAC** (Media Access Control) address | public ID [fully static]<br><br>assigned on the factory (in theory global  unique) |

## IP - Internet Protocol
IP allows us to identify a temporary device on a network. Meaning that with can identify a new device with the same IP address

However, they cannot be two similar IP addresses connected at the same time within the same network

IP addresses follow a set of standards known as **protocols**. The backbone of networking and device communication. They force devices to communicate within 'the same language'

Ex:
In the morning, a laptop connects to our network and its then assigned the IP: **192.168.1.1** 

Later on, the laptop is no longer connected, but instead a friend with his cellphones enters the network, its then assigned the same IP: **192.168.1.1** 

### Structure
![[Pasted image 20250911214603.png]]

IP addresses are made of *4* **octets** , each of a value from 0 to 255

Each octet and value patter representing something on its own. For example, **public** and **private** IP's
Example:
![[Pasted image 20250911215953.png]]
These two devices can communicate **between them** using their **private IP's**. Data sent from or to the **internet** will be identified by their shared **public IP** address 

**Public IP** addresses are given with an **Internet Service Provider** (**ISP**) with a monthly fee (the internet bill)
![[Pasted image 20250911220503.png]]

The most common **IP Version** is **IPv4** , this version allowed a total of 50 billion devices. However, as timed passed and more and more devices where added to the internet, we ended up using all IPv4 addresses by 2021.

To fix this issue **IPv6** was developed, allowing more than 340 trillion devices
![[Pasted image 20250911220820.png]]

 
## MAC - Media Access Protocol

Every device that has the feature of connecting to the internet does so thanks to a microchip known as **physical network interface** (a network adapter/wifi card) 

Every **Physical Network Interface device** has its own unique (in theory) **MAC Address** that was assigned in the factory

A **MAC** address is made of **twelve hexadecimal characters** split by groups of two and divided by semicolons. The  first six character represent the company that made the device, and the last 6 is a unique number
![[Pasted image 20250911222123.png]]

Even though MAC addresses are unique they can be faked. Meaning we can make a device identify with the MAC address of another. Leaving potential security issues

## 'ping' Command
The ping command uses **ICMP** (Internet Control Message Protocol) packets to determine the performance of a connection between devices

Ex.
- if a connection exists or is reliable

