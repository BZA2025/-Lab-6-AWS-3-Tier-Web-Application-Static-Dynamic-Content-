# ⚡ Lab 6 – AWS 3-Tier Web Application (Static + Dynamic Content)

## 📌 Overview
In this lab, I deployed a **3-tier web application architecture** on AWS using my reusable VPC design (from Lab 7). The focus was on separating **presentation, application, and database layers** for scalability, security, and maintainability.  

This lab simulates a **production-style architecture** where static assets are delivered securely and application logic is isolated from the database layer.  

---

## 🏗️ Architecture Components
- **VPC** with **public**, **private (app)**, and **database** subnets  
- **S3 bucket** for hosting static content (`styles.css`, `logo.png`)  
- **EC2 Web/App Tier** in public/private subnets  
- **Security Groups & NACLs** enforcing restricted flows  
- **Route Tables** directing internet and private traffic correctly  

---

## 🔑 Key Steps Completed
- Created an **S3 bucket** (`rt-lab6-static-bazbucket-<random>`) for static hosting  
- Uploaded and served **logo.png** + **styles.css** from the bucket  
- Configured **IAM roles/policies** for EC2 → S3 access  
- Launched **EC2 instances** in correct subnets with public/private accessibility  
- Verified connectivity across **tiers** (web → app → db placeholder)  

---

## ✅ Skills Demonstrated
- AWS 3-Tier Web App deployment  
- S3 static hosting + bucket policy configuration  
- IAM role integration with EC2  
- Networking design with public/private subnets  
- Enforcing least-privilege SG/NACL access  

---

## 🚀 Next Steps
- Integrate **RDS MySQL** (Lab 7) for a full 3-tier stack  
- Add **ALB + Auto Scaling Group** for web tier resilience  
- Automate deployments with **Terraform**  

---

📂 **Repository:** [Lab 6 – AWS 3-Tier Web Application]  
