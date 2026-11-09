# Highly Available Multi-Tier Web Application on AWS

## Overview

This project involved setting up and testing a highly available, multi-tier web application infrastructure on Amazon Web Services (AWS). The architecture uses Amazon EC2 for application hosting, Amazon RDS for database management, and an Application Load Balancer to distribute incoming traffic across application instances.

The project also explored infrastructure configuration using Terraform and tested application behaviour under simulated traffic to observe instance health and Auto Scaling behaviour.

## Architecture

The infrastructure was organised into multiple AWS components:

- **Amazon VPC:** Created an isolated network environment for hosting the application.
- **Public and Private Subnets:** Organised resources across different network tiers.
- **Internet Gateway:** Enabled internet connectivity for public-facing resources.
- **NAT Gateway:** Provided outbound internet access for resources in private subnets.
- **Amazon EC2:** Hosted the application instances.
- **Amazon RDS (MariaDB):** Provided relational database services.
- **Application Load Balancer (ALB):** Distributed incoming application traffic.
- **Auto Scaling Group:** Managed application instances and supported instance replacement.
- **IAM:** Configured permissions and roles for AWS resource access.
- **Security Groups:** Controlled network traffic between infrastructure components.

## Technologies Used

- Amazon Web Services (AWS)
- Amazon EC2
- Amazon VPC
- Amazon RDS (MariaDB)
- Application Load Balancer
- Auto Scaling
- IAM
- Terraform
- ApacheBench (ab)

## Implementation

### 1. Network Infrastructure

Configured the VPC networking environment with public and private subnets, route tables, an Internet Gateway, and a NAT Gateway to organise network connectivity.

### 2. Application Infrastructure

Set up EC2 application instances and an RDS MariaDB database. Configured the Application Load Balancer to distribute incoming requests across the application instances.

### 3. High Availability and Scaling

Configured an Auto Scaling Group to manage EC2 instances across availability zones. Observed instance health and replacement behaviour during infrastructure testing.

### 4. Infrastructure as Code

Worked with existing Terraform configurations, making modifications to support the infrastructure setup and configuration.

### 5. Load Testing

Used ApacheBench to generate simulated HTTP traffic and examine application behaviour under load. Observed instance health and Auto Scaling responses during testing.

## Key Learning Outcomes

- Understanding AWS networking and VPC architecture.
- Working with EC2, RDS, IAM, and security groups.
- Understanding load balancing and Auto Scaling.
- Working with existing Terraform infrastructure configurations.
- Observing application and instance behaviour under simulated traffic.
- Understanding the relationship between networking, application hosting, and database infrastructure.

## Project Scope

This was a team-based academic project focused on AWS infrastructure setup, high availability, and load testing. The implementation and testing were conducted in a project environment and should not be interpreted as a production deployment.



Jeswanth Naidu Padi

[GitHub](https://github.com/Jeswanthpadi) · [LinkedIn](https://www.linkedin.com/in/jeswanthnaidupadi/)
