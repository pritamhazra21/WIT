
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

0. It initiates a connection with remote Virtual Machine (JVM),
0. It writes and transmits (marshals) the parameters to the remote Virtual Machine (JVM),
0. It waits for the result
0. It reads (unmarshals) the return value or exception, and
0. It finally, returns the value to the caller.
#### skeleton
The skeleton is an object, acts as a gateway for the server side object. All the incoming requests are routed through it. When the skeleton receives the incoming request, it does the following tasks:

0. It reads the parameter for the remote method
0. It invokes the method on the actual remote object, and
0. It writes and transmits (marshals) the result to the caller.

In the Java 2 SDK, an stub protocol was introduced that eliminates the need for skeletons. 

Threats (1L):
Malicious code-viruses, Trojan horses, worms; eavesdropping, spoofing, modification, denial of service attacks.
Network security techniques (2L): 
Password and Authentication;
VPN, 
IP Security, 
security in electronic transaction, 
Secure Socket Layer (SSL),
Secure Shell (SSH).
Firewall (1L):
Introduction, 
Packet filtering, 
Stateful, 
Application layer, 
Proxy.
