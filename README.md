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
![Git](https://img.shields.io/badge/Git-E5534B?logo=git&logoColor=white&style=for-the-badge&logoWidth=30) 
![GitHub](https://img.shields.io/badge/GitHub-24292E?logo=github&logoColor=white&style=for-the-badge&logoWidth=30) 
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-0078D7?logo=githubactions&logoColor=white&style=for-the-badge&logoWidth=30) 
![Docker](https://img.shields.io/badge/Docker-1CA7EC?logo=docker&logoColor=white&style=for-the-badge&logoWidth=30) 
![Docker Compose](https://img.shields.io/badge/Docker%20Compose-0052CC?logo=docker&logoColor=white&style=for-the-badge&logoWidth=30) 
![AWS](https://img.shields.io/badge/AWS-FF9900?logo=amazonaws&logoColor=white&style=for-the-badge&logoWidth=30)




## Virtualization and Bash:
Hypervisors: VirtualBox (installation and configuration)

Installed and configured a UNIX OS on a virtual machine

Performed system update and upgrade via command line

Installed and configured all necessary tools for server operation

## Bash Scripting:
Writing Bash scripts to automate daily tasks and make work easier.

Created one script that:

Clones GitHub repository using SSH

Makes compressed backup files with version numbers

Tracks backup info in a JSON file using jq

Deletes old backups if needed

Can run many backups in one go

## Docker and Containerization:
Wrote a Dockerfile to run the backup script inside a container

Used Docker volumes to keep backup files safe and outside the container

Used environment variables to protect sensitive data

Backups are saved to the host system so they are not lost when the container stops

## Docker Compose:
Created Dockerfiles for backend and frontend applications
Built multi-container architecture using Docker Compose

Configured services for:

Backend API

Frontend app

PostgreSQL database

Nginx as reverse proxy

Wrote Nginx config to route requests between frontend and backend
Used environment variables to manage settings across services
Connected services using Docker networks
Mapped ports to access the app in browser

## CI/CD with GitHub Actions:
Created pipelines for backend, frontend, nginx, and backup using GitHub Actions

For each component:

Wrote separate workflows triggered by code changes (push/PR to specific folders)

Used workflow_dispatch to allow manual launch with choice of runner

Configured support for both GitHub-hosted and self-hosted runners

Added custom names and dropdown menu for clarity and flexibility

Backend pipeline:

Linting with ruff

Running tests with python manage.py test and env variables

Building Docker image with two tags: latest and short Git SHA

Saving Docker image as artifact (1-day retention)

Frontend pipeline:

Linting with npm run lint

Testing with npm run test

Building Docker image tagged latest

Saving image as artifact (1-day retention)

Nginx pipeline:

Building Docker image with latest and short Git SHA tags

Saving image as artifact (1-day retention)

Backup pipeline:

Running backup.sh script

Checking versions.json from previous artifact and appending data

Saving both backup archive and updated versions.json as separate artifacts (5-day retention)

## Cloud & AWS Services:
Configured and secured cloud infrastructure using AWS Console and GitHub Actions

IAM & User Management:

Created and configured IAM users with read-only permissions for multiple team members

Used least privilege principle to assign roles and permissions

Compute (EC2):

Deployed a Virtual Machine (EC2) instance with Elastic IP

Attached custom IAM role to allow secure ECR access

Container Registry (ECR):

Created and configured a private ECR registry

Built secure GitHub Actions pipeline to push Docker images to ECR using minimal IAM permissions

Storage (S3):

Created an S3 bucket named devops-intern-$GITHUB_USERNAME

Modified backup.sh pipeline to:

Download versions.json from S3

Update backup metadata

Upload updated versions.json and archive to S3

CI/CD Integration with GitHub:

Connected GitHub to AWS using OIDC (OpenID Connect) for secure, token-based access (no secrets exposed)

Integrated AWS services into CI/CD pipeline using environment-specific roles
