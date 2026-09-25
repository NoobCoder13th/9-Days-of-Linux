[README.md](https://github.com/user-attachments/files/32672931/README.md)
# 9-Day Linux & IT Operations Lab

## Why I Am Doing This

I created this 9-day hands-on lab to move from Linux and IT concepts into practical system administration and IT operations.

The lab focuses on building practical experience with Linux servers, users and permissions, services, networking, storage, security, Docker, automation, and troubleshooting.

The main goal is to understand how these components work together in a real operational environment rather than learning individual commands in isolation.

---

## How the Lab Works

The lab is divided into **9 days**, with each day focusing on a different area of Linux and IT operations.

Each day contains several practical tasks followed by a larger scenario that combines the skills learned during that day.

The exercises are performed hands-on in an Ubuntu environment, with commands, verification steps, testing, and troubleshooting.

---

## Skills I Hope to Gain

By completing the lab, I aim to gain hands-on experience with:

* Linux user, group, and permission management
* Employee onboarding and offboarding workflows
* Linux services and `systemd`
* Process and resource monitoring
* System and application log investigation
* Network interfaces, routing, ports, and DNS
* SSH and remote administration
* Firewall configuration with UFW
* Nginx web server administration
* Linux storage and disk management
* Backup and restoration procedures
* Docker containers and images
* Docker volumes and persistent data
* Docker networking and environment configuration
* Docker Compose and multi-container applications
* Bash scripting and cron automation
* Basic security investigation
* End-to-end infrastructure troubleshooting

---

# 9-Day Lab Curriculum

## Day 1: Linux Administration & Identity

* [✅] **Day 1 completed**

### Task 1: Employee Onboarding

* Create users and groups
* Configure home directories and shells
* Assign employees to departments
* Verify account configuration

### Task 2: Department Access

* Create department directories
* Configure group ownership
* Apply Linux permissions
* Test access between departments
* Create shared employee storage

### Task 3: Employee Offboarding

* Lock an employee account
* Remove department access
* Handle primary group membership
* Preserve employee data
* Archive data when required

**Day 1 focus:** Users, groups, permissions, access control, and employee lifecycle management.

---

## Day 2: Services, Processes & System Administration

* [ ] **Day 2 completed**

### Task 1: Service Management

* Install Nginx
* Start and stop services
* Enable services at boot
* Inspect service status with `systemctl`

### Task 2: Process & Resource Monitoring

* Inspect running processes
* Identify PIDs
* Monitor CPU and memory usage
* Generate controlled system load
* Investigate resource usage with `top` and `htop`

### Task 3: Log Investigation

* Inspect logs using `journalctl`
* Investigate failed services
* Introduce a configuration error
* Use logs to identify the cause

### Final Task: Web Server Incident

* Investigate a failed Nginx service
* Check the service and processes
* Inspect logs
* Identify and fix the problem
* Verify the service is working again

**Day 2 focus:** Services, processes, resource usage, and system logs.

---

## Day 3: Networking & Remote Administration

* [ ] **Day 3 completed**

### Task 1: Network Investigation

* Inspect network interfaces with `ip`
* Identify IP addresses
* Inspect routing tables
* Identify listening ports with `ss`

### Task 2: DNS Troubleshooting

* Inspect DNS configuration
* Test DNS resolution with `dig`
* Use `nslookup`
* Inspect DNS configuration with `resolvectl`
* Troubleshoot a simulated DNS problem

### Task 3: SSH Administration

* Configure OpenSSH
* Connect to the server remotely
* Generate SSH keys
* Configure key-based authentication
* Verify remote access

### Final Task: Remote Server Setup

* Configure network access
* Configure SSH
* Verify remote connectivity
* Troubleshoot a simulated connection problem

**Day 3 focus:** Networking, DNS, SSH, and remote administration.

---

## Day 4: Web Servers, Storage & Backups

* [ ] **Day 4 completed**

### Task 1: Static Website with Nginx

* Deploy a static website
* Configure the Nginx document root
* Verify the website
* Inspect the listening port

### Task 2: Disk Investigation

* Check filesystem usage with `df`
* Find large directories with `du`
* Inspect disks with `lsblk`
* Identify unnecessary files
* Perform basic cleanup

### Task 3: Backup & Restoration

* Create archives with `tar`
* Back up files with `rsync`
* Simulate data loss
* Restore the data
* Verify the restoration

### Final Task: Small Company Web Server

* Operate the website
* Monitor disk usage
* Create a backup
* Simulate data loss
* Restore the required files

**Day 4 focus:** Nginx, storage, backups, and restoration.

---

## Day 5: Docker & Container Operations

* [ ] **Day 5 completed**

### Task 1: Docker Fundamentals

* Pull images
* Run containers
* Map ports
* Inspect containers
* Read container logs
* Start, stop, and remove containers

### Task 2: PostgreSQL Container

* Deploy PostgreSQL with Docker
* Configure environment variables
* Connect to the database
* Create test data

### Task 3: Persistent Storage

* Create a Docker volume
* Attach it to PostgreSQL
* Remove the container
* Recreate the container
* Verify that the database data remains

### Final Task: Container Troubleshooting

* Investigate a container that fails to start
* Inspect logs
* Check environment variables
* Check port mappings
* Inspect the container configuration

**Day 5 focus:** Docker containers, images, volumes, and basic troubleshooting.

---

## Day 6: Docker Compose & Application Infrastructure

* [ ] **Day 6 completed**

### Task 1: Multi-Container Application

* Create a Docker Compose project
* Deploy Nginx
* Deploy FastAPI
* Deploy PostgreSQL
* Connect the services

### Task 2: Configuration Management

* Configure environment variables
* Use `.env`
* Protect configuration with `.gitignore`
* Configure application and database settings

### Task 3: Container Networking

* Inspect Docker networks
* Understand service-name resolution
* Test communication between containers
* Troubleshoot a broken connection

### Final Task: Application Deployment

* Deploy the complete stack
* Configure health checks
* Verify service communication
* Test the application from Nginx through FastAPI to PostgreSQL

### Application Architecture

```text
Internet
   │
   ▼
 Nginx
   │
   ▼
FastAPI
   │
   ▼
PostgreSQL
```

**Day 6 focus:** Docker Compose, container networking, configuration, and multi-container applications.

---

## Day 7: Linux Security & Access Control

* [ ] **Day 7 completed**

### Task 1: SSH Hardening

* Disable direct root login
* Enforce key-based authentication
* Review SSH configuration
* Verify legitimate access

### Task 2: Firewall Configuration

* Configure UFW
* Allow required ports
* Block unnecessary access
* Verify firewall rules

### Task 3: Authentication Investigation

* Inspect `last`
* Inspect `lastb`
* Inspect `who`
* Review active sessions
* Investigate failed login attempts

### Final Task: Security Incident

* Investigate suspicious login activity
* Review authentication logs
* Check active sessions
* Apply appropriate SSH and firewall controls
* Verify the system remains accessible

**Day 7 focus:** SSH security, firewall rules, and basic security investigation.

---

## Day 8: Monitoring, Automation & Troubleshooting

* [ ] **Day 8 completed**

### Task 1: System Monitoring

* Establish a basic system baseline
* Monitor CPU, memory, disk, and network usage
* Generate controlled system load
* Identify abnormal resource usage

### Task 2: Backup Automation

* Write a Bash backup script
* Add timestamps to backups
* Add basic error handling
* Schedule the script with cron
* Verify automated backups

### Task 3: Troubleshooting Challenge

* Start with a deliberately broken system
* Investigate the symptoms
* Determine which subsystem is failing
* Use logs, processes, networking, storage, and services
* Apply the appropriate fix

### Final Task: IT Operations Routine

* Check system health
* Review services
* Check disk usage
* Review logs
* Run backups
* Produce a short operational status report

**Day 8 focus:** Monitoring, Bash automation, scheduled tasks, and troubleshooting.

---

# Day 9: Full IT Operations Simulation

* [ ] **Day 9 completed**

The final day combines the skills developed throughout the lab into a single simulated company environment.

### Task 1: Employee Lifecycle

Handle a company request involving:

* New employee accounts
* Department assignments
* Access requirements
* Shared resources
* Employee offboarding
* Data preservation

### Task 2: Production Application Incident

A containerized application becomes unavailable.

Investigate:

* Container status
* Application logs
* Nginx
* FastAPI
* PostgreSQL
* Docker networking
* Persistent volumes

Restore the application and verify that the database data remains intact.

### Task 3: Security & Capacity Incident

The server reports suspicious authentication activity and increasing disk usage.

Investigate:

* Authentication logs
* Active sessions
* Disk usage
* Running processes
* Network connections
* System logs

Apply the necessary remediation and verify system health.

### Final Capstone

Operate a simulated company infrastructure by working through multiple operational phases:

1. Employee onboarding
2. Access configuration
3. Server and service deployment
4. Network and remote administration
5. Application deployment
6. Security investigation
7. Incident recovery
8. Operational reporting

The goal of the capstone is to troubleshoot the environment using the knowledge gained throughout the previous days rather than following a predetermined command sequence.

---

# Expected Outcome

By completing this lab, I aim to build a practical understanding of Linux and IT operations and become more comfortable working with real system administration tasks.

The lab will give me hands-on practice with:

```text
Linux
├── Users & Groups
├── Permissions
├── Services
├── Processes
├── Logs
├── Networking
├── DNS
├── SSH
├── Firewall
├── Nginx
├── Storage
├── Backups
└── Docker
    ├── Containers
    ├── Volumes
    ├── Networking
    ├── Configuration
    └── Docker Compose
        └── Nginx → FastAPI → PostgreSQL
```

The main objective is not to memorize commands, but to understand **what the system is doing, how to investigate problems, and how to verify that a solution actually works**.
