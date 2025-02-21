# Ansible Automation for Hetzner Cloud Infrastructure

This repository contains Ansible playbooks for automating the deployment and management of services on Hetzner Cloud infrastructure. The playbooks are designed to simplify the setup and configuration of various services including Nginx Proxy Manager and SABnzbd.

## 🚀 Features

- Automated server creation and configuration in Hetzner Cloud
- Nginx Proxy Manager deployment and configuration
- SABnzbd server setup
- DNS management for Hetzner DNS
- SSL certificate management
- Server cleanup and removal capabilities

## 📋 Prerequisites

- Ansible installed on your local machine
- Hetzner Cloud account and API token
- Basic understanding of Ansible playbooks
- Python 3.x

## 🗂️ Repository Structure

```
.
├── playbooks/
│   ├── create-hc-nginx-proxy-manager.yaml  # Creates and configures Nginx Proxy Manager
│   ├── create-hc-sabnzbd-server.yaml      # Sets up SABnzbd server
│   ├── add-domain-ssl-npm.yaml            # Manages SSL certificates
│   ├── hetzner_dns_management.yaml        # Handles DNS records
│   └── remove-hc-server.yaml              # Removes Hetzner Cloud servers
```

## 🛠️ Usage

### Setting up Nginx Proxy Manager

```bash
ansible-playbook playbooks/create-hc-nginx-proxy-manager.yaml
```

### Deploying SABnzbd Server

```bash
ansible-playbook playbooks/create-hc-sabnzbd-server.yaml
```

### Managing SSL Certificates

```bash
ansible-playbook playbooks/add-domain-ssl-npm.yaml
```

### Managing DNS Records

```bash
ansible-playbook playbooks/hetzner_dns_management.yaml
```

### Removing a Server

```bash
ansible-playbook playbooks/remove-hc-server.yaml
```

## ⚙️ Configuration

Before running the playbooks, ensure you have:

1. Set up your Hetzner Cloud API token
2. Configured your DNS settings if using Hetzner DNS
3. Updated any necessary variables in the playbooks

## 🔒 Security

- API tokens and sensitive information should be stored securely
- Use environment variables or Ansible vault for sensitive data
- Follow security best practices when deploying services

## 📝 License

This project is licensed under the terms of the included LICENSE file.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## ⚠️ Disclaimer

Please test these playbooks in a non-production environment first. Always backup your data before making changes to your infrastructure.
