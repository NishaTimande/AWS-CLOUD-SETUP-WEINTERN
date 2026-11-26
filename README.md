# AWS-CLOUD-SETUP-WEINTERN
# AWS EC2 - Nginx Web Server Setup

## Project Overview
In this project, an Ubuntu Server was launched on AWS EC2 and Nginx Web Server was installed on it.

## Architecture / Details
- **Cloud:** AWS
- **Service:** EC2
- **OS:** Ubuntu 22.04 LTS
- **Instance Type:** t2.micro (Free Tier)
- **Web Server:** Nginx 1.24.0
- **Public IP:** 32.237.98.212

## Implementation Steps

### 1. Log in to AWS Console and navigate to EC2
Logged in to AWS Console and opened EC2 Service.

### 2. Launch Instance - Ubuntu 22.04 LTS
Clicked on Launch Instance and selected Ubuntu 22.04 LTS (Free Tier).

### 3. Choose t2.micro Instance Type
Selected t2.micro which is available in Free Tier.

### 4. Create Key Pair
Created a new Key Pair and downloaded the `.pem` file.

### 5. Configure Security Group
- SSH (Port 22) - My IP
- HTTP (Port 80) - Anywhere (0.0.0.0/0)

### 6. Review and Launch Instance
Checked all settings and Launched the Instance.

### 7. Connect via SSH
```bash
ssh -i "key.pem" ubuntu@32.237.98.212
