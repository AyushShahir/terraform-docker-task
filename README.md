## 🚀 Terraform Docker Infrastructure

## 🎓 DevOps Internship — Task 3

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision and manage a local Docker container running NGINX.

## 🎯 Objective

The objective of this task is to:

🏗️ Understand the concept of Infrastructure as Code (IaC)

⚙️ Use Terraform to define infrastructure

🐳 Provision a Docker container using Terraform

🔄 Understand the Terraform workflow

🧹 Provision and destroy infrastructure using code

## 🛠️ Technologies Used

🟣 Terraform

🐳 Docker

🌐 NGINX

🐙 Git

☁️ GitHub

## 🏗️ Architecture

                 Terraform
                     │
                     ▼
              Docker Provider
                     │
                     ▼
             NGINX Docker Image
                     │
                     ▼
             Docker Container
             (terraform-nginx)
                     │
                     ▼
              localhost:8081

## 📁 Project Structure
```text

terraform-docker-iac-task/
│
├── 📄 main.tf
├── 📄 README.md
├── 📄 .gitignore
├── 📄 .terraform.lock.hcl
│
└── 📁 screenshots/
    ├── terraform-plan.png
    ├── terraform-apply.png
    ├── docker-ps.png
    ├── nginx-browser.png
    ├── terraform-state.png
    └── terraform-destroy.png
```

## 🔒 Terraform state files and the .terraform directory are excluded from Git using .gitignore.

## 🔄 Terraform Workflow

The following Terraform commands were used during the task:

1️⃣ Initialize Terraform

terraform init

Initializes the Terraform working directory and downloads the required provider.

2️⃣ Format the Configuration

terraform fmt

Formats the Terraform configuration file according to standard formatting.

3️⃣ Validate the Configuration

terraform validate

Checks whether the Terraform configuration is syntactically valid and correctly configured.

4️⃣ Preview Infrastructure Changes

terraform plan

Creates an execution plan showing what Terraform will create, modify, or destroy.

5️⃣ Create the Infrastructure

terraform apply

Applies the Terraform configuration and creates the required Docker resources.

6️⃣ Check Terraform State

terraform state list

Displays the resources currently tracked by Terraform.

7️⃣ Destroy the Infrastructure

terraform destroy

Removes the infrastructure managed by Terraform.

## 🐳 Resources Created

Terraform created two resources:

🖼️ NGINX Docker Image

📦 NGINX Docker Container

📦 Container Details

Property

Value

Container Name

terraform-nginx

Container Image

nginx:latest

Internal Port

80

Host Port

8081

Access URL

http://localhost:8081

## 🌐 Application Verification

After running terraform apply, the NGINX container was verified using:

docker ps

The application was then accessed through:

http://localhost:8081

The NGINX welcome page confirmed that the container was running successfully. ✅

## 🗂️ Terraform State

Terraform maintains a state file to keep track of the infrastructure it manages.

The following resources were tracked:

docker_container.nginx
docker_image.nginx

They were verified using:

terraform state list

## 🧹 Cleanup

After completing the verification, the infrastructure was removed using:

terraform destroy

This successfully removed the Terraform-managed Docker resources. ✅

## 📸 Screenshots

The project includes screenshots demonstrating the execution and verification of the Terraform workflow.

📋 Terraform Plan

Shows the resources Terraform planned to create.

🚀 Terraform Apply

Shows the successful creation of the Docker image and container.

🐳 Docker Container

Shows the running terraform-nginx container using:

docker ps

🌐 NGINX Application

Shows the NGINX application running at:

http://localhost:8081

🗂️ Terraform State

Shows the resources tracked by Terraform using:

terraform state list

🧹 Terraform Destroy

Shows the successful removal of the Terraform-managed infrastructure.

## 🧠 Key Concepts Learned

Through this task, I learned:

🏗️ Infrastructure as Code (IaC)

🔌 Terraform Providers

📦 Terraform Resources

🗂️ Terraform State

⚙️ terraform init

✨ terraform fmt

✅ terraform validate

🔍 terraform plan

🚀 terraform apply

📋 terraform state list

🧹 terraform destroy

🐳 Docker container provisioning using Terraform

## 💡 What I Learned

This task helped me understand how infrastructure can be defined and managed using code instead of manually configuring resources.

I also learned the complete Terraform workflow:

Write Configuration
       ↓
terraform init
       ↓
terraform fmt
       ↓
terraform validate
       ↓
terraform plan
       ↓
terraform apply
       ↓
Verify Resources
       ↓
terraform state list
       ↓
terraform destroy

## 🎓 Internship Task

DevOps Internship — Task 3

Infrastructure as Code (IaC) with Terraform

🚀 Successfully provisioned a local Docker container using Terraform and verified the deployment using Docker and Terraform commands.

⭐ Built as part of my DevOps learning journey.
