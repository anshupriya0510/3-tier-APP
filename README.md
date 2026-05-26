# 🚀 AWS 3-Tier Architecture on AWS

A **Production-Ready 3-Tier Architecture** built on **Amazon Web Services (AWS)** using **VPC, EC2, Application Load Balancer, Auto Scaling Group, RDS, NAT Gateway, Bastion Host, and Multi-AZ Deployment**.

This project demonstrates how to build a **secure, scalable, and highly available cloud infrastructure** following industry best practices.

---

# 📌 Architecture Overview

This architecture consists of **3 layers**:

## 1️⃣ Web Tier
- Hosted in **Public Subnets**
- Internet-facing **Application Load Balancer**
- EC2 instances in Auto Scaling Group

## 2️⃣ Application Tier
- Hosted in **Private Subnets**
- Internal Load Balancer
- Backend EC2 instances

## 3️⃣ Database Tier
- Hosted in **Private Database Subnets**
- Amazon RDS
- Secure access only from application servers

---

# 🛠️ AWS Services Used

- Amazon VPC
- Public & Private Subnets
- EC2
- Application Load Balancer
- Auto Scaling Group
- Amazon RDS
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Bastion Host
- Elastic IP

---

# 🖼️ Architecture Diagram
<img width="800" height="822" alt="image" src="https://github.com/user-attachments/assets/7d9bb7f6-582a-433d-a59b-c0757a3fdbfc" />

step wise implemention

CREATE VPC
<img width="1920" height="1020" alt="Screenshot 2026-05-25 125159" src="https://github.com/user-attachments/assets/3f2738e2-adec-4b0f-bb55-2ef8f0306e16" />
<img width="1920" height="1020" alt="Screenshot 2026-05-26 093406" src="https://github.com/user-attachments/assets/a40a6880-40e8-433a-906b-0f2d2e4a83ae" />


CREATE SECURITY GROUP
<img width="1920" height="1020" alt="Screenshot 2026-05-26 093423" src="https://github.com/user-attachments/assets/fe21d2c3-15c7-4721-ac34-588f7370b833" />

CREATE S3
<img width="1920" height="1020" alt="Screenshot 2026-05-26 093205" src="https://github.com/user-attachments/assets/1eedd973-45e2-410c-822e-be1361ce90ae" />

CREATE RDS
<img width="1920" height="1020" alt="Screenshot 2026-05-26 093514" src="https://github.com/user-attachments/assets/f4056e73-a539-4a30-bd8b-06179f1aad75" />

CREATE IAM ROLE
<img width="1920" height="1020" alt="Screenshot 2026-05-26 093615" src="https://github.com/user-attachments/assets/c97e2c69-dc90-4e99-937b-54017436bff8" />

LAUNCH INSTANCE
<img width="1920" height="1020" alt="Screenshot 2026-05-26 092926" src="https://github.com/user-attachments/assets/3b27ba32-fd37-43d4-8798-c3fbd17d5ffe" />
FOR WEB AND APP
CONNECT <img width="1920" height="1020" alt="Screenshot 2026-05-26 093011" src="https://github.com/user-attachments/assets/42069a1a-70ab-4d0e-bb5e-25cd410b0a4d" />
CONNECT <img width="1920" height="1020" alt="Screenshot 2026-05-26 092949" src="https://github.com/user-attachments/assets/294c5ae2-58ad-43e3-a3d1-72039143474a" />

CREATE TARGET GROUPS <img width="1920" height="1020" alt="Screenshot 2026-05-26 092908" src="https://github.com/user-attachments/assets/339989fc-6c42-4c25-8244-a7e0074c323b" />

CREATE LOADBALANCER <img width="1920" height="1020" alt="Screenshot 2026-05-26 092855" src="https://github.com/user-attachments/assets/ecd7db1b-5476-4086-b95a-15f6d2865688" />
FINALLY DEPLOYED












```text
Name: 3tier-vpc
CIDR Block: 10.0.0.0/16
