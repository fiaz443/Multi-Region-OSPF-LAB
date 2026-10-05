# Multi-Region-OSPF-LAB

This lab demonstrates how *OSPF Stub Areas, Totally Stubby Areas, and Regular Areas* can be used in a multi-regional enterprise network to reduce unnecessary routing information and optimize routing resources at branch locations.
**Overview:**

This project models a multi-region enterprise network. Router1 and Router2 form the Area 0 backbone. Each regional area connects to the backbone through a point-to-point /30 link and contains one router, one switch and end devices. Router0 represents the external (Resource/Internet) network and connects to a separate R-ISP router hosting a NAT/PAT server.

**Objectives:**

Build a multi-area OSPF design with a central backbone

Understand the difference between Regular, Stub and Totally Stubby areas

Connect regional LANs to the backbone using /30 point-to-point links

Provide external connectivity through an edge router

Practice NAT/PAT with an ISP-side server

**Topology:**
The lab is built in Cisco Packet Tracer. The full diagram is available as

![Multi-Region OSPF Topology](https://raw.githubusercontent.com/fiaz443/Multi-Region-OSPF-LAB/main/WhatsApp%20Image%202026-09-30%20at%201.39.05%20PM.jpeg)

**Area Design:**

Area
Region
Area Type
Router
Switch
End Devices
Area 0
Backbone
Backbone
Router1, Router2
-
-
Area 40
North
Stub
Router3
Switch0
PC0, PC1
Area 50
South
Totally Stubby
Router4
Switch1
Server0, PC3
Area 60
East
Regular
Router6
Switch3
PC4, PC5
Area 70
West
Regular
Router5
Switch2
PC6, PC7
External
Resource/Internet
-
Router0
-
-
NAT/PAT
ISP side
-
R-ISP
-
NAT/PAT_SERVER


