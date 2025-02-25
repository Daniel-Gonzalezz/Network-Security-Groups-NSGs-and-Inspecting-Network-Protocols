<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1: Create a Network Security Group (NSG)
- Step 2:  Associate NSG with Virtual Machines' Subnet or Network Interface
- Step 3: Define Inbound and Outbound Security Rules
- Step 4: Inspect Traffic Between Virtual Machines

<h2>Actions and Observations</h2>

![image](https://github.com/user-attachments/assets/b866c7ef-a51d-4d0d-b88c-01b8c6cc7725)

When two computers "ping" each other, they essentially send a small data packet (like a "hello" message) from one computer to the other, and then wait for a response packet back, effectively checking if the other computer is reachable on the network and confirming the connection quality by measuring the time it takes for the packet to travel between them; this is done using a network command called "ping" which displays the round-trip time for the data packet. 

![image](https://github.com/user-attachments/assets/b37b199c-b5d2-418b-a0b9-58aa03b2a980)

In this example we have set up a layer 3 firewall and you can see that the request timed out, which essentially means that a firewall is blocking the connection. A firewall acts as a security barrier between a private network and the public internet, monitoring and filtering all incoming and outgoing network traffic based on predefined rules, deciding whether to allow or block data packets depending on whether they meet the established security criteria, effectively preventing unauthorized access and malicious traffic from entering the network while permitting legitimate connections. 

