# AWS Cloud Web Server Deployment with LAMP Stack

## 📌 Project Overview
This project demonstrates how to deploy a secure web server on AWS using **Terraform** and configure a **LAMP (Linux, Apache, MySQL, PHP)** stack on an EC2 instance.  

The setup ensures a secure and scalable environment by using a **custom VPC** with both public and private subnets, NAT Gateway, and properly configured security groups.  

---

## 🚀 Project Architecture
- **Terraform** provisions:
  - VPC with public and private subnets  
  - Internet Gateway & NAT Gateway  
  - Route Tables for public/private networking  
  - Security Groups for web and database layers  
  - EC2 instance named **lamp-stack**  

- **Manual Configuration (on EC2 Ubuntu 24.04)**:
  - Install Apache, MySQL, and PHP  
  - Configure PHP and Apache for web hosting  
  - Secure MySQL and create a database with user  
  - Deploy test PHP scripts (`info.php` and `dbtest.php`)  

---

## 🛠️ Prerequisites
- AWS account with IAM user (programmatic access)  
- Terraform installed locally  
- SSH client (e.g., **Termius** or `ssh`)  
- Basic knowledge of Linux commands  

---

## 📂 Project Setup

### 1. Clone Repository
```bash
git clone https://github.com/<your-username>/aws-lamp-stack.git
cd aws-lamp-stack
