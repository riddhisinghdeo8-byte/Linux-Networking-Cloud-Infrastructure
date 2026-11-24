
# Linux Server Deployment

## 1. Introduction

Linux server deployment involves creating a virtual machine, installing Linux, configuring the system, securing access and deploying a service.

## 2. Deployment Workflow

### Step 1: Create Virtual Machine

- Create a virtual machine.
- Allocate memory and storage.
- Install Ubuntu Linux.
- Complete the initial system setup.

### Step 2: Configure Linux

Update the package repository:

```bash
sudo apt update
```

Upgrade installed packages:

```bash
sudo apt upgrade -y
```

Check system information:

```bash
uname -a
```

### Step 3: Secure Access

SSH is used for secure remote access.

Generate an SSH key:

```bash
ssh-keygen -t ed25519
```

Check SSH service:

```bash
sudo systemctl status ssh
```

### Step 4: Deploy Nginx Web Server

Install Nginx:

```bash
sudo apt install nginx -y
```

Start Nginx:

```bash
sudo systemctl start nginx
```

Enable Nginx at startup:

```bash
sudo systemctl enable nginx
```

Check Nginx status:

```bash
sudo systemctl status nginx
```

### Step 5: Test Connectivity

Check the server IP address:

```bash
hostname -I
```

Test the web server:

```bash
curl http://localhost
```

If Nginx is running correctly, the default Nginx welcome page HTML should appear.

The web server can also be tested through a browser using the appropriate server IP address.

## 3. Tools Used

- Ubuntu Linux
- Virtual Machine
- SSH
- Nginx
- Linux Terminal
- curl

## 4. Expected Result

A working Linux server with secure access and an operational Nginx web server.

## 5. Evidence

Screenshots of VM configuration, Linux setup, SSH configuration, Nginx status and connectivity testing will be added here.

## Status

## Deployment Result

- Operating System: Ubuntu Server 26.04
- Virtual Machine: Oracle VirtualBox
- Web Server: Nginx
- Network Mode: NAT
- Port Forwarding: Host 8080 → Guest 80
- Firewall: UFW
- Website Status: Successfully deployed
- Testing: Accessed through http://localhost:8080
- Verification: Nginx welcome page displayed successfully.

Documentation Added – Deployment Evidence Pending
