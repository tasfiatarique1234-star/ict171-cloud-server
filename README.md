# ICT171 Cloud Server Project

## Student Information
- Name: Tasfia Tarique
- Student Number: 35674474
- Unit: ICT171 Introduction to Server Environments and Architectures
## Server Access Information
- Public IP Address: 151.158.219.97
- DNS Entry: tasfiaict171.xyz
- Website Link: https://tasfiaict171.xyz
- GitHub Repository: https://github.com/tasfiatarique1234-star/ict171-cloud-server

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
| Public IP Address | 151.158.219.97 |

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

DNS Configuration

Domain Name:
tasfiaict171.xyz

A Record:
151.158.219.97

The DNS A Record was configured in Namecheap to point the domain name to the public IP address of the Ubuntu cloud server.
## Website Pages

The website contains multiple pages to provide project information and server details:

Home Page (index.html)

About This Project (about.html)

Server Status (status.html)

Project Information (project.html)

These pages demonstrate basic website navigation and provide information about the cloud server deployment.


---

# Commands Used

SSH Connection

ssh -i 35674474.key ubuntu@151.158.219.97

This command was used to securely connect to the Ubuntu cloud server for administration and configuration tasks.

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
-SSH connection to server
- Nginx installation
- Custom homepage
- About This Project page
- Server Status page
- Project Information page
- Domain configuration
- HTTPS SSL configuration
  
## Script
```
#!/bin/bash

# ICT171 Server Health Check Script
# This script checks whether Nginx is running and whether the website is reachable through HTTPS.

echo "Checking Nginx service..."

if systemctl is-active --quiet nginx
then
    echo "Nginx is running."
else
    echo "Nginx is not running."
fi

echo ""

echo "Checking website availability..."

if curl -s https://tasfiaict171.xyz > /dev/null
then
    echo "Website is reachable."
else
    echo "Website is not reachable."
fi

echo ""

echo "Server health check completed."
```






## Script Explanation

This Bash script performs a basic server health check. It verifies whether the Nginx web server is active and checks if the website is accessible through HTTPS. The script helps administrators quickly confirm that the server and website are operating correctly and can assist with troubleshooting if issues occur.

## Script Verification

The website used to verify the script output can be accessed at:

https://tasfiaict171.xyz

The script checks that the website is reachable over HTTPS and confirms that the Nginx service is operational.
## Script Output

Example successful output:

Checking Nginx service...
Nginx is running.

Checking website availability...
Website is reachable.

Server health check completed.



---

# Conclusion

This project successfully demonstrated the deployment and management of a Linux cloud server environment using Ubuntu and Nginx. DNS configuration, HTTPS security implementation, and server administration skills were developed through the completion of this project.
## References

Documentation - Let’s Encrypt. (n.d.). Letsencrypt.org. https://letsencrypt.org/docs/

Installing nginx. (n.d.). Nginx.org. https://nginx.org/en/docs/install.html

SCH-IT-MurdochUni. (2025). NetworkingLabs/Server_Environments_and_Architectures/dns.md at main · SCH-IT-MurdochUni/NetworkingLabs. GitHub. https://github.com/SCH-IT-MurdochUni/NetworkingLabs/blob/main/Server_Environments_and_Architectures/dns.md

