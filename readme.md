# AWS Project Deployment Checklist

## 1️⃣ Network Setup  
**Objective:** Build the foundational AWS network environment.

We will create and configure:

- VPC  
- Internet Gateway (IGW)  
- Public & Private Subnets  
- Public Route Table  
- NAT Gateway  
- Private Route Table  
- Security Groups  

---

## 2️⃣ Upload Application Code  
**Objective:** Store and prepare website files for hosting.

- Create S3 Bucket  
- Upload static website files (HTML, CSS, JS)  

---

## 3️⃣ IAM Permissions  
**Objective:** Enable secure access between AWS services.

- Create IAM Role with S3 Full Access  

---

## 4️⃣ Server Setup  
**Objective:** Launch and configure EC2 instances.

- Create SSH Key Pair  
- Launch EC2 Web Server in Public Subnet  
- SSH into EC2  

---

## 5️⃣ Application Installation  
**Objective:** Install and configure the web server.

- Install Apache  
- Deploy Application Files  
- Verify Web Server Accessibility  

---

## 6️⃣ Bastion Host Setup  
**Objective:** Enable secure SSH access for private instances.

- Launch Bastion Host in Public Subnet  
- Launch Private EC2 Instance  
- Install & Configure Web Application (via Bash Script)  
- SSH through Bastion Host to verify access  

---

## 7️⃣ Load Balancing  
**Objective:** Ensure high availability and scalability.

- Create Target Group  
- Create Application Load Balancer (ALB)  
- Verify Health Checks  

---

## 8️⃣ Domain & SSL Configuration  
**Objective:** Make the website accessible securely.

- Register Domain in Route 53  
- Create DNS Record (A/CNAME)  
- Request SSL Certificate via ACM  
- Attach Certificate to ALB  

---

## 9️⃣ Auto Scaling  
**Objective:** Enable automatic scaling for demand changes.

- Create Launch Template  
- Create Auto Scaling Group (ASG)  
- Test Scaling Triggers  

---

## 🔟 Project Wrap-Up  
**Objective:** Validate and clean up resources.

- Test access via domain  
- Clean up AWS resources  
