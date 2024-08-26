# Born2beRoot

## Introduction
- This is one of 42 Seoul subjects.
- The purpose of this project is to set up a Linux Operating System on a virtual machine.
- For this project, I chose 'Debian' as the operating system and 'VirtualBox' as the virtual machine.
- The virtual machine is not saved in the git repository due to its large file size.
- Only the monitoring shell script remains, which is executed by cron on Linux.
- For more details, please refer to the [Subject PDF](requirements/subject.pdf).

## Project Overview
This project aims to introduce the world of virtualization. It involves creating a machine in VirtualBox (or UTM if VirtualBox can't be used) under specific instructions, setting up an operating system while implementing strict rules.

## Required Concepts
- Virtual Machine
- Linux Operating System
- Firewall (UFW)
- Logical Volume Manager (LVM)
- SSH (Secure Shell)
- Sudo (Super User Do)
- Port Forwarding

## Key Components
1. **Operating System**: Latest stable version of Debian
2. **Partitioning**: At least 2 encrypted partitions using LVM
3. **SSH Service**: Running on port 4242 only
4. **Firewall**: UFW with only port 4242 open
5. **Hostname**: login42 (e.g., jsmith42)
6. **Password Policy**: Strong password rules implemented
7. **Sudo**: Configured with strict rules
8. **Monitoring Script**: Displays system information every 10 minutes

## Monitoring Script (monitoring.sh)
A bash script that displays the following information:
- Operating system architecture and kernel version
- Number of physical and virtual processors
- Current available RAM and its utilization rate
- Current available memory and its utilization rate
- Current processor utilization rate
- Date and time of last reboot
- LVM status
- Number of active connections
- Number of users using the server
- Server's IPv4 address and MAC address
- Number of commands executed with sudo

## Bonus Features (if implemented)
- Partition setup as specified in the subject
- Functional WordPress website with lighttpd, MariaDB, and PHP
- Additional service of choice (excluding NGINX/Apache2)

## Note
The virtual machine itself is not included in this repository. Only the configuration files and scripts are provided.

## Evaluation
During the defense, you'll be asked to:
- Explain the choice of operating system
- Demonstrate understanding of basic commands and the project's requirements
- Show the functioning of the monitoring script
- Create a new user and assign it to a group

For detailed instructions on submission and evaluation, refer to the subject PDF.