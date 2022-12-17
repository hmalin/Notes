

The OSI Networking Reference Model


# A brief history.

The Open Systems Interconnection (OSI) reference model is a conceptual model with two major components. The first main component of the OSI networking reference model is an abstract model of networking—a seven-layer model. The second is a set of specific protocols, which allow differing computing systems to communicate with one another despite their different architectures.

## Why a networking model was required.

A networking model was required because early networks communicated using proprietary languages. Because of their proprietary languages, early networks could only communicate with like systems, so an IBM network could only communicate with another IBM network. In addition to that, the U.S. government desired a robust computer communications system that could survive disasters.

#### Highlights:

●      Early networks could only communicate with like systems.

●      The U.S. government desired a robust computer communications system that could survive disasters.

## TCP/IP reference model.

The first networking reference model that was developed was the TCP/IP (Transmission Control Protocol/Internet Protocol) reference model. The TCP/IP reference model was published as the standard for the U.S. Department of Defense (DoD) in 1982. All of the major system manufacturers adopted the TCP/IP reference model beginning in 1984. AT&T moved the UNIX implementation of TCP/IP to open source in 1989, further cementing TCP/IP's place in networking.

#### Highlights:

●      The TCP/IP model was published as the U.S. DoD standard in 1982.

●      Adopted by the big players beginning in 1984.

●      AT&T moved the UNIX implementation to open source in 1989.

## OSI reference model.

The OSI reference model was developed a year later than the TCP/IP reference model. The OSI model was published in 1983 and it defines the relationships between differing protocols and hardware.

#### Highlights:

●      The OSI model was published in 1983.

●      The OSI model defines the relationships between differing protocols and the relationship between protocols and hardware.

# Networking reference models.

## The OSI networking reference model.

While all networks rely upon the TCP/IP reference model, the OSI reference model is more commonly used for troubleshooting and for describing how networks operate. The reason for this is that the seven layers of the OSI model make it easier to break down the function and operation of both the protocols and hardware that make up networks. A brief description of each of the seven layers follows.

### Layer 1, the physical layer.

Layer 1, the physical layer, standardizes the electrical signals that networks use. It also defines cable standards and how the bits of data are placed on the physical media. Network cables and hubs are part of Layer 1 of the OSI model.

#### Highlights:

●      The physical layer standardizes the electrical signal that networks use; it also defines cable standards and how bits are placed on the physical media.

●      Network cables and hubs are part of Layer 1.

### Layer 2, the data link layer.

Layer 2, the data link layer, is responsible for identifying the individual nodes—both the sending node and the receiving node. It also introduces an error correction method known as the frame check sequence (FCS). Layer 2 is composed of two sublayers. The first of those is the logical link control (LLC) layer, which is mainly responsible for flow control and error correction. The second is the media access control (MAC) layer, which is mainly responsible for node addressing. Switches and bridges are Layer 2 devices.

#### Highlights:

●      The data link layer is responsible for identifying the individual nodes; it also introduces an error correction method known as the FCS.

●      Layer 2 is composed of two sub-layers:

○      The LLC layer is mainly responsible for flow control and error correction.

○      The MAC layer is mainly responsible for node addressing.

●      Switches and bridges are Layer 2 devices.

### Layer 3, the network layer.

Layer 3, the network layer, is responsible for routing functions between networks. It also identifies networks and nodes on the network. Routers are Layer 3 devices.

### Highlights:

●      The network layer is responsible for routing functions between networks and it defines node and network addresses.

●      Routers are Layer 3 devices.

### Layer 4, the transport layer.

Layer 4, the transport layer, is responsible for breaking the data into smaller pieces for the lower layers and for the actual data transport protocols—two of which are TCP (Transmission Control Protocol) and UDP (User Datagram Protocol). The transport layer may be required to confirm the actual delivery of the data stream and it may be required to offer error correction. If so, it does this through the use of TCP.

#### Highlights:

●      The transport layer is responsible for breaking the data into smaller pieces for the lower layers and for the actual data transport protocols.

●      The two most common Layer 4 protocols are TCP and UDP.

●      TCP offers both packet delivery confirmation and error control.

### Layer 5, the session layer.

Layer 5, the session layer, is the layer that is responsible for establishing the initial parameters between two systems. It sets up and tears down the communication channel. 

#### Highlights:

●      The session layer is responsible for establishing the initial parameters between two systems.

●      Layer 5 sets up and tears down the communication channels.

### Layer 6, the presentation layer.

Layer 6, the presentation layer, is responsible for taking data and converting it from a machine-dependent language to a machine-independent language. This is also the layer that has the main responsibility for encryption between networks.

#### Highlights:

●      The presentation layer is responsible for taking data and converting it from a machine dependent language to a machine independent language.

●      Layer 6 is also the layer with the main responsibility for encryption between networks.

### Layer 7, the application layer.

Layer 7, the application layer, is the layer that is responsible for the protocols that request services or functions from other systems. These protocols may not be the actual application. For instance, Internet Explorer is an application that uses HTTP at Layer 7 to request Web pages.

#### Highlights:

●      The application layer is responsible for the protocols that request services or functions from other systems.

●      The protocols may not be the actual application.

## TCP/IP reference model.

The TCP/IP reference model is a four-layer reference model that was designed to meet the requirements of the U.S. DoD standards for a robust network communication system. All networks that communicate with other networks rely upon the TCP/IP reference model. The four layers that comprise the model are discussed below.

### Network interface layer (a.k.a. Link layer).

The lowest layer is the Network interface layer, which is also known as the Link layer. It handles electrical signaling, flow control, error detection, and node addressing. This layer can be mapped to Layer 1 and Layer 2 of the OSI reference model.

#### Highlights:

●      The Network interface layer handles electrical signaling, flow control, error detection, and node addressing.

●      This layer maps to Layer 1 and Layer 2 of the OSI reference model.

### Internet layer.

The Internet layer handles routing functions and identifies network systems and nodes on those networks. This layer can be mapped to Layer 3 of the OSI reference model. 

#### Highlights:

●      The Internet layer handles routing functions and identifies network systems and nodes.

●      This layer maps to Layer 3 of the OSI reference model.

### Transport layer.

The Transport layer handles breaking the data into more manageable pieces for the lower layers. It is also the layer that is responsible for the delivery method—which can be either reliable or unreliable. When reliable delivery is used, the Transport layer also handles error correction. This layer maps to Layer 4 of the OSI reference model.

#### Highlights:

●      The Transport layer handles breaking the data into more manageable chunks for lower layers.

●      It is the layer responsible for the delivery method, either reliable or unreliable, and error correction for reliable delivery.

●      This layer maps to Layer 4 of the OSI reference model.

### Application layer.

The Application layer handles requests for services from applications. It also handles translation to machine-independent languages and encryption. Additionally, the Application layer sets up and tears down communication sessions between systems. This layer maps to the top three layers of the OSI model (Layer 5, Layer 6, and Layer 7).

#### Highlights:

●      The Application layer handles requests for services from applications, translation to machine independent languages, and encryption.

●      It also sets up and tears down sessions.

●      This layer maps to Layer 5, Layer 6, and Layer 7 of the OSI reference model.

# OSI and TCP/IP comparison.

While TCP/IP is the dominant model, most technicians communicate issues using the OSI reference model because it allows them to be more specific. When problems occur—and they will—it is easier to resolve them with a more highly defined set of specifications (e.g., Layer 5 of the OSI model vs. the Application layer of the TCP/IP model).

Both the OSI and TCP/IP models are references only. It is not mandatory that they be followed. Each developer and manufacturer determines its own method of implementing the reference model. While, in theory, there will never be a problem in communication between devices and systems, it is only a theory.

# What was covered.

## A brief history.

The OSI and TCP/IP networking models were created to allow disparate systems and networks to communicate easily between each other.

## Networking reference models.

The OSI reference model has seven layers: physical, data link, network, transport, session, presentation, and application. The TCP/IP reference model has four layers: Network interface, Internet, Transport, and Application.

## OSI and TCP/IP comparison.

TCP/IP is the dominant model in use; however, the OSI model is more commonly used when discussing problems. Both models are references only; developers and manufacturers determine their own methods of implementing network models


Mac address – operates at layer 2 the data link layer and is a unique identifier of the network interface.

Ip address- logical address that operates at layer 3 network layer

Switch – layer 2, learns mac addresses and stores them in the cam table, forwards, or floods data

Router – operates at layer 3 logical addressing is the gateway between networks.

Access Point- sends data over rf channels follows 802.11 standard.

Firewall – a firewall is used for network security; it monitors incoming and outgoing traffic and either allows or blocks data based on rules set. Operates at layer 3.

DHCP – dynamic host configuration protocol – dhcp server hands out ips to devices.

DHCP Process – DORA -> DHCP Discover -> DHCP Offer <-   DHCP Request -> 
<-DHCP Acknowledge.

TCP- transport control protocol – reliable communication, 3 way handshake syn  syn/ack ack messages 

UDP – user datagram protocol – Unreliable faster used for voip or video

Ssh – secure shell protocol port 22 secure remoting protocol. - encrypted

telnet – port 23 unsecure remoting protocol – credentials can be captured via Wireshark an shown in clear text. 

VLAN – Virtual lan – isolated section within a network, layer2 A VLAN automatically limit access to a specified group of users by dividing workstations into different isolated LAN segments.

DNS- Domain name system is essentially the phonebook of the internet, dns translates domain names to ip addresses for us so we do not have to memorize every unique ip address.

ACL-access control list - a set of rules that is usually used to filter network traffic. ACLs can be configured on network devices with packet filtering capabilities, such as routers and firewalls.

Subnet – subdivision of an ip network. The main purpose in using subnets is to relive network congestion used to be a larger problem back in the day when hubs where used rather than switches.

Osi model: open standard interconnect– 7 layers- used as a guide for troubleshooting

Away- Application- provides network services to application

Pizza- Presentation – formats data to be presented, encrypts data

Sausage –Session layer maintains session between sender and receiver.

Throw – Transport – port numbers. Tcp ,udp



TCIP model:

Application Layer – (OSI model application , presentation ,session  layers.)

Transport Layer- (OSI model transport Layer)

Internet Layer (OSI Model network layer)

Network interface Layer /Link layer - (OSI model Data link layer and Physical layer.)

ARP- Address resolution protocol – discovers mac address using arp requests “who is 10.1.1.0 ?” “ hey im 10.1.1.0” here is my mac xx xx xx bc “  at layer 2

CDP – cisco discovery protocol used to find directly connected cisco devices on a network. Cisco specific (sh cdp neighbors-) (CDP operates at Layer 2 only. )

LLDP- link layer discovery protocol – non cisco specific protocol used to find other directly connected network devices

STP – Spanning tree protocol. Used in redundant networks to identify which links are redundant links and shutting them down to avoid network loops.

Root bridge - The root bridge function is only for the spanning tree protocol. The root bridge should be the center of the network. The other switches/bridges refer to the root bridge to find redundant paths, so no Layer 2 Loops exist. The switch with the lowest BID becomes the Root Bridge. Since the BID starts with the Bridge Priority field, essentially, the switch with the lowest Bridge Priority field becomes the Root Bridge. If there is a tie between two switches having the same priority value, then the switch with the lowest MAC address becomes the Root Bridge.

BPDU- Bridge Protocol Data Units are frames that contain information about the spanning tree protocol. A switch sends BPDUs using a unique source MAC address from its origin port to a multicast address with destination MAC.

OSPF- open shortest path first – Interior protocols are meant to dynamically route data across a network that you fully control and maintain. Open standard - routers rely on cost to compute the shortest path , essentially the more hops greater cost , ospf is used to find lowest cost route.

EIGRP- Enhanced interior gateway protocol –Interior protocols are meant to dynamically route data across a network that you fully control and maintain. Cisco specific until 2013.

BGP- boarder gateway protocol, Exterior routing protocols are used to exchange routes between distinctly separate networks that you have no administrative control over. BGP is the routing protocol used on the internet; therefore, the most common enterprise use is to run BGP on your internet edge when connecting to your ISP.

Network loop – A network loop is a network configuration where there is more than one path between two computers or devices, which causes packets to be constantly repeated. 

Broadcast storm- usually from a network loop continually forwarding traffic flooding the network bringing it down.



**Common port numbers:**

Application      Port                        Use                                     Protocol

HTTP

80

Web

TCP

HTTPS

443

Web(secure)

TCP

FTP

20,21

File Transfer

TCP

SMTP

25

Email

TCP

DNS

53

Translates domain names to IP addresses 

UDP , TCP

telnet

23

Remote login

TCP

SSH

22

Remote login (Secure)

TCP

NTP

123

Network time of day

UDP![[Subnet Mask Cheat Sheet.pdf]]