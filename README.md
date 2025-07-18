# ☁️ AWS 3-Tier Architecture Deployment Project

Designed and deployed a highly available and scalable three-tier web architecture on AWS using best practices for performance, security, fault tolerance, and cost optimization.

## 🧩 Architecture Overview

This project follows the classic 3-tier design pattern:

- 🔹 **Presentation Layer (Frontend)**  
  - Hosted on Amazon S3 (static website hosting)  
  - Secured and accelerated using Amazon CloudFront (CDN)  
  - Custom domain setup via Route 53  

- 🔹 **Application Layer (Backend)**  
  - Hosted on EC2 instances inside an Auto Scaling Group (ASG)  
  - Load balanced using an Application Load Balancer (ALB)  
  - Managed using custom launch templates and IAM roles  

- 🔹 **Database Layer**  
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
- AWS WAF & Shield
- SSL/TLS with HTTPS (via CloudFront/ALB)
- Principle of Least Privilege (PoLP)

✅ Monitoring & Logging :
- CloudWatch for metrics & logs
- CloudTrail for API auditing

✅ Automation & DevOps :
- Infrastructure as Code using Terraform
- GitHub Actions for CI/CD pipeline
- Linux Shell Scripting
- AWS Lambda (optional components/functions)

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

 
 



