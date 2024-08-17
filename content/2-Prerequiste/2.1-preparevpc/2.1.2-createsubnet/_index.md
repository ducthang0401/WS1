---
title : "Create Subnet"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2.1.2 </b> "
---


In this task, we are going to create both public and private subnets within the VPC. Public subnets have internet connectivity, while private subnets do not have direct internet access.


In the AWS Management Console, navigate to Subnets in the left panel of the VPC page.



#### CREATE PUBLIC SUBNET

1. Click **Create subnet**.

![Subnet](/images/subnet1.png)

 At the **Create subnet** page.
-	VPC ID : select **Lab VPC**
-	Subnet Name : Enter **MyPublicSubnet**
-	Availability Zone : No Preference
-	IPv4 CIDR block : Enter **10.0.0.0/24**
-	Click on **Create subnet** button.

![Subnet](/images/subnet2.png)

1. Let's enable Auto Assign public IP to Instances created within this subnet:
-	Select **MyPublicSubnet** , Click on **Actions**.
-	Click on **Edit subnet settings**.
-	**Enable auto-assign public IPv4 address** : Check
-	Click on **Save**.

Oke, the public Subnet has been created


#### CREATE PRIVATE SUBNET

Click on **Create subnet**.

![Subnet](/images/subnet1.png)

- VPC ID : select **Lab VPC**
-	Subnet Name : Enter **MyPrivateSubnet**
-	Availability Zone : No Preference
-	IPv4 CIDR block : Enter **10.0.1.0/24**
-	Click on **Create subnet** button.
	
![Subnet2](/images/subnet3.png)
