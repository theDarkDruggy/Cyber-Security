# **Network Fundamentals**  

**Open System :** A system that is able to connect with other systems.  
**Closed System :** A system that is not able to connect with other systems.  
**Computer Networks :** An interconnection between multiple systems and multiple devices.   
**Network Topology :** Shape of how network devices connecting.  
**OSI**( *open Systems interconnection* ) : That defines protocols for communication and connection.  
**Host Name :** Uniqe name of the device in the Network.  
**Ip address :** Ip address is address of the every device in the network. *private ip address* is used to connect with other devices in the network. *public ip address* is used to connect with devices out of the network. You can get ip addresses while writing ifconfig/ipconfig to command line.  
**MAC**( *Media Access Control* ) : A media access control address (MAC address) is a unique identifier assigned to a network interface controller (NIC) for use as a network address in communications within a network segment.  
**Port :** A port can be referred to as a logical channel through which data can be sent/received to an application.  
* 0-1023 : Well-known ports
* 1024-49151 : Registered ports
* 19152-65535 : Ephemeral ports  

You can write **netstat -a** to command line.  
**Socket :** A unique combination of port number and ip number , those are termed together as Socket.  
**DNS Server :** DNS (Domain  Name System) is a system that converts urls to ip address and provides access.  
**ARP :**( *Address resolution Protocol* ) The Address Resolution Protocol (ARP) is a communication protocol used for discovering the link layer address, such as a MAC address, associated with a given internet layer address.    
**RARP :**( *Reverse ARP* ) The Reverse Address Resolution Protocol (RARP) is an obsolete computer networking protocol used by a client computer to request its Internet Protocol (IPv4) address from a computer network, when all it has available is its link layer or hardware address, such as a MAC address.  
**Internet :** Internet is a global network that was created with smaller networks.  
**Web :** Web is only way of accessing information through the internet.  
**URI :** URI means "uniform resource identifier"  A URI can be a name, locator, or both for an online resource whereas a URL is just the locator.

### **How is websites opening**
**when you open a url :**  
* HTTP Request (request of getting HTML file)  
    * When you send http request , it is converted to binary code and it is sent by internet to thee server. DNS servers turn URIs into IP addresses and binary code is forwarded there.
* Servers Response
    * Servers analyzes clients request and makes a decision. and sends file via internet to your port of your public IP.

### **Some Facts about Networking**
* Internet was invented by ARPANET in 1983.
* Internet is controlled by 75 million servers.
* Backbone of internet is made by 550, 000 miles of underwater cable.
* About one billion computer systems are connected to internet.
* Internet consists of five billion computing devices such as computers, phones, modems, switches, routers etc.
* According to Google, Internet consists of 5 million Terabytes of data.
* If the internet goes down for a day, approximately 200 billion emails and 3 billion Google search would have to wait.
* Approximately 204 million emails per minute are send over Internet. 70% of them are spam.
* 269 billion emails are sent per day.
* for more you can visit [this site ...](https://www.geeksforgeeks.org/unknown-facts-of-networking/?ref=lbp)
### **Network Goals**
#### *Network Elements:*
* At least two computers
* Transmission medium between either wired or wireless
* Protocols that will provide communication
* Network Software such as Network operating system

#### **Criteria**
1. Performance
    * Transit Time  
    * Response Time
    * These are affect performance :
        * Number of Users
        * Type of transmission medium
        * Capability of Network
        * Efficiency of Software
2. Reliability
    * Frequency of Failure
    * Recovery from failures
3. Security
    * Protecting data that was shared through network  

#### **Goals**
1. Resource Sharing
    * Many organization has computers more than one , sharing data between these is one of goals.
2. High Reliability
    * Connecting many computers to each other without problem.
3. Inter-Process communication
    * Network must provide nearly errorless communication between devices in different geographical conditions.
4. Flexible Access
    * Files can be accessed from any computer in the network.
### **Transmission Modes**
* Simplex Mode
    * in simplex mode , there is only one way to send data. Like radios.
* Half-Duplex Mode
    * in half-duplex mode , there is two way to send data but not at the same time.
* Duplex Mode
    * in duplex mode , there is two way to send data and you can send and receive data at the same time.

### **Types of Transmission Media**
* Guided Media
	* High Speed
	* Secure
	* Used for short distances
	1. Twisted Pair Cable
		1. UTP (Unshielded Twisted Pair)
			* Has Ability of block interferance
			* This is used for telephonic applications
			* Easy to install
			* High-speed capacity
			* Lower capacity and performance in comparsion to STP
		2. STP (Shielded Twisted Pair)
			* Performance is better than UTP
			* Faster
			* Difficult to install and manufacture
			* More expensive
			* Bulky
	2. Coaxible Cable
		* Advantages:
			* High Bandwidth
			* Better Noise Immunity
			* Easy to install and expand
			* Inexpensive
		* Disadvantages:
			* Single cable failure can disrupt entire network
		* Analog TV Networks and Cable TV
	3. Optical Fibre Cable
		* Advantages:
			* Increased capacity and bandwidth
			* Lightweight
			* Less signal Autantion
			* Immunity to electromagnetic  interferance
		* Disadvantages:
			* Difficult to install and maintain
			* High cost
			* Fragile
* Unguided Media
	* The signal is broadcasted through air
	* Less Secure
	* Used for largerdistances
	1. Radiowaves
		* Frequency range : 3KHz - 1GHz
		* AM and FM radios use
	2. Microwaves
		* 1GHz - 300GHz
		* Phone communication and television distribution use
	3. Infrared
		* 300 GHz - 400 THz
		* TV remotes , Wireless , Mouse , Printer , Keyboard  
**Unicast :** Communication between two computers.   
**Broadcast :** Communication between one sender and receivers  
	* Limited Broadcasting : In the same network  
	* Direct Broadcasting : Broadcast to the another network  
**Multicast :** One sender and multiple receivers  

***
*Websites that i used* :  
* [Geeks4Geeks](https://www.geeksforgeeks.org/computer-network-tutorials/)  
* [Wikipedia](https://en.wikipedia.org/wiki/)
