# ICT171 Cloud Server Project

## Student Information
- Name: Tasfia Tarique
- Unit: ICT171 Introduction to Server Environments and Architectures

---

# Project Overview

This project demonstrates the deployment and configuration of a cloud-hosted Ubuntu Linux web server using Nginx. The server was configured with a custom domain name and secured using HTTPS with Let's Encrypt SSL certificates.

---

# Server Information

| Component | Details |
|---|---|
| Operating System | Ubuntu 24.04 LTS |
| Web Server | Nginx |
| Domain Name | tasfiaict171.xyz |
| SSL Certificate | Let's Encrypt |
| Cloud Environment | ICT171 Private Cloud |

---

# Website Setup

The following tasks were completed:

- Connected to the Ubuntu server using SSH
- Updated Ubuntu system packages
- Installed and configured Nginx
- Created a custom HTML webpage
- Registered and configured a custom domain
- Configured DNS A records
- Installed SSL certificates using Certbot
- Enabled HTTPS secure communication

---

# Commands Used

## System Update

```bash
sudo apt update && sudo apt upgrade -y
```

## Install Nginx

```bash
sudo apt install nginx -y
```

## Install SSL Packages

```bash
sudo apt install certbot python3-certbot-nginx -y
```

## Configure HTTPS SSL

```bash
sudo certbot --nginx -d tasfiaict171.xyz
```

---

# Website Access

## HTTP Version
http://tasfiaict171.xyz

## HTTPS Version
https://tasfiaict171.xyz

---

# Screenshots

Screenshots included:
- SSH connection to server
- Nginx installation
- Custom webpage
- Domain configuration
- HTTPS SSL configuration

---

# Conclusion

This project successfully demonstrated the deployment and management of a Linux cloud server environment using Ubuntu and Nginx. DNS configuration, HTTPS security implementation, and server administration skills were developed through the completion of this project.
# ICT171 Cloud Server Project

## Student Information
- Name: Tasfia Tarique
- Unit: ICT171 Introduction to Server Environments and Architectures

## Project Overview
This project demonstrates the deployment of a cloud-hosted Ubuntu Linux web server using Nginx and HTTPS.

## Website Link
https://tasfiaict171.xyz

## GitHub Repository
https://github.com/tasfiatarique1234-star/ict171-cloud-server
