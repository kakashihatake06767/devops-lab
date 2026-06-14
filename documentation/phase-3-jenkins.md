Phase 3 - Jenkins CI/CD Foundation
Objective

Implement Jenkins as the CI/CD controller for the DevOps Lab and establish communication between GitHub, Jenkins, and the application server.

Infrastructure
Servers
devops-control
jenkins-server
app-server
monitor-server
Technologies Used
Ubuntu Server
Git
GitHub
Jenkins
SSH
Docker
Docker Compose
Tasks Completed
Jenkins Installation
Installed OpenJDK 21
Installed Jenkins
Enabled Jenkins service
Verified Jenkins running on port 8080
GitHub Integration
Generated SSH key for Jenkins user
Added Deploy Key to GitHub repository
Verified GitHub authentication
Jenkins Pipeline

Created first Jenkins Pipeline using Jenkinsfile.

Pipeline stages:

Repository Check
SSH To App Server
Docker Verification
Jenkins Remote Access

Verified Jenkins can execute commands on app-server through SSH.

Test performed:

hostname

Output:

app-server

Docker Verification

Verified Jenkins can execute Docker commands remotely.

Command executed:

docker ps

Successfully retrieved running containers from app-server.

Skills Learned
Jenkins Concepts
Jenkins Dashboard
Jenkins Jobs
Jenkins Pipelines
Jenkinsfile
Pipeline Stages
Workspace
GitHub Integration
Deploy Keys
Repository Access
Source Code Management
SSH Automation
Passwordless Authentication
Remote Command Execution
Docker Operations
Container Verification
Remote Docker Management
Current Architecture

GitHub
↓
Jenkins Server
↓ SSH
app-server
↓
Docker Engine
↓
Flask + MySQL Containers

Outcome

Successfully established an automated CI pipeline capable of:

Pulling source code from GitHub
Executing Jenkins pipelines
Connecting to remote servers through SSH
Managing Docker workloads on the application server

Ready for next phase:

Automatic Application Deployment (CI/CD)
