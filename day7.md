## Training day 7:-

## Network:
A computer network is a group of two or more interconnected computer systems that share data and resources through communication channels.
## Host:-
A host is a network-connected device assigned with an IP address, which allows it to participate in communication over a network.
## Server:-
A server is a powerful host machine in a network that runs server software and responds to client requests, such as hosting websites, storing files, or managing emails.
## Client:-
A server is a powerful host machine in a network that runs server software and responds to client requests, such as hosting websites, storing files, or managing emails.
## Traffic:-
Network traffic is the flow of data packets over a network, including all types of communication such as browsing, file transfers, video streaming, emails, etc.

 ### IP address:
full form: Internet Protocol.
where protocol refers to the set of rules which govern the data transmission.
Properties:

Unique: Each device on a network must have a unique IP address.

Universal: IP addresses are a globally recognized standard for network communication.

Types:

Public IP Address: Used on the internet, these addresses are globally unique and routable.

Private IP Address: Used within private networks (e.g., home or school networks), these addresses are not directly routable on the internet.

Dynamic Nature: IP address can change over time, especially for devices on dynamic IP assignments. However, its fundamental properties (uniqueness and universality) remain constant.
### IPV4:
Internet Protocol version 4
An IPv4 address consists of series of four eight-bit binary numbers which are separated by decimal point. Although any numbering system can be used to represent a unique 32- bit number, most commonly you see IP address expressed in dot decimal notation.
#### IPv4 Address Format:

An IPv4 address consists of 32 bit (binary digit), grouped into four section of known as octets or bytes. Each octet has 8 bits and this bits can be represented only in 0 or 1 form, and when they grouped together, they form a binary number. Since each octet has 8 bits, it can represent 256 numbers ranging from o to 255. These four octets are represented as decimal numbers, separated by periods known as dotted decimal notation. For example IPv4 address 185.107.80.231 consists of four octets.
#### Binary Representation:
IPv4 is basically converted into binary form by computer although these are usually seen in decimal form for human readability. Each octet is converted into 8 bit binary number . For instance 185.107.80.231 in binary looks like:
![image](https://github.com/user-attachments/assets/2247b1e7-421c-4a3b-9db4-bdf5f9dff972)

185: 10111001
107: 01101011
80: 01010000
231: 11100111

### IPV6:
Internet Protocol Version 6
The Internet Protocol version 6, or IPv6, is the latest version of the Internet Protocol (IP), which is the system used for identifying and locating computers on the Internet. IPv6 was developed by the Internet Engineering Task Force (IETF) to deal with the problem of IPv4 exhaustion. IPv6 is a 128-bit address having an address space of 2128, which is way bigger than IPv4. IPv6 uses a Hexa-Decimal format separated by a colon (:).
#### Components in IPv6 Address Format:
There are 8 groups and each group represents 2 Bytes (16-bits). 
Each Hex-Digit is of 4 bits (1 nibble)
Delimiter used - colon (:)

![image](https://github.com/user-attachments/assets/1c29e8ab-6b31-40ae-9c51-29f8dc6defed)

 ### Classes in IP:
![image](https://github.com/user-attachments/assets/e4cd50a3-1462-45a4-bc68-1da24261f54f)

### DIFFERENCE BTW UNICAST, MULTICAST, BROADCAST.
![image](https://github.com/user-attachments/assets/56949c97-5759-426e-88fb-3abb589900d0)

## Subnetting 
subnetting is a technique used to split a network into multiple smaller networks, each with its own range of IP addresses, while still being part of the same larger network.

### Why Use Subnetting?
-Reduces network congestion

- Improves security (isolates network sections)

- Helps in efficient IP address allocation

- Simplifies network management
## Mac address:-
A MAC address is a 48-bit unique identifier assigned to a network device by its manufacturer, used for communication within a local network (LAN).

- Key Features:
Permanently burned into hardware (but can be changed in software)

Expressed in hexadecimal format

Used for device-to-device communication in the same network
## DNS :-
The Domain Name System (DNS) is a hierarchical system that maps human-readable domain names to machine-readable IP addresses on the internet or within a network.

### Why DNS is Needed:
- Humans remember names like youtube.com

- Computers use IP addresses like 142.250.195.14

- DNS acts as a translator between them

### How DNS Works (Steps):
- You type www.example.com in your browser.

- The computer asks the DNS Resolver for the IP.

- Resolver queries DNS servers in order:

### Root Server

- Top-Level Domain (TLD) Server (.com, .org)

- Authoritative Name Server (actual domain's IP info)

- The IP address is returned to the browser.

-Browser connects to the IP and loads the website.
### default Gateway:-
A Default Gateway is the device (usually a router) that connects a local network to the internet or to another network. It acts as an access point or IP router that a device uses to send data to another network or the outside world.
 ### Why It’s Important:
 - It connects devices in your network to the internet.

- Without a default gateway, devices can only communicate locally.

- It helps in routing data between networks.


