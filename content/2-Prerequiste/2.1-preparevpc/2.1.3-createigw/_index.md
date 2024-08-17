---
title : "Create Internet Gateway"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 2.1.3 </b> "
---

In this task, we are going to create an Internet Gateway, which acts as a bridge between the VPC and the internet, allowing instances in the VPC to communicate with the internet.


#### CREATE INTERNET GATEWAY

In the VPC Management Console:

- Click **Internet Gateway**
- Click **Create Internet Gateway**
  
![igw](/images/igw1.png)

At the **Creat Internet Gateway** page:

1.	Name tag: **MyIGW**
2.	**Creat**

![igw](/images/igw2.png)

#### ATTACH AN IGW TO A VPC

1.	Click on **Actions**, Select **Attach to VPC**.
2.	VPC : Select **Lab VPC**
3.	Click on **Attach internet gateway**.

![igw](/images/igw3.png)

Now, MyIGW is attached to Lab VPC
