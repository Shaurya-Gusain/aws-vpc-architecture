# AWS VPC Architecture with Public & Private Subnets

## 📌 Project Overview

This project demonstrates the design and implementation of a secure and scalable network architecture using Amazon Web Services (AWS). The setup includes a Virtual Private Cloud (VPC) with both public and private subnets, enabling controlled internet access and internal communication between resources.

---

## 🎯 Objective

* To create a custom VPC with isolated network environments
* To deploy resources in both public and private subnets
* To enable secure internet access using gateways
* To understand AWS networking fundamentals and routing

---

## 🏗️ Architecture Components

* **VPC (Virtual Private Cloud)**
* **Public Subnet** (for internet-facing resources)
* **Private Subnet** (for secure/internal resources)
* **Internet Gateway (IGW)**
* **NAT Gateway**
* **Route Tables**
* **EC2 Instances**

---

## 🌐 Architecture Description

* A VPC is created with a defined CIDR block
* Two subnets are configured:

  * Public Subnet (connected to Internet Gateway)
  * Private Subnet (isolated, uses NAT Gateway for outbound access)
* Route tables are configured to manage traffic flow
* EC2 instances are deployed in both subnets
* Public instance can access the internet directly
* Private instance accesses the internet via NAT Gateway

---

## 🪜 Implementation Steps

1. Created a VPC with a custom CIDR block
2. Created Public and Private Subnets
3. Attached an Internet Gateway to the VPC
4. Created a NAT Gateway in the Public Subnet
5. Configured Route Tables:

   * Public route → Internet Gateway
   * Private route → NAT Gateway
6. Launched EC2 instances in both subnets
7. Verified connectivity:

   * Internet access from public instance
   * Outbound internet from private instance via NAT

---

## 📸 Screenshots

*(Add your screenshots here)*

* VPC configuration
* Subnet setup
* Route tables
* EC2 instances
* Connectivity tests

---

## 🧠 Key Learnings

* Understanding of AWS VPC and subnetting
* Difference between public and private subnets
* Role of Internet Gateway and NAT Gateway
* Route table configuration and traffic flow
* Secure cloud architecture design

---

## 🚀 Future Improvements

* Automate setup using Terraform or AWS CloudFormation
* Add Load Balancer for high availability
* Implement Auto Scaling
* Add security groups and network ACL optimizations

---

## 💼 Use Case

This architecture is widely used in real-world applications where:

* Web servers are hosted in public subnets
* Databases and internal services are secured in private subnets
* Controlled and secure communication is required

---

## 🏁 Conclusion

This project provides a foundational understanding of AWS networking and demonstrates the ability to design secure and scalable cloud infrastructure, which is essential for Cloud and DevOps roles.

---
