# AWS 3-Tier Architecture Project

This project implements a 3-tier architecture on AWS to simulate a production-ready web application setup.

## 🧱 Architecture Overview

The project includes the following layers:

- **Presentation Layer (Web Tier)**:
  - Public subnet with EC2 instances behind an Application Load Balancer (ALB)
  - Handles internet (HTTP(S)) requests to the architecture.

- **Application Layer (App Tier)**:
  - Private subnet with EC2 instances
  - Processes business logic
  - Connected to Web Tier via security groups

- **Data Layer (Database Tier)**:
  - Private subnet hosting an RDS instance (MySQL/PostgreSQL)
  - Only accessible from App Tier

## ☁️ AWS Services/Tools Used

- VPC -  public and private subnets
- EC2 instances 
- Security Groups
- Application Load Balancer (ALB)
- Auto Scaling Groups (ASG)
- RDS (Relational Database Service)
- Internet Gateway & NAT Gateway
- AWS CLI
- Terraform

## 🧪 How to Deploy


1. Clone the repository:
   ```bash
   git clone https://github.com/Tangential313/Aws3tierarchitecture.git
   cd Aws3tierarchitecture
