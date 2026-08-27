# EX 4 :DEPLOYMENT AND CONFIGURATION OF A PRIVATE CLOUD IN AWS
### NAME: MURALITHARAN K M
### REG NO: 212223040121

## Aim
To create an Amazon Virtual Private Cloud (VPC) with public and private subnets, configure a security group, and launch an EC2 instance hosting a web server within the VPC. 

## Objectives
- Create an Amazon VPC.
- Create public and private subnets.
- Configure a security group for HTTP access.
- Launch an EC2 instance inside the VPC.
- Deploy and access a web server running on the EC2 instance.

---

# Procedure

## Task 1: Create a Virtual Private Cloud (VPC)

1. Log in to the AWS Management Console and open the **VPC** service.
2. Select **Create VPC** and choose **VPC and More**.
3. Configure the VPC with the required CIDR block, public subnet, private subnet, Internet Gateway, and NAT Gateway.
4. Create the VPC and verify that all resources are created successfully.

---

## Task 2: Create Additional Subnets

1. Create a second public subnet in another Availability Zone.
2. Create a second private subnet in the same Availability Zone.
3. Associate the private route table with the new private subnet.
4. Associate the public route table with the new public subnet.
5. Verify the subnet associations.
---

## Task 3: Create a Security Group

1. Navigate to **Security Groups** in the VPC console.
2. Create a new security group named **Web Security Group**.
3. Add an inbound rule allowing **HTTP (Port 80)** traffic from **Anywhere (IPv4)**.
4. Save the security group.
---

## Task 4: Launch an EC2 Web Server

1. Open the **EC2** service and launch a new instance.
2. Select **Amazon Linux 2023 AMI** and **t2.micro** instance type.
3. Configure the instance to use the newly created VPC, public subnet, and Web Security Group.
4. Add the provided user data script to install Apache, PHP, and the sample web application.
5. Launch the instance and wait until all status checks pass.
6. Access the web server using the Public IPv4 DNS.

---

# Outputs

## Output 1: VPC Creation


<img width="1400" height="953" alt="Screenshot 2026-08-25 092927" src="https://github.com/user-attachments/assets/5241755b-8aa5-4921-8f1a-377e3cbd50b2" />



## Output 2: Additional Subnets

<img width="1412" height="957" alt="Screenshot 2026-08-25 092938" src="https://github.com/user-attachments/assets/398c44b7-e277-4400-85e1-191eaf313a1e" />

<img width="1411" height="963" alt="Screenshot 2026-08-25 093128" src="https://github.com/user-attachments/assets/26e076b3-ae54-4b9b-8022-6fd6cd91563c" />

<img width="1405" height="978" alt="Screenshot 2026-08-25 093242" src="https://github.com/user-attachments/assets/9f2fe94f-720a-4a55-b167-3bc1c1fb7195" />

<img width="1422" height="965" alt="Screenshot 2026-08-25 093806" src="https://github.com/user-attachments/assets/079845cd-a408-4a73-a815-428d792b533d" />

## Output 3: Security Group Configuration

<img width="1421" height="970" alt="Screenshot 2026-08-25 094349" src="https://github.com/user-attachments/assets/e4af5790-4b20-41b0-a4d0-ae5e8e0e478f" />


## Output 4: EC2 Web Server Deployment

<img width="1405" height="967" alt="Screenshot 2026-08-25 094920" src="https://github.com/user-attachments/assets/8872f8ca-5723-4594-aae3-6abddd5db197" />

<img width="1840" height="843" alt="Screenshot 2026-08-25 095323" src="https://github.com/user-attachments/assets/ef182112-2524-4e5b-ae9a-68a5741bc4a9" />

## Output 5: Grade and Submission Report

<img width="1917" height="933" alt="Screenshot 2026-08-20 215651" src="https://github.com/user-attachments/assets/e6b55151-efd8-426b-900b-cf3f9c44452f" />

<img width="1557" height="575" alt="Screenshot 2026-08-20 215711" src="https://github.com/user-attachments/assets/5604515f-d61b-4d8a-a559-a82cfce5434f" />


---

# Result

Thus, a VPC was configured, an EC2 instance was launched, and the hosted web application was accessed successfully. 
