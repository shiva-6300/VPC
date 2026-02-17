AWS VPC Architecture using Terraform

This project demonstrates how to design and deploy a secure, production-style VPC architecture in Amazon Web Services using Terraform.

The infrastructure is fully automated using Infrastructure as Code (IaC) principles.

📌 Project Overview

This Terraform project creates:

Custom VPC

Public Subnet

Private Subnet

Internet Gateway

NAT Gateway

Route Tables

Security Groups

EC2 Instance (Public)

The architecture follows a secure cloud networking design where:

Public subnet allows internet access

Private subnet routes traffic through NAT Gateway

Security Groups control inbound/outbound traffic

🏗️ Architecture Diagram

Internet
↓
Internet Gateway
↓
Public Subnet (EC2)
↓
NAT Gateway
↓
Private Subnet


🛠️ Technologies Used

Terraform

AWS VPC

AWS EC2

AWS NAT Gateway

AWS Internet Gateway

AWS Route Tables

AWS Security Groups

📁 Project Structure
vpc-project/
│── provider.tf
│── variables.tf
│── main.tf
│── outputs.tf

⚙️ How to Deploy
1 Clone the repository
git clone <your-repo-link>
cd vpc-project

2️ Initialize Terraform
terraform init

3️ Preview Infrastructure
terraform plan

4️ Deploy Infrastructure
terraform apply


Type yes to confirm.

🧹 How to Destroy Infrastructure

To delete all resources:

terraform destroy

🔐 Security Implementation

SSH (Port 22) enabled

HTTP (Port 80) enabled

Private subnet instances do not have direct internet access

NAT Gateway used for secure outbound traffic


👨‍💻 Author

Shiva
Aspiring DevOps / Cloud Engineer
Actively seeking entry-level opportunities
