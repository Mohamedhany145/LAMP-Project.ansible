# LAMP Stack Automation with Ansible

This project automates the installation and configuration of a LAMP (Linux, Apache, MySQL, PHP) stack using **Ansible**.
```markdown
# LAMP Stack Automation with Ansible

Automates the deployment of a LAMP (Linux, Apache, MySQL, PHP) stack using Ansible.

## Stack Components
- **Linux**: Ubuntu 20.04 LTS
- **Apache**: Web server
- **MySQL**: Database server
- **PHP**: Scripting language

## Features
- Automated LAMP stack installation
- Secure MySQL setup with configurable credentials
- Apache web server configuration
- PHP installation with validation
- Modular Ansible role structure


## Requirements
- Ansible installed on control node
- SSH access to target servers
- Ubuntu 20.04 on managed nodes

## Quick Start
1. Clone the repo:
   ```bash
   git clone https://github.com/Mohamedhany145/LAMP-Project.ansible.git
   cd LAMP-Project.ansible
   ```

2. Configure inventory:
   - Edit `hosts` file with your server IPs

3. Set variables:
   - Modify `group_vars/all.yml` with your credentials

4. Run playbook:
   ```bash
   ansible-playbook -i hosts install-lamp.yml
   ```

## Verification
- Access `http://<server-ip>` for Apache
- Check PHP with `phpinfo()`
- MySQL login: `mysql -u root -p`
