---
title : "Creat public route table and config"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

In this step, we are going to create a public route table and configure it to associate with the public subnet. The public route table defines how traffic is routed between the VPC and the internet.



1. In the **VPC Management Console**:
- Click **Route table**  --> **Creat Route table**

  ![route table](/images/rt1.png)

2. Configure the **Route table**:
- Name: **route table public**
- VPC: **Lab VPC**
- Create
 ![route table](/images/rt2.png)

3. Attach to **IGW** (Internet Gateway)
- Click **public route table** --> **Edit route**
- In the **Edit route interface**, choose **Add route**
- Destination: **0.0.0.0/0** (Internet)
- Target: **Internet Gateway**
- Save changes

4. Associate the **Public Subnet** to the **route table** 
- Select PublicRouteTable:
- Click on the Subnet Associations tab.
- Click on Edit subnet associations.
- On the next page, select MyPublicSubnet from the list displayed.
- Click on Save associations.


