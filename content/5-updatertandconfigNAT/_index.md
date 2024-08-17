---
title : "Private route table and config NAT Gateway"
date :  "`r Sys.Date()`" 
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---


1. Create Route table - Private and assign to private subnets
In the VPC interface:
- Select **Route Table**
- Select Create **route table**
![route table](/images/rt1.png)
 
In the **Route table** interface:
- Name: Enter **route table private**
- VPC: Select **Lab VPC**
- Select Create **route table**
![route table](/images/5.1.png)
  
In the **Route table private** interface:
- Select **Subnet Associations**
- Select **Edit subnet associations**
- Choose **My Private Subnet**
- Select Save associations
![route table](/images/5.2.png)


2. **Associate to NAT Gateway**:
   
In the **Route table private** interface:
- Select Routes
- Select **Edit routes**

In the **Edit routes** interface:
- Select **Add route**
- Destination: **0.0.0.0/0**
- Target: **NAT Gateway**
- Select Save changes

![route table](/images/5.3.png)
  

 
