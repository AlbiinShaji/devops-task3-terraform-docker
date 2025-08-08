 DevOps Task 3 – Infrastructure as Code (IaC) with Terraform

## Objective

Provision a local Docker container (NGINX) using Terraform as part of the DevOps Internship.

## Tools Used

- [Terraform](https://www.terraform.io/)
- [Docker](https://www.docker.com/)

## Steps Performed

1. Created a `main.tf` file using the **Docker provider** in Terraform.
2. Configured Terraform to:
   - Pull the `nginx:latest` Docker image
   - Create a Docker container from that image
   - Map container port `80` to host port `8080`
3. Ran:
   ```bash
   terraform init
   terraform plan
   terraform apply
   ```

Verified NGINX was running at http://localhost:8080.

Destroyed the infrastructure using:

terraform destroy

**Folder Contents**
main.tf – Terraform configuration file

terraform-init-log.txt – Output of terraform init

terraform-plan-log.txt – Output of terraform plan

terraform-apply-log.txt – Output of terraform apply

terraform-destroy-log.txt – Output of terraform destroy

**Outcome**
Successfully provisioned and destroyed a Docker container using Terraform, gaining hands-on experience with Infrastructure as Code.
