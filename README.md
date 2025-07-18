# ☁️ AWS 3-Tier Architecture Deployment Project

Designed and deployed a highly available and scalable three-tier web architecture on AWS using best practices for performance, security, fault tolerance, and cost optimization.

 🧩 Architecture Overview

This project follows the classic 3-tier design pattern:

 🔹 **Presentation Layer (Frontend)**  
  - Static website hosted on Amazon S3
  - Public access secured with S3 Bucket Policies
  - Website accessible via S3 endpoint or custom domain 

  🔹 **Application Layer (Backend)**  
  - Hosted on EC2 instances inside an Auto Scaling Group (ASG)  
  - Load balanced using an Application Load Balancer (ALB)  
  - Managed using custom launch templates and IAM roles  

 🔹 **Database Layer**  
  - Managed MySQL database on Amazon RDS  
  - Multi-AZ deployment with automatic backups and failover  


 ⚙️ Technologies & Tools Used

✅ AWS Services :
- EC2, S3, RDS (MySQL)
- IAM, ALB, ASG, VPC

✅ Networking :
- Custom VPC
- Public & Private Subnets
- NAT Gateway
- Security Groups & NACLs

✅ Security :
- IAM Roles & Policies
- SSL/TLS with HTTPS (ALB)
- Principle of Least Privilege (PoLP)

✅ Automation & DevOps :
- Linux Shell Scripting for instance configuration and deployment tasks
- Manual setup of infrastructure using AWS Console and CLI
- AWS Lambda 

🚀 Features Implemented :
-  Highly available and auto-scaled EC2-based app tier
-  Secure static frontend hosting with  S3
-  RDS MySQL with Multi-AZ & automated backups
-  CI/CD pipeline for code deployment (GitHub Actions)
-  IAM policy management and logging setup
-  Cost-efficient resource provisioning
-  Infrastructure automation with Terraform

  📁 Project Structure :
application code/

├── web-tier/ # Static frontend files (HTML/CSS/JS)

├── app-tier/ # Backend application code (Flask/Node)

├── nginx.conf # Reverse proxy configuration

├── .github/workflows/ # GitHub Actions pipeline definition

 
 



