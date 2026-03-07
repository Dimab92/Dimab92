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
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?logo=terraform&logoColor=white&style=for-the-badge&logoWidth=30)

## Virtualization | Bash and Bash Scripting:
VirtualBox hypervisor: VM installation, configuration, and management

Installing and configuring UNIX-based OS in virtual environments

System updates and package management via CLI

Setting up essential server tools required for server functionality

Experience writing Bash scripts to automate routine tasks like backups, cron jobs, and system maintenance

Troubleshooting: identifying and resolving system, network, and application issues to ensure smooth operations

## Docker and Docker Compose:
Full Dockerization of the application with Nginx or Nginx + Traefik as a reverse proxy

Multi-container architecture using Docker Compose with services: Backend API, Frontend app, PostgreSQL, Reverse Proxy


## GitHub Actions:
Creating CI pipelines for backend, frontend, nginx, traefik, custom scripts using GitHub Actions:

Covering the full CI flow: code checkout, linting, testing, Docker image build, and saving images as artifacts

Configuring support for both GitHub-hosted and self-hosted runners, following security and CI best practices.

## AWS Integration:
Connecting GitHub to AWS and integrating ECR and S3 into CI/CD pipelines via secure, environment-specific roles

IAM: Creating IAM users with read-only access and separate service roles using the least-privilege principle

EC2 & EIP: Deploying an EC2 instance with Elastic IP and attaching a dedicated IAM role

ECR: Setting up a private ECR registry and configuring GitHub Actions to push Docker images with minimal permissions

S3 & Backups: Implementing automated backups to S3, including downloading, updating, and uploading versions.json with backup artifacts

## Cloud Deployment & Automation:
Automated the full deployment pipeline from GitHub to AWS (EC2) using GitHub Actions

Creating docker-compose-file to deploy production-ready services using prebuilt images from ECR

## Terraform | AWS Infrastructure:

### ECS Cluster:

Creating ECS cluster with EC2 capacity provider and autoscaling group vith user data

Containerized Task Definition: Deployed multi-container task with: Frontend, Backend, Traefik, PostgreSQL

Security Groups configured using the least-privilege principle

Application Load Balancer with routing to ECS services

### State Management:

Stored Terraform state in S3

Enabled state locking with DynamoDB for safe team collaboration

### CI/CD Integration:

Integrated GitHub Actions to:

Push Docker images to ECR

Update ECS task and service without downtime
