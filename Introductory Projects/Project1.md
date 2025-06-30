## 📖 Use Case Scenario
**Company**: A FinTech startup  
**Project Goal**: Launch an MVP for a **crypto price-tracking web app**  
**Constraints**:
- No managed compute services (e.g., ECS, Lambda) during MVP
- Must host on secure, isolated infrastructure
- Should allow internet access for end users
- Should be scalable in future phases
- Must provide full transparency into networking, security, and costs

**CTO Requirements**:
- Use **Amazon EC2** instead of managed platforms
- Deploy inside a **custom VPC**
- Manually configure networking and security for hands-on learning
- Keep costs low and setup simple for the MVP phase
  
## 🎯 Project Goals

You, acting as a **Cloud/DevOps Engineer**, are tasked with:

- ✅ Designing a secure, **public-facing network architecture** in AWS  
- ✅ Deploying a **Linux EC2 instance** to host the application  
- ✅ Ensuring **public HTTP/HTTPS access**  
- ✅ Applying **layered security** using both **NACLs** and **Security Groups**

ARCHITECTURE:
![1 drawio](https://github.com/user-attachments/assets/f60a7bfb-8150-486b-81ac-a057ccad2eaf)

## 🧰 Technologies Used   EDIT
-----------------------------------------------------------------------------------------------------------
| AWS Service             | Description                                                                   |
|-------------------------|-------------------------------------------------------------------------------|
| **Amazon VPC**          | Created a custom Virtual Private Cloud with CIDR block `172.16.0.0/16`        |
| **Subnet**              | Created a Public Subnet (`172.16.1.0/24`) inside the VPC                      |
| **Internet Gateway**    | Created and attached an IGW to enable internet access                         |
| **Route Table**         | Configured routing for the subnet to send traffic to the internet via IGW     |
| **Elastic IP (EIP)**    | Allocated and attached a static public IP to the EC2 instance                 |
| **Amazon EC2**          | Launched a Linux instance in the public subnet                                |
| **Security Groups (SG)**| Allowed ports 22 (SSH), 80 (HTTP), and 443 (HTTPS) for secure instance access |
| **Network ACLs (NACLs)**| Configured stateless firewall rules for the subnet                            |
| **Key Pairs (EC2)**     | Used for SSH access to the EC2 instance                                       |
| **AWS Console**         | All services provisioned manually through the AWS Management Console UI       |
-----------------------------------------------------------------------------------------------------------

DEPLOYMENT STEPS: 
