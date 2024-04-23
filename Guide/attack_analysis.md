# NTAnalyser
NTAnalyser is a lightweight tool designed for network engineers to analyse packet data efficiently. It provides various analysis options such as protocol, IPv4, IPv6, MAC, source, and destination analysis. Use NTAnalyser to gain insights into your network traffic and troubleshoot issues effectively.

To start NTAnalyser, firs start the server with `build.sh`, then run the main packet capturing tool with the `--analysis` argument. NTAnalyser should open as a local webpage in the background. To begin analysis of captured packets, press the *start analysis* button.

## Source/Destination Analysis
<img src="https://github.com/TomosSherlock/NetworkTrafficAnalysis/assets/123552121/bda4d6a1-8601-44da-ba72-82790a4e6710" alt="address graph" align="left" style="padding-right:30px"/>NTAnalyser can chart the addresses of connected devices within the network. It tracks three different address formats. If any format doesn't show a graph, the software has not found any devices with that address format. Every node is a different address. Every edge between a node means that these two addresses have communicated with each other. These graphs are undirected, so it is not indicated whether a node is the receiver, sender, or both. Hovering over a node will display its address. A link is indicative of if a connection between these addresses has been made, not the number of times they have communicated. 

### IPv4 Analysis
These graphs can grow quite large, so scrolling may be needed. It is usual for an IPv4 graph to be more dense than its IPv6 counterpart, though this is not always the case.

### IPv6 Analysis 
IPv6 nodes are shown. These graphs can also grow quite large, but are usually less dense than IPv4 graphs.

### MAC Analysis
A visualisation of MAC nodes. A MAC graph is generally more sparse than an IPv6 or IPv4, since network interfaces may have multiple IPs, but will have only one MAC address.

## Frequency Analysis
The total number of captured packets packets is graphed for different protocols, source addresses and destination addresses:
![image](https://github.com/TomosSherlock/NetworkTrafficAnalysis/assets/123552121/e4f96f41-8aa3-4abf-8918-470077ee336d)
![image](https://github.com/TomosSherlock/NetworkTrafficAnalysis/assets/123552121/ef9bcabe-a599-4dab-867f-40e2b3afdddc)


