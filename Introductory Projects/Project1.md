Usecase:

Project Goals:

Architecture:

## 🧰 Technologies Used
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

Deployment steps:
