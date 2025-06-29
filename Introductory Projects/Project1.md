Usecase:

Project Goals:

Architecture:

Technologies used:

## 🧰 Technologies Used

- **Amazon VPC** – Created a custom Virtual Private Cloud with CIDR `172.16.0.0/16`
- **Subnet** – Configured a public subnet (`172.16.1.0/24`)
- **Internet Gateway (IGW)** – Enabled outbound internet access for the VPC
- **Route Tables** – Set up custom route to direct traffic through the IGW
- **Amazon EC2** – Launched a Linux virtual machine in the public subnet
- **Elastic IP (EIP)** – Assigned a static public IP to the EC2 instance
- **Security Groups** – Allowed inbound traffic for SSH (22), HTTP (80), HTTPS (443)
- **Network ACLs (NACLs)** – Added subnet-level stateless firewall rules
- **Key Pairs** – Used to securely SSH into the EC2 instance
- **AWS Management Console** – Used the console UI to provision all resources

Deployment steps:
