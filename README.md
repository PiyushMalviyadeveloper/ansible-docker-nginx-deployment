#Ansible Docker Nginx Deployment Project

#Project Overview
Automated deployment of an Nginx container using Ansible with conditional Docker installation logic.

#Technologies Used
- Ansible
- Docker CE
- Nginx
- Firewalld
- Linux (RHEL/CentOS)

#Features
- Conditional Docker installation
- Official Docker CE repo configuration
- Idempotent deployment
- Automatic firewall configuration
- Containerized web server deployment

#How to Run

ansible-playbook -i inventory deploy.yml

#Access

http://<server-ip>:8080

#What I Learned
- Infrastructure as Code (IaC)
- Ansible Playbook development
- Docker automation
- Conditional task execution
- Production-style debugging
