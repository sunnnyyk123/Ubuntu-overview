# Ubuntu Overview Documentation

## Author Information

| Created by    | Created on | Version | Last updated | Pre-Reviewer |
|--------------|------------|---------|--------------|--------------|
| Sunny Kumar  | 16-07-2025 | V 1.0   | 22-07-2025   | Aman Raj     |

---
## Table of Contents

- [1. Introduction](#1-introduction)
- [2. What is Ubuntu?](#2-what-is-ubuntu)
- [3. Why Ubuntu?](#3-why-ubuntu)
- [4. Ubuntu Architecture](#4-ubuntu-architecture)
- [5. Software Management in Ubuntu](#5-software-management-in-ubuntu)
    - [5.1. APT](#51-apt)
    - [5.2. Snap Package Manager](#52-snap-package-manager)
- [6. Services in Ubuntu](#6-services-in-ubuntu)
    - [6.1. Understanding systemd](#61-understanding-systemd)
    - [6.2. Common Service Commands](#62-common-service-commands)
    - [6.3. Essential Ubuntu Services](#63-essential-ubuntu-services)
- [7. Advantages of Ubuntu](#7-advantages-of-ubuntu)
- [8. Disadvantages of Ubuntu](#8-disadvantages-of-ubuntu)
- [9. Conclusion](#9-conclusion)
- [10. FAQ](#10-faq)
- [11. Contact Information](#11-contact-information)
- [12. References](#12-references)

---

## 1. Introduction

This document provides a structured and easy-to-understand overview of Ubuntu. It explains what Ubuntu is, why it's used, its core features, and how to get started.

---
## 2. What is Ubuntu?

Ubuntu is an open-source, Linux-based operating system developed by Canonical Ltd. in 2004. Ubuntu is designed to be easy to use, highly secure, and reliable.

Ubuntu is widely used on personal computers, servers, and in cloud computing.

---
## 3. Why Ubuntu?

- **Free & Open Source:** Ubuntu is completely free to download, use, and share. Its source code is open to everyone, allowing users and developers to view, modify, and contribute.

- **Secure:** Ubuntu is highly secure. It comes with a built-in firewall (ufw), user-privilege management, and receives regular security patches from Canonical.

- **Package Management:** Installing, updating, and removing software is easy using Ubuntu's package management tools like `apt` and `snap`.

- **Community Support:** Ubuntu has one of the largest and most active open-source communities. If you are stuck with an error or looking for a tutorial, help is available through forums like Ask Ubuntu, Stack Overflow, and the official documentation of Ubuntu.

- **DevOps & Cloud Ready:** Ubuntu is widely used in cloud environments like AWS, Azure, and GCP. It is a top choice for running DevOps tools like Ansible, Terraform, and Jenkins.

---

## 4. Ubuntu Architecture

| Layer      | Description                                                      |
|------------|------------------------------------------------------------------|
| Hardware   | Physical components like CPU, RAM, Hard Disk, etc.               |
| Kernel     | Core part of the operating system; acts as a bridge between hardware and software. |
| Shell      | Interface between the user and the kernel.                       |
| Applications | User-level programs like browsers, text editors, media players, etc. |
| Users      | People who interact with the system using applications.          |

<img width="515" height="398" alt="image" src="https://github.com/user-attachments/assets/237e31b3-02f6-4835-a671-d827ca5b46e0" />

---

## 5. Software Management in Ubuntu

Ubuntu uses various tools to manage software packages efficiently.

### 5.1. APT
APT (Advanced Package Tool) is a command-line tool for installing, updating, and removing `.deb` packages.

```bash
sudo apt update
sudo apt install <package-name>
sudo apt remove <package-name>
```

### 5.2. Snap Package Manager
`snap` is a command-line tool for installing, updating, and removing Snap packages (self-contained apps).

```bash
sudo snap install <package-name>
sudo snap refresh <package-name>
sudo snap remove <package-name>
```
For more details about software management in Ubuntu, click here: [Documentation](https://github.com/Snaatak-Apt-Get-Swag/documentation/blob/scrum-8-nitin/Documentation/Operating-System/Ubuntu/SOP/Software-Management/readme.md)

---

## 6. Services in Ubuntu

Services or daemons in Ubuntu are managed using `systemd`, the default `init` system.

### 6.1. Understanding systemd

`systemd` is the default init system used in Ubuntu. It is responsible for managing the system's boot-up process, controlling the lifecycle of services (such as starting, stopping, enabling, and disabling them), and handling logging and service dependencies. `systemd` ensures that services start in the correct order and provides powerful tools for monitoring and managing system processes efficiently.

### 6.2. Common Service Commands

Use `systemctl` to manage services:

```bash
# Start a service
sudo systemctl start <service-name>

# Stop a service
sudo systemctl stop <service-name>

# Restart a service
sudo systemctl restart <service-name>

# Enable a service (auto-start at boot)
sudo systemctl enable <service-name>

# Disable a service
sudo systemctl disable <service-name>

# Check service status
systemctl status <service-name>

# List all active services
systemctl list-units --type=service
```

### 6.3. Essential Ubuntu Services

| Service Name | Description                             |
|--------------|-----------------------------------------|
| `networking` | Manages network interfaces              |
| `ssh`        | Enables remote SSH access               |
| `cron`       | Schedules tasks (cron jobs)             |
| `snapd`      | Snap package manager background service |

For more details about Ubuntu services, click here: [Documentation](https://github.com/Snaatak-Apt-Get-Swag/documentation/tree/scrum-7-hifza/Operating-System/Ubuntu/SOP/Services)

---
## 7. Advantages of Ubuntu
- **Free and Open Source:** No licensing cost; source code is open for anyone to use or modify.
- **User-Friendly Interface:** Clean and simple UI (especially with GNOME), good for beginners.
- **Regular Updates & Long-Term Support (LTS):** LTS versions are supported for 5 years, offering stability and security.
- **Large Community Support:** Easy to find help through forums, documentation, and tutorials.
- **Secure by Default:** Fewer viruses and malware compared to Windows.
- **Great for Development:** Built-in support for most programming languages and tools (Python, Java, Git, etc.).
- **Good Package Management:** APT and Snap make installing software easy.
- **Lightweight & Fast:** Can run smoothly on older hardware with lighter desktop environments.

---

## 8. Disadvantages of Ubuntu
- **Software Compatibility:** Many commercial apps or games (e.g., Adobe Photoshop, MS Office) are not natively available.
- **Learning Curve for Beginners:** Terminal use can be confusing for new users.
- **Enterprise Support Costs:** Official Ubuntu Advantage support (for enterprises) comes with a cost.
- **Snap Performance Issues:** Snap apps can be slower to start and use more disk space.

---

## 9. Conclusion

Ubuntu is a free and user-friendly operating system based on Linux. It offers a simple interface, regular updates, and a large collection of software, making it great for both beginners and advanced users. With different versions for desktops, servers, and even IoT devices, Ubuntu supports a strong open-source community and continues to grow with new features and support.

---
## 10. FAQ

| **Question**                                                 | **Answer**                                                                                                                                    |
|--------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| **Q1. What is Ubuntu?**                                      | Ubuntu is a free and open-source Linux-based operating system developed by Canonical Ltd., known for its ease of use, security, and reliability. |
| **Q2. Is Ubuntu free to use?**                               | Yes, Ubuntu is completely free to download, install, and use. It is also open-source, so its source code is freely available.                  |
| **Q3. What are the key package management tools in Ubuntu?** | Ubuntu uses `apt` for `.deb` packages and `snap` for containerized software packages.                                                         |
| **Q4. How do I update software in Ubuntu?**                  | You can update using `sudo apt update && sudo apt upgrade` for APT or `sudo snap refresh` for Snap packages.                                  |
| **Q5. What is systemd in Ubuntu?**                           | `systemd` is Ubuntu’s default init system responsible for managing services and system boot processes.                                         |
| **Q6. Can I use Ubuntu for development?**                    | Yes, Ubuntu is highly preferred for development with built-in support for tools like Python, Java, Git, etc.                                  |
| **Q7. Is Ubuntu good for beginners?**                        | Yes, Ubuntu has a clean interface (GNOME), a large support community, and is beginner-friendly.                                               |
| **Q8. What are Snap packages?**                              | Snap packages are self-contained applications that include all dependencies, managed via the `snap` command.                                  |
| **Q9. How is Ubuntu used in the cloud?**                     | Ubuntu is widely used in cloud platforms like AWS, GCP, and Azure. It's often the base OS for running DevOps tools.                           |
| **Q10. What are some limitations of Ubuntu?**                | Ubuntu lacks native support for some commercial software, may require terminal usage, and Snap apps can be slow.                              |

---

## 11. Contact Information

| **Field** | **Details**                                                                     |
|-----------|---------------------------------------------------------------------------------|
| Name      | Sunny Kumar                                                                     |
| Email     | [sunny.kumar.snaatak@mygurukulam.co](mailto:sunny.kumar.snaatak@mygurukulam.co) |

---

## 12. References

| **Title**                     | **Link**                                                                                                                   |
|-------------------------------|--------------------------------------------------------------------------------------------------------------------------|
| Ubuntu Official Documentation | [documentation.ubuntu.com/core](https://documentation.ubuntu.com/core/)                                                    |
| Installing Ubuntu             | [ubuntu.com/download/desktop](https://ubuntu.com/download/desktop)                                                         |
| Linux Architecture            | [geeksforgeeks.org - Linux Architecture](https://www.geeksforgeeks.org/linux-unix/architecture-of-linux-operating-system/) |



