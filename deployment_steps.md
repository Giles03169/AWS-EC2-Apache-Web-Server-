# Deployment Steps for AWS EC2 Apache Web Server

This document details the step-by-step process used to deploy an Apache web server on an AWS EC2 instance.

---

## 1. Launch EC2 Instance
- Go to AWS Management Console → EC2 → Launch Instance
- AMI: **Ubuntu Server 24.04 LTS (Free Tier Eligible)**
- Instance type: **t3.micro**
- Key pair: Create or use an existing key (e.g., `deploykey.pem`)
- Configure security group:
  - Allow **SSH (port 22)** from your IP
  - Allow **HTTP (port 80)** from anywhere (0.0.0.0/0)
- Launch the instance.

---

## 2. Connect to EC2 Instance
- Open Terminal (Mac/Linux) or Git Bash (Windows).
- Set permissions for the key:
  ```bash
  chmod 400 /path/to/mydeploykey.pem
  ssh -i /path/to/deploykey.pem ubuntu@13.61.181.171
  sudo apt update
  sudo apt install apache2 -y
  sudo systemctl status apache2
