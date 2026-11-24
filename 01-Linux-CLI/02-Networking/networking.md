
# Networking Fundamentals – Practical Documentation

## 1. Introduction

Computer networking allows devices and servers to communicate and exchange data over a network.

## 2. IP Addressing

An IP address is a unique numerical address assigned to a device on a network.

Command:

```bash
ip addr
```

Displays network interfaces and their IP addresses.

```bash
ip route
```

Displays the system's routing table.

## 3. DNS (Domain Name System)

DNS translates domain names into IP addresses.

Commands:

```bash
nslookup google.com
```

```bash
ping google.com
```

These commands help check DNS resolution and network connectivity.

## 4. Network Ports

Ports allow different services to communicate over a network.

Common ports:

| Port | Service |
|---|---|
| 22 | SSH |
| 53 | DNS |
| 80 | HTTP |
| 443 | HTTPS |
| 3306 | MySQL |

Command:

```bash
ss -tuln
```

Displays listening TCP and UDP ports.

## 5. Firewall Configuration

A firewall controls incoming and outgoing network traffic.

Ubuntu uses UFW (Uncomplicated Firewall) as a firewall management tool.

Useful commands:

```bash
sudo ufw status
sudo ufw status verbose
sudo ufw allow 22/tcp
sudo ufw allow 80/tcp
```

Note: Firewall rules will be tested during server configuration. SSH access should be secured before enabling a firewall on a remote server.

## 6. Security Groups

Security groups are virtual network firewalls used by cloud platforms.

They control inbound and outbound traffic through rules based on:

- Protocol
- Port number
- Source IP address
- Destination IP address

## 7. Tools Used

- ip
- ping
- nslookup
- ss
- UFW
- curl

## 8. Practical Environment

Operating System: Ubuntu Linux

Terminal: Ubuntu on Windows (WSL)

## 9. Result

Networking commands and concepts for IP addressing, DNS, ports, firewalls and security groups are documented for practical implementation.

## Status

## Practical Results

- Checked server IP address using hostname -I and ip addr.
- Tested DNS resolution using nslookup google.com.
- Checked listening network ports using ss.
- Configured UFW firewall.
- Allowed HTTP traffic on port 80.
- Allowed SSH traffic using OpenSSH.
- Configured VirtualBox NAT port forwarding (8080 → 80).
- Tested website connectivity from Windows browser.

Documentation Added – Practical Verification Pending
