---
title : "Introduction"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---
**A NAT Gateway** is a device in AWS that enables instances within a private subnet to connect to the internet or other AWS services, while preventing inbound connections from the internet. It works by forwarding outbound traffic from the private instances, translating their private IP addresses to the NAT Gateway's IP address, and then routing the response back to the instances. This ensures that instances remain secure from direct internet exposure.


There are two types of NAT devices: NAT Instances and NAT Gateways. 
- NAT Instances use Amazon Linux AMIs and have limitations based on the instance type and region, without support for IPv6 traffic. 
- NAT Gateways, on the other hand, are charged hourly and also do not support IPv6 traffic. However, AWS recommends using NAT Gateways due to their better availability and higher bandwidth compared to NAT Instances.
