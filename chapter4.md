
## Java Socket

Java Socket programming is used for communication between the applications running on different JRE.

Java Socket programming can be connection-oriented or connection-less.

Socket and ServerSocket classes are used for connection-oriented socket programming and DatagramSocket and DatagramPacket classes are used for connection-less socket programming.

The client in socket programming must know two information:

1. IP Address of Server, and
2. Port number.

Here, we are going to make one-way client and server communication. In this application, client sends a message to the server, server reads the message and prints it. Here, two classes are being used: Socket and ServerSocket. The Socket class is used to communicate client and server. Through this class, we can read and write message. The ServerSocket class is used at server-side. The accept() method of ServerSocket class blocks the console until the client is connected. After the successful connection of client, it returns the instance of Socket at server-side.

![image](https://github.com/pritamhazra21/WIT/assets/75198912/621650d4-00b8-48a4-922a-c2fb394df486)


## Java RMI.

The RMI (Remote Method Invocation) is an API that provides a mechanism to create distributed application in java. The RMI allows an object to invoke methods on an object running in another JVM.

The RMI provides remote communication between the applications using two objects stub and skeleton.

### Understanding stub and skeleton
RMI uses stub and skeleton object for communication with the remote object.

A remote object is an object whose method can be invoked from another JVM. Let's understand the stub and skeleton objects:

#### stub
The stub is an object, acts as a gateway for the client side. All the outgoing requests are routed through it. It resides at the client side and represents the remote object. When the caller invokes method on the stub object, it does the following tasks:

1. It initiates a connection with remote Virtual Machine (JVM),
0. It writes and transmits (marshals) the parameters to the remote Virtual Machine (JVM),
0. It waits for the result
0. It reads (unmarshals) the return value or exception, and
0. It finally, returns the value to the caller.
#### skeleton
The skeleton is an object, acts as a gateway for the server side object. All the incoming requests are routed through it. When the skeleton receives the incoming request, it does the following tasks:

1. It reads the parameter for the remote method
0. It invokes the method on the actual remote object, and
0. It writes and transmits (marshals) the result to the caller.

In the Java 2 SDK, an stub protocol was introduced that eliminates the need for skeletons. 
![image](https://github.com/pritamhazra21/WIT/assets/75198912/d894c92c-2903-4d26-98bc-843a1c196b8b)
### Understanding requirements for the distributed applications
If any application performs these tasks, it can be distributed application.

1. The application need to locate the remote method
1. It need to provide the communication with the remote objects, and
1. The application need to load the class definitions for the objects.

The RMI application have all these features, so it is called the distributed application.

### Java RMI Example
The is given the 6 steps to write the RMI program.

1. Create the remote interface
1. Provide the implementation of the remote interface
1. Compile the implementation class and create the stub and skeleton objects using the rmic tool
1. Start the registry service by rmiregistry tool
1. Create and start the remote application
1. Create and start the client application


## Threats (1L):
## Malicious code-viruses, Trojan horses, worms; eavesdropping, spoofing, modification, denial of service attacks.

Malicious code and various cyber threats pose significant risks to computer systems, networks, and individuals. Here are some common threats you mentioned:

1. Viruses: These are self-replicating programs that can attach themselves to files and spread from one computer to another. Viruses can cause damage by corrupting or deleting files, disrupting system operations, or stealing personal information.

1. Trojan Horses: These are malicious programs disguised as legitimate software. Once installed, Trojan horses can perform unauthorized actions, such as stealing sensitive information, modifying files, or providing unauthorized access to the attacker.

1. Worms: Worms are similar to viruses but can spread independently without requiring user interaction. They exploit vulnerabilities in computer systems and networks to propagate rapidly, causing network congestion, system slowdowns, or unauthorized access.

1. Eavesdropping: Also known as snooping or sniffing, eavesdropping involves intercepting and monitoring network traffic to capture sensitive information. Attackers can exploit insecure networks or unencrypted communications to gain unauthorized access to data, including passwords, financial details, or confidential conversations.

1. Spoofing: Spoofing refers to impersonating or masquerading as someone or something else to deceive users or gain unauthorized access. This can include IP spoofing (manipulating the source IP address of network packets), email spoofing (forging the sender's email address), or DNS spoofing (redirecting users to malicious websites).

1. Modification: Modification attacks involve altering data or code to manipulate its integrity, leading to unauthorized changes in system behavior or compromising the confidentiality and accuracy of information. This can include unauthorized modifications of files, databases, or system configurations.

1. Denial of Service (DoS) Attacks: DoS attacks aim to disrupt or deny access to a system, network, or service, making them inaccessible to legitimate users. Attackers flood the target with excessive traffic, overwhelming its resources and causing system failures or slowdowns. Distributed Denial of Service (DDoS) attacks involve multiple compromised systems coordinating the attack.

These threats highlight the importance of implementing robust security measures, such as antivirus software, firewalls, encryption, secure network protocols, and user awareness training, to mitigate the risks and protect against cyber attacks. Regular software updates and patches are also crucial to address known vulnerabilities.

Network security techniques (2L): 
Password and Authentication;

## VPN,

VPN stands for the virtual private network. A virtual private network (VPN) is a technology that creates a safe and encrypted connection over a less secure network, such as the internet. A Virtual Private Network is a way to extend a private network using a public network such as the internet. The name only suggests that it is a Virtual “private network” i.e. user can be part of a local network sitting at a remote location. It makes use of tunneling protocols to establish a secure connection. 

## IP Security, 

IPsec, short for IP Security, is a set of protocols and standards used to secure IP communications at the network layer. It provides confidentiality, integrity, and authentication for IP packets. IPsec encrypts and authenticates data to protect it from unauthorized access or tampering. It is commonly used in VPNs to create secure tunnels over untrusted networks like the Internet. IPsec ensures secure transmission of data at the network level, making it an essential tool for network security.

## security in electronic transaction, 


## Secure Socket Layer (SSL),

Secure Socket Layer (SSL) provides security to the data that is transferred between web browser and server. SSL encrypts the link between a web server and a browser which ensures that all data passed between them remain private and free from attack. 

#### Secure Socket Layer Protocols: 

+ SSL record protocol
+ Handshake protocol
+ Change-cipher spec protocol
+ Alert protocol


### SSL Protocol Stack:  
![image](https://github.com/pritamhazra21/WIT/assets/75198912/fb794289-bb18-4b0d-b32d-9be867725d7d)
#### SSL Record Protocol: 
SSL Record provides two services to SSL connection. 

+ Confidentiality
+ Message Integrity

In the SSL Record Protocol application data is divided into fragments. The fragment is compressed and then encrypted MAC (Message Authentication Code) generated by algorithms like SHA (Secure Hash Protocol) and MD5 (Message Digest) is appended. After that encryption of the data is done and in last SSL header is appended to the data. 
![image](https://github.com/pritamhazra21/WIT/assets/75198912/adb179dc-576c-4a59-ba9e-c6f24aa40ad6)
#### Handshake Protocol: 

Handshake Protocol is used to establish sessions. This protocol allows the client and server to authenticate each other by sending a series of messages to each other. Handshake protocol uses four phases to complete its cycle. 

+ Phase-1: In Phase-1 both Client and Server send hello-packets to each other. In this IP session, cipher suite and protocol version are exchanged for security purposes. 
+ Phase-2: Server sends his certificate and Server-key-exchange. The server end phase-2 by sending the Server-hello-end packet. 
+ Phase-3: In this phase, Client replies to the server by sending his certificate and Client-exchange-key. 
+ Phase-4: In Phase-4 Change-cipher suite occurs and after this the Handshake Protocol ends. 
![image](https://github.com/pritamhazra21/WIT/assets/75198912/d68e8b6d-d927-4769-9580-e2d57ddbb0df)
#### Change-cipher Protocol: 
This protocol uses the SSL record protocol. Unless Handshake Protocol is completed, the SSL record Output will be in a pending state. After the handshake protocol, the Pending state is converted into the current state. 
Change-cipher protocol consists of a single message which is 1 byte in length and can have only one value. This protocol’s purpose is to cause the pending state to be copied into the current state. 
![image](https://github.com/pritamhazra21/WIT/assets/75198912/23d7ec14-2213-4a6b-8c16-27204958a345)
#### Alert Protocol: 
This protocol is used to convey SSL-related alerts to the peer entity. Each message in this protocol contains 2 bytes.
![image](https://github.com/pritamhazra21/WIT/assets/75198912/0ae90d00-ca9e-42d9-a72f-bc2614701566)

## Secure Shell (SSH).

SSH(Secure Shell) is access credential that is used in the SSH Protocol. In other words, it is a cryptographic network protocol that is used for transferring encrypted data over network. It allows you to connect to a server, or multiple servers, without having you to remember or enter your password for each system that is to login remotely from one system into another. 

It always comes in key pair: 
 

1. Public key – Everyone can see it, no need to protect it. (for encryption function)
2. Private key – Stays in computer, must be protected. (for decryption function)

Key pairs can be of the following types: 
 
1. User Key – If public key and private key remain with the user.
1. Host Key – If public key and private key are on a remote system.
1. Session key – Used when large amount of data is to be transmitted.

How SSH Works ? 
It uses asymmetric cipher for performing encryption and decryption. There are many encryption methods: rsa, dsa, ed25519 etc. 

General procedure is :- 
 

+ Public keys from the local computers (system) are passed to the server which is to be accessed.
+ Server then identifies if the public key is registered.
+ If so, the server then creates a new secret key and encrypts it with the public key which was send to it via local computer.
+ This encrypted code is send to the local computer.
+ This data is unlocked by the private key of the system and is send to the server.
+ Server after receiving this data verifies the local computer.
+ SSH creates a route and all the encrypted data are transferred through it with no security issues.


Firewall (1L):
Introduction, 
Packet filtering, 
Stateful, 
Application layer, 
Proxy.
