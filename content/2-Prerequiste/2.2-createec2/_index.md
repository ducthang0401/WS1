---
title : "Create EC2"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---

#### CREATE PUBLIC EC2 INSTANCE

**Access the AWS Management Console**:

1.	Navigate to EC2, then Click on **Instances**
 
**In the EC2 interface**:

1.	Select Instances

2.	Choose Launch instances

![EC2](/images/2.prerequisite/027-createec2.png)

3.	Provide a Name and tags for the instance, enter **public instance**

4.	**Choose the AMI:**
-	 Select Quick Start
-	 Choose Amazon Linux 2
-	 Select an AMI
 
5.	Select an **Instance type (t2micro)** and opt to Create a new key pair

6.	In the **Create key pair interface**:
-  Specify the Key pair name, e.g., NAT-keypair (optional name, you can set any).
-  Choose Key pair type: RSA
-  Select Private key file format: .pem
 
7.	**Configure the Network:**
- Select the VPC: **Lab VPC**
- Choose the Subnet: **MyPublicSubnet**
- **Enable** Auto-assign public IP
  ![ec2](/images/ec1.png)

-  For Firewall (Security Group), select **creat security group**
    ![ec2](/images/ec2.png)
 
8.	**Complete the instance creation**


 
#### CREAT EC2 INSTANCE IN PRIVATE SUBNET

**In the EC2 interface**:

1. Select Instances
   
2. Choose Launch instances
   ![EC2](/images/2.prerequisite/027-createec2.png)

**Repeat the steps to create an EC2 in a public instance.**

3.	**Configure the Network:**
-	 Select the VPC: **Lab VPC**
-	 Choose the Subnet: **My Private Subnet**
-	 **Disable** Auto-assign public IP. 
(If not disabling it, ensure you’ve checked the configuration
for automatically allocating public IP for the subnet).
    ![ec2](/images/ec3.png)

4.	Select EC2 Private:
-  Choose Details
-  Store Private IPv4 addresses
 

