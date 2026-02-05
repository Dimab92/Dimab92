# Hi there 👋 I have hands-on experience with:

<!--
**Dimab92/Dimab92** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
![VirtualBox](https://img.shields.io/badge/VirtualBox-8A2BE2?logo=virtualbox&logoColor=white&style=for-the-badge&logoWidth=30)
![Bash](https://img.shields.io/badge/Bash-7ED957?logo=gnu-bash&logoColor=white&style=for-the-badge&logoWidth=30) 
![Bash scripting](https://img.shields.io/badge/Bash%20Scripting-2E8B57?logo=gnubash&logoColor=white&style=for-the-badge&logoWidth=30) 
![Networking](https://img.shields.io/badge/Networking-F4D35E?logo=cloudflare&logoColor=white&style=for-the-badge)
![Apache](https://img.shields.io/badge/Apache-D22128?style=for-the-badge&logo=apache&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git-E5534B?logo=git&logoColor=white&style=for-the-badge&logoWidth=30) 
![GitHub](https://img.shields.io/badge/GitHub-24292E?logo=github&logoColor=white&style=for-the-badge&logoWidth=30) 
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-0078D7?logo=githubactions&logoColor=white&style=for-the-badge&logoWidth=30) 
![Docker](https://img.shields.io/badge/Docker-1CA7EC?logo=docker&logoColor=white&style=for-the-badge&logoWidth=30) 
![Docker Compose](https://img.shields.io/badge/Docker%20Compose-0052CC?logo=docker&logoColor=white&style=for-the-badge&logoWidth=30) 
![AWS](https://img.shields.io/badge/AWS-FF9900?logo=amazonaws&logoColor=white&style=for-the-badge&logoWidth=30)


## Virtualization | Bash and Bash Scripting:
VirtualBox hypervisor: installation, configuration, and management of virtual machines

Installing and configuring UNIX-based OS in a virtualized environment

Performing system updates and package upgrades using the command line

Setting up and configuring essential tools required for server functionality

Experience writing Bash scripts to automate routine tasks like backups, cron jobs, and system maintenance

Troubleshooting: identifying and resolving system, network, and application issues to ensure smooth operations

## Docker and Docker Compose:
Full Dockerization of the application with Nginx or Traefik configured as a reverse proxy

Building multi-container architecture using Docker Compose

Configured services for:

Backend API

Frontend app

PostgreSQL database

Nginx or Traefik as reverse proxy

## GitHub Actions:
Creating CI pipelines for backend, frontend, nginx, traefik, custom scripts using GitHub Actions:

Covering the full CI flow: code checkout, linting, testing, Docker image build, and saving images as artifacts

Configuring support for both GitHub-hosted and self-hosted runners, following security and CI best practices.

## AWS Integration:
Configured and secured cloud infrastructure using AWS Console and GitHub Actions

IAM:

Created and configured IAM users with read-only permissions for multiple team members

Used least privilege principle to assign roles and permissions

EC2:

Deployed a Virtual Machine (EC2) instance with Elastic IP

Attached custom IAM role to allow secure ECR access

ECR:

Created and configured a private ECR registry

Built secure GitHub Actions pipeline to push Docker images to ECR using minimal IAM permissions

S3:

Created an S3 bucket 

Modified backup.sh pipeline to:

Download versions.json from S3

Update backup metadata

Upload updated versions.json and archive to S3

CI/CD Integration with GitHub:

Connected GitHub to AWS

Integrated AWS services into CI/CD pipeline using environment-specific roles

## Cloud Deployment & Automation:
Automated the full deployment pipeline from GitHub to cloud VM using Docker and GitHub Actions.

Docker Compose (Production):

Created docker-compose-prod.yaml to deploy production-ready services (Nginx, Backend, Frontend) using prebuilt images from private container registry

Ensured separation of development and production environments

## Infrastructure as Code (IaC) with Terraform:
Provisioned production-grade infrastructure on AWS using Terraform with focus on scalability, automation, and cost-efficiency (Free Tier).

### Key Components Deployed:

ECS Cluster: Created ECS cluster terraform-ecs-cluster-$GITHUB_USERNAME with EC2 capacity provider and autoscaling group (bootstrapped via user data)

Containerized Task Definition: Deployed multi-container task with:

Frontend

Backend

Nginx

PostgreSQL database

Security Groups: Designed using least-privilege principle

Application Load Balancer (ALB): Configured listener rules and health checks for seamless routing to ECS tasks

### State Management:

Stored Terraform state in S3

Enabled state locking with DynamoDB for safe team collaboration

### CI/CD Integration:

Integrated GitHub Actions to:

Trigger deployment on push to main or workflow_dispatch

Push Docker images to ECR

Update ECS task and service without downtime

Retained workflow naming for consistent automation control

### Best Practices:

Defined Terraform version for stability

Used cost-effective Free Tier AWS instances

Removed old EC2 + Elastic IP setup after migration to ECS

Application successfully served via Load Balancer DNS
