# Introduction

## Internet
Internet is a global network that connects billions of computers across the world with each other and to the World Wide Web. It uses standard internet protocol suite (TCP/IP) to connect billions of computer users worldwide. It is set up by using cables such as optical fibers and other wireless and networking technologies. At present, internet is the fastest mean of sending or exchanging information and data between computers across the world.

## Intranet, Extranet and Internet.
![image](https://github.com/pritamhazra21/WIT/assets/75198912/8b74f862-5b30-47b8-88ff-a0375741ebfc)
![image](https://github.com/pritamhazra21/WIT/assets/75198912/fae38001-9fde-493e-9464-0690f05819dc)


## World Wide Web (1L):
## Domain and Sub domain 

In the context of computer networks and the internet, a domain refers to a group of devices or resources that are organized and managed together. It represents a specific network or a collection of related resources.

A subdomain, on the other hand, is a subset or subdivision of a larger domain. It allows for further organization and categorization of resources within the main domain. Subdomains are typically used to distinguish different sections or departments within an organization or to allocate specific functions or services to different parts of a website or network.

For example, in the domain "example.com," a subdomain could be "blog.example.com" or "shop.example.com." These subdomains can be used to separate the blog section or the e-commerce section of the website from the main domain.

In summary, a domain represents a broader group or network of resources, while a subdomain is a subset or subdivision within that domain, used for further organization or categorization purposes.

## Address Resolution,
Address resolution refers to the process of mapping a higher-level identifier, such as a logical or symbolic address, to a lower-level identifier, such as a physical address. It is commonly used in computer networks, specifically in the context of mapping IP addresses to MAC addresses in Ethernet networks.

In an IP network, devices are identified by their IP addresses, which are logical addresses assigned to them. However, when data needs to be transmitted over the network, it needs to be delivered to the correct device's physical address, known as the MAC address. This is where address resolution comes into play.

The Address Resolution Protocol (ARP) is a commonly used protocol for address resolution in Ethernet networks. When a device wants to send data to another device on the same network, it broadcasts an ARP request packet, asking for the MAC address associated with a specific IP address. The device that has the requested IP address responds with its MAC address, allowing the sender to create an entry in its ARP cache and use the MAC address for future communications.

In short, address resolution is the process of mapping higher-level identifiers, such as IP addresses, to lower-level identifiers, such as MAC addresses, in order to facilitate communication within a network.

## DNS

An application layer protocol defines how the application processes running on different systems, pass the messages to each other.

+ DNS stands for Domain Name System.
+ DNS is a directory service that provides a mapping between the name of a host on the network and its numerical address.
+ DNS is required for the functioning of the internet.
+ Each node in a tree has a domain name, and a full domain name is a sequence of symbols specified by dots.
+ DNS is a service that translates the domain name into IP addresses. This allows the users of networks to utilize user-friendly names when looking for other hosts instead of remembering the IP addresses.
+ For example, suppose the FTP site at EduSoft had an IP address of 132.147.165.50, most people would reach this site by specifying ftp.EduSoft.com. Therefore, the domain name is more reliable than IP address.

## Telnet, FTP

Telnet and FTP are both protocols used for remote communication and file transfer, respectively. Here's a brief explanation of each:

1. Telnet:
Telnet is a network protocol that allows a user to establish a remote connection to a computer or networking device over a network. It provides a virtual terminal or command-line interface to access and control the remote device as if you were physically present. Telnet operates on the client-server model, where a client application connects to a remote server using the Telnet protocol.

Telnet was widely used in the early days of the internet for remote administration, remote login, and accessing text-based services. However, Telnet has some security vulnerabilities, as it transmits data in plain text, including login credentials, which makes it susceptible to interception and unauthorized access. Due to these security concerns, Telnet is often replaced by more secure protocols like SSH (Secure Shell).

2. FTP (File Transfer Protocol):
FTP is a standard network protocol used for transferring files between a client and a server on a computer network. It provides a way to upload, download, and manage files remotely. FTP operates on a client-server architecture, where a client application connects to an FTP server to perform file operations.

FTP supports various operations, including uploading files from the client to the server (put), downloading files from the server to the client (get), deleting files, renaming files, creating directories, and listing directory contents. FTP can handle both binary and text files.


## HTTP.

HTTP stands for Hypertext Transfer Protocol, and it is the underlying protocol used for communication between clients (web browsers) and servers on the World Wide Web. HTTP allows for the transfer of hypertext documents, such as HTML files, over the Internet.

Here are some key points about HTTP:

1. Client-Server Communication: HTTP follows a client-server model, where a client (usually a web browser) sends requests to a server, and the server responds with the requested data. The client initiates the communication by sending an HTTP request, and the server sends back an HTTP response containing the requested data or an error message.

2. Stateless Protocol: HTTP is a stateless protocol, which means that each request-response cycle is independent and does not retain any information about previous requests. This requires the use of additional mechanisms, such as cookies or session tokens, to maintain stateful interactions between the client and server.

3. Request Methods: HTTP defines various request methods or verbs that indicate the desired action to be performed on the server. The most common methods are:

+ GET: Retrieves a resource from the server.
+ POST: Sends data to the server to be processed, often used for form submissions.
+ PUT: Updates a resource on the server with the provided data.
+ DELETE: Removes a resource from the server.
4. URL Structure: HTTP requests include a Uniform Resource Locator (URL) to specify the location of the requested resource. The URL consists of a protocol identifier (e.g., "http://"), a domain name or IP address of the server, and a path to the specific resource.

5. Status Codes: HTTP responses include status codes that indicate the outcome of the request. Common status codes include:

+ 200 OK: The request was successful, and the server is sending the requested data.
+ 404 Not Found: The requested resource was not found on the server.
+ 500 Internal Server Error: An error occurred on the server while processing the request.
6. Secure Communication: HTTPS (HTTP Secure) is an extension of HTTP that uses encryption and secure sockets layer (SSL) or transport layer security (TLS) protocols to provide secure communication between the client and server. HTTPS is commonly used for transmitting sensitive data, such as login credentials or financial information.

HTTP is a fundamental protocol for web browsing and data exchange on the Internet. It enables the retrieval and delivery of web content, making it possible for users to access websites, interact with web applications, and retrieve resources from remote servers.


## Review of TCP/IP (1L):
Features, Segment, Three-Way Handshaking, Flow
Control, Error Control, Congestion control, IP
Datagram, IPv4
and IPv6.
IP Subnetting and addressing (1L):
Classful and Classless Addressing, Subnetting. NAT,
IP masquerading, IP tables.



## Internet Routing Protocol (1L):

Internet routing protocols are protocols used by routers to exchange information and make decisions on how to forward network traffic within an interconnected network, such as the Internet. These protocols help in determining the most efficient paths for data to travel from source to destination across multiple networks. Here are some commonly used Internet routing protocols:

1. Border Gateway Protocol (BGP): BGP is the primary routing protocol used for routing between autonomous systems (ASes) in the Internet. It enables routers in different ASes to exchange information about network reachability and make routing decisions. BGP is a path vector protocol that takes into account various attributes, including network policies, to determine the best path for traffic.

2. Open Shortest Path First (OSPF): OSPF is an interior gateway protocol (IGP) used within a single autonomous system. It operates based on the shortest path first algorithm to calculate the best routes and exchange routing information between routers. OSPF is commonly used in large enterprise networks and Internet Service Provider (ISP) networks.

3. Routing Information Protocol (RIP): RIP is an older distance-vector routing protocol that operates within a single autonomous system. It uses hop count as a metric to determine the best paths and shares routing information periodically with neighboring routers. RIP is simple to configure and deploy but may have limitations in larger networks due to its limited scalability.

4. Intermediate System to Intermediate System (IS-IS): IS-IS is a link-state routing protocol used for routing within a single autonomous system. It is similar to OSPF but is commonly used in larger service provider networks. IS-IS operates based on the link-state database and uses metrics to determine the best routes.

These are just a few examples of routing protocols used in the Internet. Different protocols are designed to meet specific needs, considering factors such as scalability, convergence speed, network size, and administrative control. Internet routing protocols play a crucial role in ensuring efficient and reliable data transmission across the interconnected networks of the Internet.

## Routing -Intra and Inter Domain Routing

In the context of networking and Internet routing, intra-domain routing and inter-domain routing refer to different levels of routing within and between autonomous systems (ASes). Here's an explanation of each:

1. Intra-Domain Routing:
Intra-domain routing, also known as interior gateway protocol (IGP) routing, focuses on routing within a single autonomous system (AS). An AS is a collection of networks under a single administrative control, such as an organization or an Internet service provider (ISP). Intra-domain routing protocols are used to exchange routing information and determine the best paths for traffic within the boundaries of an AS.
Common examples of intra-domain routing protocols include OSPF (Open Shortest Path First) and IS-IS (Intermediate System to Intermediate System). These protocols operate within an AS and are responsible for computing and disseminating routing information among routers within the same network.

The goal of intra-domain routing is to ensure efficient and reliable communication within the boundaries of an AS, optimizing network performance and facilitating connectivity between devices within the same organization or network.

2. Inter-Domain Routing:
Inter-domain routing, also referred to as exterior gateway protocol (EGP) routing, focuses on routing between different autonomous systems. It involves the exchange of routing information and the determination of the best paths for traffic between ASes, enabling communication across different networks or organizations.
The primary inter-domain routing protocol used in the Internet is the Border Gateway Protocol (BGP). BGP enables routers in different ASes to exchange information about network reachability and make decisions on how to forward traffic between ASes. BGP takes into account various attributes, such as network policies, path preferences, and path costs, to determine the optimal routes for data transmission between ASes.

Inter-domain routing is essential for connecting networks operated by different organizations, ISPs, or service providers, allowing data to traverse multiple autonomous systems to reach its destination. It enables global connectivity and facilitates communication between networks belonging to different entities.

In summary, intra-domain routing deals with routing within a single autonomous system, optimizing traffic paths within an organization or network. Inter-domain routing, on the other hand, focuses on routing between different autonomous systems, facilitating connectivity and communication between networks operated by different organizations or service providers.

## Unicast and Multicast Routing, 

Unicast and multicast routing are two different approaches to routing network traffic in computer networks. Here's an explanation of each:

1. Unicast Routing:
Unicast routing is the most common form of routing in computer networks. In unicast routing, data is sent from a single source to a single destination. Each packet is addressed to a specific destination address, and the routing decisions are made based on the destination address contained in the packet header.
Unicast routing is used in typical client-server communication scenarios, where a client device sends a request to a specific server, and the response is sent back to the client. Routing protocols such as OSPF and BGP are examples of unicast routing protocols that determine the best path for data transmission from a source to a destination.

2. Multicast Routing:
Multicast routing is designed for simultaneous transmission of data from a single source to multiple recipients. In multicast routing, a single packet is sent from the source, and it is replicated and forwarded to a group of designated recipients. The recipients are part of a multicast group and share a common group address.
Multicast routing is particularly useful for applications that require one-to-many or many-to-many communication, such as multimedia streaming, video conferencing, and online gaming. Instead of sending multiple unicast packets to each recipient individually, multicast routing optimizes network bandwidth and reduces network traffic by sending a single packet that is shared among the recipients.

Multicast routing protocols, such as Protocol Independent Multicast (PIM) and Internet Group Management Protocol (IGMP), are used to manage the membership of multicast groups, establish multicast distribution trees, and efficiently forward multicast packets to the group members.

In summary, unicast routing is used for point-to-point communication, where data is sent from a single source to a single destination. Multicast routing, on the other hand, is designed for one-to-many or many-to-many communication, where a single packet is sent to a group of recipients. Unicast is the traditional form of routing, while multicast is specifically optimized for efficient distribution of data to multiple recipients

## Broadcast.

Broadcast is a communication method used in computer networks to send a message from a source device to all devices within a specific network segment or broadcast domain. The message is intended for all devices to receive and process, and it is typically addressed using a special broadcast address. Broadcasts are commonly used for network discovery, service announcements, address resolution, and configuration updates. However, as networks grow larger, broadcasts can become resource-intensive and less efficient.

## Electronic Mail (1L):

Email (electronic mail) is a widely used method of exchanging digital messages between individuals, businesses, and organizations. It allows users to send, receive, and store messages electronically. Here are some key points about email:

1. Message Composition: Email messages typically consist of a sender's address, a recipient's address, a subject line, and the message body. Users can compose messages using email clients, web-based email services, or mobile apps.

2. Addressing: Each email message requires a unique email address for the sender and recipient. Email addresses have a specific format, typically in the form of username@domain.com, where the username represents the individual or organization, and the domain specifies the mail server.

3. Message Transmission: Email messages are transmitted over computer networks using the Simple Mail Transfer Protocol (SMTP). The sender's email server connects to the recipient's email server to deliver the message. Intermediate servers and routing protocols help ensure the message reaches its intended destination.

4. Attachments: Email messages can include attachments, which are files (e.g., documents, images, or videos) that are sent along with the message. Attachments allow users to share files easily and efficiently.

5. Storage and Retrieval: Emails can be stored on email servers or downloaded to a client device. Users can access their email messages through email clients (e.g., Outlook, Thunderbird) or web-based email interfaces (e.g., Gmail, Outlook.com). Email clients often support features like organizing messages into folders, searching for specific emails, and managing contacts.

6. Spam and Security: Email is vulnerable to various security risks, including spam (unsolicited bulk emails), phishing attempts, malware attachments, and email spoofing. Users should be cautious when opening email attachments or clicking on links from unknown or suspicious sources.

7. Email Protocols: In addition to SMTP, email communication often involves other protocols such as POP3 (Post Office Protocol version 3) and IMAP (Internet Message Access Protocol). POP3 and IMAP allow users to retrieve emails from a mail server to a client device, synchronize email across multiple devices, and manage folders and messages on the server.

Email has become an integral part of personal and professional communication, offering a convenient and efficient means of exchanging messages and information across vast distances. It has revolutionized communication and remains one of the most widely used forms of digital communication worldwide.

## POP3, SMTP.

POP3 (Post Office Protocol version 3) and SMTP (Simple Mail Transfer Protocol) are two common protocols used for email communication. Here's a brief explanation of each:

POP3 (Post Office Protocol version 3):
POP3 is an email retrieval protocol that allows an email client to access and download emails from a remote mail server. When a user checks their email using a POP3 client, such as Microsoft Outlook or Mozilla Thunderbird, the client connects to the POP3 server and retrieves the email messages stored there. Once the messages are downloaded to the client's device, they are typically removed from the server (although some configurations allow leaving copies on the server).
POP3 is a relatively simple protocol and works well in situations where users want to download and store their emails locally. However, it lacks some advanced features like folder synchronization and server-side message management. It is primarily used for receiving emails.

SMTP (Simple Mail Transfer Protocol):
SMTP is a protocol used for sending email messages between mail servers. It is responsible for the transmission of email from the sender's mail server to the recipient's mail server. When a user sends an email using an email client, such as Gmail or Outlook, the client uses SMTP to connect to the sender's mail server and deliver the email. The sender's server then communicates with the recipient's server via SMTP to deliver the email message.
SMTP is a robust and widely supported protocol that enables reliable email delivery across different mail servers. It handles the routing and delivery of email messages, including features like message queuing, error handling, and authentication.

In email systems, POP3 and SMTP often work together. SMTP is used for sending outgoing mail from the client to the server, while POP3 is used for retrieving incoming mail from the server to the client. These protocols, along with others like IMAP (Internet Message Access Protocol), form the foundation of email communication and enable users to send, receive, and manage their email messages.

In summary, POP3 is a protocol for retrieving email messages from a mail server to a client, while SMTP is a protocol for sending email messages between mail servers. They are complementary protocols that enable email communication and are commonly used in email systems.




