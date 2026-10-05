# Terraform Docker Infrastructure

## DevOps Internship - Task 3

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision a local Docker container.

## Objective

Provision a local Docker container using Terraform.

## Technologies Used

- Terraform
- Docker
- NGINX
- Git & GitHub

## Architecture

```text
Terraform
    |
    v
Docker Provider
    |
    v
Docker Image (NGINX)
    |
    v
Docker Container
    |
    v
localhost:8081
Terraform Workflow
```

## The following Terraform commands were used:

terraform init
terraform fmt
terraform validate
terraform plan
terraform apply
terraform state list
terraform destroy
Resources Created

Terraform created two resources:

NGINX Docker image
NGINX Docker container

The container was named:

terraform-nginx

The container's port 80 was mapped to port 8081 on the host.

The application was accessed using:

http://localhost:8081
Terraform State

The following resources were tracked by Terraform:

docker_container.nginx
docker_image.nginx
Verification

The Docker container was verified using:

docker ps

Terraform resources were verified using:

terraform state list
Cleanup

After verification, the infrastructure was removed using:

terraform destroy

This successfully removed the Terraform-managed Docker image and container.

## Key Concepts Learned
Infrastructure as Code (IaC)
Terraform providers
Terraform resources
Terraform state
terraform init
terraform validate
terraform plan
terraform apply
terraform destroy
Docker and container provisioning using Terraform