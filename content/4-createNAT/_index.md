---
title : "Create NAT Gateway"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---


In this step, we are going to create a NAT Gateway, which provides internet access to instances in the private subnet. The NAT Gateway acts as a middleman to forward traffic between the private subnet and the internet.

1.	**Allocate Elastic IP Address**
- Select Elastic IPs --> Allocate Elastic IP address
![NAT](/images/nat1.png)
- Public IPv4 address pool: Select **Amazon’s pool of IPv4 addresses**
  
 
2. **Create NAT Gateway**
-	Select **NAT Gateway** --> Create **NAT gateway**
![NAT](/images/nat2.png)
 
In **NAT gateway** interface:
- Name: Enter **NAT-gw**
- Subnet: Select **MypublicSubnet**
- Connectivity type: Select **Public**
- Elastic IP allocation ID: Select recently created Elastic IP
- Create **NAT gateway**
![NAT](/images/nat3.png)
 

 


