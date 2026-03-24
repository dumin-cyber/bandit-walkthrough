# Bandit Level 0

## 🎯 Objective
Log into the Bandit game server using SSH.

## 🔍 Approach
To access the system, I used Secure Shell (SSH), a protocol that allows remote access to a machine over a network.

The challenge provided the necessary credentials:
- Username
- Host
- Port
- Password

Using this information, I established a remote connection to the target machine.

## 💻 Command Used
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
