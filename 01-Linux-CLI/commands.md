
# Linux CLI Practical Commands

## 1. Introduction

Linux Command Line Interface (CLI) allows users to interact with the operating system using text-based commands.

## 2. File and Directory Management

| Command | Description |
|---|---|
| pwd | Displays current directory |
| ls | Lists files and directories |
| cd | Changes directory |
| mkdir | Creates a directory |
| touch | Creates an empty file |
| cp | Copies files |
| mv | Moves or renames files |
| rm | Removes files |

## 3. File Permissions

| Command | Description |
|---|---|
| chmod | Changes file permissions |
| chown | Changes file ownership |
| ls -l | Displays file permissions |

Example:

```bash
chmod 755 filename
chmod 644 filename
```

## 4. User and Group Management

| Command | Description |
|---|---|
| whoami | Displays current username |
| id | Displays user and group IDs |
| sudo adduser username | Creates a user |
| groups | Displays group membership |
| sudo groupadd groupname | Creates a group |

## 5. Process Management

| Command | Description |
|---|---|
| ps | Displays running processes |
| top | Monitors system processes |
| kill | Terminates a process |
| systemctl | Manages system services |

## 6. SSH Configuration

SSH (Secure Shell) provides secure remote access to Linux systems.

Example:

```bash
ssh-keygen -t ed25519
```

This generates an SSH key pair for secure authentication.

## 7. Practical Environment

Operating System: Ubuntu Linux

Terminal: Ubuntu on Windows (WSL)

## 8. Result

Linux command-line operations, file management, permissions, user management, process management and SSH key generation were practised.

## Status

Completed
