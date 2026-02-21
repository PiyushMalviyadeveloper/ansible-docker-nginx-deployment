# Ansible Docker Nginx Deployment Project

# Project Overview
Automated deployment of an Nginx container using Ansible with conditional Docker installation logic on a remote Linux server.

---

# Infrastructure Setup

This project was implemented using **two machines**:

# Control Node
- Installed Ansible
- Maintains inventory file
- Executes playbooks
- Connects to target via SSH

# Target Node
- RHEL/CentOS-based Linux system
- Docker Engine (installed conditionally if absent)
- Firewalld enabled
- Runs Nginx container

---

# Workflow Execution

1. Ansible connects to Target Node via SSH.
2. Checks whether Docker is installed.
3. If Docker is not installed:
   - Adds official Docker CE repository
   - Installs Docker packages
   - Starts and enables Docker service
4. Pulls the official Nginx image from Docker Hub.
5. Deploys Nginx container on port **8080**.
6. Configures firewall to allow HTTP traffic.
7. Verifies container is running.

---

#:# 🏗 Architecture Diagram
