<img width="1224" height="688" alt="image" src="https://github.com/user-attachments/assets/13899dce-790f-40a3-ade2-39c2b68a49b8" />

# High-Availability & Scalable Web Infrastructure on AWS ☁️

## 📝 Project Overview
This project demonstrates the design and implementation of a resilient, highly available, and secure multi-tier architecture on **Amazon Web Services (AWS)**. The infrastructure is designed for web pplication hosting handling traffic by distributing workloads across multiple **Availability Zones (AZs)**.

## 🏗️ Architecture Design 

### 1. Networking & Connectivity
* **Custom VPC:** A logically isolated virtual network with a `10.0.0.0/16` CIDR block for secure resource management.
* **Multi-AZ Deployment:** Resources are distributed across **Availability Zone A** and **Availability Zone B** to eliminate single points of failure.
* **Subnet Strategy:**
    * **Public Subnets:** Host the Application Load Balancer (ALB) and NAT Gateway to manage inbound/outbound internet traffic.
    * **Private Subnets:** Securely host Web Instances and RDS Databases, completely isolated from direct public internet access.
* **Internet Gateway (IGW):** Acts as the bridge between the VPC and the public internet.

### 2. Compute & Traffic Management
* **Application Load Balancer (ALB):** Distributes incoming traffic across multiple EC2 instances to optimize performance and availability.
* **Auto Scaling Group (ASG):** Automatically adjusts the number of EC2 instances based on demand, ensuring the application stays available during traffic spikes.

### 3. Database Layer (Persistence)
* **Amazon RDS (Multi-AZ):** Implements a **Primary** database instance with a **Standby (Secondary)** instance in a different AZ for synchronous replication and automatic failover.

### 4. Security & Traffic Control
* **Security Groups:** Layered virtual firewalls for the ALB, Web, and Database tiers.
* **NAT Gateway:** Provides instances in private subnets with internet access for updates while blocking inbound traffic.

## 🛠️ AWS Services Stack
* **Compute:** EC2, Auto Scaling.
* **Networking:** VPC, ALB, Internet Gateway, NAT Gateway.
* **Database:** Amazon RDS (Relational Database Service).

---
*Developed by Hanaa Abd El-reheem - Cloud & DevOps Engineer*
