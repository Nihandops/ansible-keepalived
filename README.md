# Ansible Keepalived Installation Example

This is a beginner-friendly Ansible project that demonstrates how to automate the installation and configuration of **Keepalived** on multiple servers. The project is designed to help new users understand how Ansible works, including basic configuration and deployment tasks.

## Overview

This project includes an example Ansible playbook for installing **Keepalived**, a Linux-based high availability solution for load balancing and failover. The playbook can be applied to multiple servers at once, saving time and reducing manual intervention.

### Requirements

- **Ansible**: This project requires Ansible to be installed on the control machine (your Ansible server).
  
  **To install Ansible on CentOS 7:**
  ```bash
  yum install ansible

  SSH access to the target servers: Ensure that the control machine (Ansible server) can access other target servers via SSH using the root user or another privileged user with the correct SSH keys.

Project Structure
hosts.ini: This file contains the inventory of the target servers. It includes the IP addresses of all the servers where Keepalived will be installed.

install_keepalived.yml: This Ansible playbook installs and configures Keepalived on all target servers listed in the inventory. It ensures that the package is installed, updated, and that the Keepalived service is running and enable
Setup
Clone this repository:
git clone https://github.com/yourusername/ansible-keepalived.git
cd ansible-keepalived
Configure SSH access: Make sure you can access the target servers via SSH from your Ansible server. Update the hosts.ini file to include the correct IP addresses for your servers.

Update the playbook (optional): If you want to customize the Keepalived configuration, you can modify the install_keepalived.yml playbook accordingly.

Usage
Navigate to the project directory:
cd /path/to/ansible-keepalived
Run the Ansible playbook:
ansible-playbook -i hosts.ini install_keepalived.yml


