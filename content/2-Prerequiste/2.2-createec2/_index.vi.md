---
title : "Tạo EC2"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2.2 </b> "
---


#### TẠO PUBLIC EC2 INSTANCE

**Truy cập vào AWS Management Console**:

1. Điều hướng đến EC2

2. Nhấp vào Instances

image

**Trong giao diện EC2**:

1. Chọn Instances

2. Chọn Launch instances

3. Cung cấp Name and tags cho phiên bản, nhập EC2 Public

4. Chọn AMI:
- Chọn Quick Start
- Chọn Amazon Linux 2
- Chọn một AMI
- Chọn loại instance (Instance type) và chọn tạo một key pair (Create a new key pair)

5. Trong giao diện Create key pair:
- Chỉ định tên cặp khóa (Key pair name), ví dụ: aws-keypair (tên tùy chọn, bạn có thể đặt bất kỳ tên nào).
- Chọn loại key pair (Key pair type): RSA
- Chọn định dạng tệp khóa riêng tư (Private key file format): .pem
  
6. Cấu hình mạng (Configure the Network):
- Chọn VPC: Lab VPC
- Chọn Subnet: MyPublicSubnet
- Bật Auto-assign public IP
- Đối với Firewall (Security Group), chọn Select existing security group
- Chọn Public subnet -SG
- Nhấp vào Launch instance
- Hoàn tất việc tạo instance (Complete the instance creation)



#### TẠO EC2 INSTANCE TRONG PRIVATE SUBNET

**Trong giao diện EC2**:

1. Chọn Instances

2. Chọn Launch instances

3. Cung cấp Name and tags, nhập EC2 Private

4. Chọn AMI:
- Chọn Quick Start
- Chọn Amazon Linux 2
- Chọn một AMI
- Chọn loại instance (Instance type). Chọn tên key pair (Key pair name): aws-keypair

5. Cấu hình mạng (Configure the Network):
- Chọn VPC: Lab VPC
- Chọn Subnet: My Private Subnet
- Tắt Auto-assign public IP. Nếu không tắt, hãy đảm bảo rằng bạn đã kiểm tra cấu hình tự động gán IP công cộng cho subnet.
- Hoàn tất việc tạo phiên bản (Complete the instance creation):
- Nhấp vào View all instances
  
6. Chọn EC2 Private:
- Chọn Details
- Lưu trữ địa chỉ Private IPv4 addresses