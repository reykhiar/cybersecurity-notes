# Computer Fundamentals for Cybersecurity

## Overview

Before learning advanced cybersecurity topics, it is important to understand how computers work. Security professionals regularly interact with hardware, operating systems, servers, virtual machines, and cloud environments. A solid understanding of these fundamentals helps build a stronger foundation for future topics such as Linux, networking, malware analysis, penetration testing, and digital forensics.

---

## Computer Components

A computer system consists of several core components that work together.

### Central Processing Unit (CPU)

The CPU is the brain of the computer. It executes instructions, performs calculations, and processes data.

### Random Access Memory (RAM)

RAM is temporary memory used to store data that is actively being processed. Data stored in RAM is lost when the computer is powered off.

### Storage

Storage devices keep data permanently.

Common examples:

* Solid State Drive (SSD)
* Hard Disk Drive (HDD)

Storage contains operating systems, applications, and user files.

### Motherboard

The motherboard connects all hardware components and allows communication between them.

### Power Supply Unit (PSU)

The PSU provides electrical power to all components inside the computer.

---

## The Boot Process

When a computer starts, it follows a sequence known as the boot process.

### 1. Power On

The user presses the power button, allowing the PSU to provide power to the system.

### 2. Firmware Initialization

The firmware (UEFI or BIOS) starts running and initializes hardware components.

### 3. Power-On Self-Test (POST)

The system checks whether required hardware components are present and functioning correctly.

### 4. Boot Device Selection

The firmware searches for a bootable device such as an SSD, HDD, or USB drive.

### 5. Bootloader Execution

The bootloader loads the operating system into memory and transfers control to it.

---

## Types of Computers

Different computers are designed for different purposes.

### Laptop

Portable computer designed for everyday use.

Characteristics:

* Battery powered
* Lightweight
* Mobile

### Desktop

Computer designed for fixed locations.

Characteristics:

* Better cooling
* Easier hardware upgrades
* Higher sustained performance

### Workstation

High-performance computer designed for professional workloads.

Common uses:

* Engineering
* 3D modeling
* Scientific simulations
* Video production

### Server

A computer that provides services to other systems over a network.

Examples:

* Web servers
* Database servers
* Mail servers

### Smartphone

Pocket-sized computer optimized for mobility, connectivity, and battery efficiency.

### IoT Devices

Internet-connected devices designed for specific tasks.

Examples:

* Smart thermostats
* Smart doorbells
* Fitness trackers

### Embedded Systems

Computers built into other devices.

Examples:

* Coffee machines
* Automatic doors
* Industrial equipment

---

## Client-Server Model

Most internet services use the client-server model.

### Client

A client initiates requests.

Examples:

* Web browsers
* Mobile applications
* Email clients

### Server

A server receives requests and provides responses.

Examples:

* Web servers
* Database servers
* File servers

### Request and Response

Communication follows a request-response pattern.

Example:

1. Client sends a request.
2. Server processes the request.
3. Server returns a response.

---

## Networking Concepts

### Protocol

A protocol defines rules for communication between systems.

Examples:

* HTTP
* HTTPS
* DNS
* FTP

### Port

A port identifies a specific service running on a system.

Examples:

* 80 (HTTP)
* 443 (HTTPS)
* 22 (SSH)

### DNS

Domain Name System (DNS) translates domain names into IP addresses.

Example:

```text
google.com → 142.250.x.x
```

### IP Address

An IP address uniquely identifies a device on a network.

Examples:

```text
192.168.1.10
8.8.8.8
```

---

## Virtualization

Virtualization allows multiple virtual systems to share the same physical hardware.

### Hypervisor

A hypervisor manages virtual machines.

Types:

#### Type 1 Hypervisor

Runs directly on hardware.

Examples:

* VMware ESXi
* Microsoft Hyper-V

#### Type 2 Hypervisor

Runs inside an existing operating system.

Examples:

* VirtualBox
* VMware Workstation

### Virtual Machine (VM)

A VM is a complete virtual computer with its own operating system and resources.

Benefits:

* Isolation
* Testing environments
* Safe malware analysis
* Cybersecurity labs

---

## Containers

Containers provide lightweight application isolation.

Unlike virtual machines, containers share the host operating system kernel.

Common platform:

* Docker

Benefits:

* Fast deployment
* Low resource usage
* Scalability
* Portability

---

## Cloud Computing Fundamentals

Cloud computing provides computing resources over the internet.

### Benefits

* Scalability
* High availability
* Global access
* Cost efficiency
* On-demand resources

### Cloud Deployment Models

#### Public Cloud

Shared infrastructure managed by cloud providers.

Examples:

* AWS
* Microsoft Azure
* Google Cloud Platform

#### Private Cloud

Dedicated cloud environment for a single organization.

#### Hybrid Cloud

Combination of public and private cloud environments.

---

## Cloud Service Models

### Infrastructure as a Service (IaaS)

Provides virtual servers, storage, and networking.

Examples:

* Amazon EC2
* Azure Virtual Machines

### Platform as a Service (PaaS)

Provides an environment for developing and deploying applications.

Examples:

* Heroku
* Google App Engine

### Software as a Service (SaaS)

Provides complete software applications over the internet.

Examples:

* Gmail
* Zoom
* Microsoft 365

---

## Why Computer Fundamentals Matter in Cybersecurity

Cybersecurity professionals must understand:

* How computers operate
* How systems boot
* How servers provide services
* How virtualization works
* How cloud infrastructure is deployed

These concepts form the foundation for later topics such as Linux, Windows security, malware analysis, penetration testing, incident response, and cloud security.

---

## Key Takeaway

Computer fundamentals provide the foundation for cybersecurity. Understanding hardware, operating systems, networking, virtualization, and cloud computing helps security professionals understand what they are protecting and how modern systems operate.
