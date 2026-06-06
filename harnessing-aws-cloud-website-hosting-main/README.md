# Harnessing EC2, VPC & MobaXterm for Cutting-Edge Entity Hosting

## Project Overview

This project demonstrates cloud-based website hosting using AWS EC2, Ubuntu Server, Apache Web Server, and MobaXterm.

The objective of this project is to deploy and host a website securely on AWS cloud infrastructure using EC2 instances within a Virtual Private Cloud (VPC).

The project includes:
- EC2 instance creation
- VPC and security group configuration
- SSH connectivity using MobaXterm
- Apache web server installation
- Website deployment using HTML/CSS
- Public website hosting using EC2 public IP

---

## Technologies Used

- AWS EC2
- AWS VPC
- Ubuntu Server
- Apache2
- MobaXterm
- HTML5
- CSS3

---

## Project Architecture

Infrastructure Layer → AWS EC2 & VPC

Server Layer → Ubuntu + Apache Web Server

Management Layer → MobaXterm SSH & SFTP

Presentation Layer → HTML/CSS Website

---

## Features

- Cloud-based website hosting
- Secure SSH access
- Apache web server configuration
- Website deployment using EC2
- Public website accessibility
- Secure file transfer using SFTP

---

## Installation & Deployment Steps

### Step 1 — Launch EC2 Instance

- Create Ubuntu EC2 instance on AWS
- Enable ports:
  - SSH (22)
  - HTTP (80)
  - HTTPS (443)

### Step 2 — Connect Using MobaXterm

Use:
- Public IPv4 address
- PEM key
- Username: ubuntu

### Step 3 — Install Apache

```bash
sudo apt update
sudo apt install apache2 -y
```

### Step 4 — Upload Website Files

Upload:
- index.html
- style.css

to:

```bash
/var/www/html
```

### Step 5 — Restart Apache

```bash
sudo systemctl restart apache2
```

### Step 6 — Launch Website

Open:

```bash
http://YOUR_PUBLIC_IP
```

---

## Future Enhancements

- SSL Certificate Integration
- Custom Domain Hosting
- Load Balancer Integration
- Auto Scaling
- CloudWatch Monitoring
- CI/CD Pipeline

---

## Author

Snehal Subhash Mali