<img width="1224" height="688" alt="image" src="https://github.com/user-attachments/assets/13899dce-790f-40a3-ade2-39c2b68a49b8" />

# Scalable and Highly Available AWS Architecture

## ☁️ Project Overview
This project focuses on designing and deploying a **Scalable and Highly Available (HA)** infrastructure on Amazon Web Services (AWS). The architecture is built to ensure performance, reliability, and security for web applications hosting following AWS Best Practices.

## 🏗️ Architecture Components
* **Compute:** Scalable **Amazon EC2** instances.
* **Networking:** * **Application Load Balancer (ALB):** To efficiently distribute incoming traffic across multiple instances.
    * **VPC & Security Groups:** Applied strict resource configuration and security protocols.
* **Database:** **Amazon RDS** (Relational Database Service) for a managed and persistent data layer.

## 🛠️ Key Features
* **High Availability:** Architecture designed to handle failures by distributing resources across multiple availability zones.
* **Scalability:** Deployed resources that can adapt to varying traffic loads using AWS best practices.
* **Security & Best Practices:** Applied AWS networking and security group standards to protect the infrastructure.

## 📂 Infrastructure Overview
```text
├── Networking/
│   ├── VPC Configuration
│   └── Security Groups Rules
├── Compute/
│   ├── EC2 Instances
│   └── Application Load Balancer
└── Database/
    └── Amazon RDS 
