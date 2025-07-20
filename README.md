# Ubuntu-Overview Documentation

## Table of Contents

- [Introduction](#introduction)
- [Why Ubuntu?](#why-Ubuntu)
- [What is Ubuntu?](#what-is-Ubuntu)
- [System Requirement](#System-Requirement)
- [Pre-requisites](#Pre-requisites)
- [Installing Ubuntu](#Installing-Ubuntu)
- [Conclusion](#conclusion)
- [Author](#author)
- [References](#references)

---

## Introduction

This document provides a structured and easy-to-understand overview of Ubuntu. It explains what Ubuntu is, why it's used, its core features, and how to get started.

---

## Why Ubuntu?

**Free & Open Source** - Ubuntu is completely free to download, use, and share. Its source code is open to everyone, that is allowing users and developers to view, modify, and contribute.

**Secure** - Ubuntu is highly secure. It comes with a built-in firewall (ufw), user privilege management, and gets regular security patches from Canonical.

**Package Management** - Installing, updating, and removing software is easy using Ubuntu package management tools like ```apt``` and ```snap```.

**Community Support** -  Ubuntu has one of the largest and most active open-source communities. if you are stuck with an error or looking for a tutorial, help is available through forums like AskUbuntu, Stack Overflow, and official documentation of ubuntu.

**DevOps & Cloud Ready** - Ubuntu is widely used in cloud environments like AWS, Azure, and GCP. It is ourfirstchoice for running Devops tools like Ansible, Terraform, and Jenkins.

---

## What is Ubuntu?

Ubuntu is an open-source Linux- based operating system which is developed by canonical Ltd in 2004. Ubuntu is designed to be easy to use, highly secure, and realiable operating system.

Ubuntu is widely used in personal computer, server and cloud computing.

---
## System Requirement

| Requirement         | Minimum          | Recommendation         |
| :------------------ | :--------------- | :--------------------- |
| Processor| 2 GHz Dual Core or higher | 2+ GHz Dual Core                   |
| RAM | 2 GB  | 4 GB or more  |
| Storage         | 25 GB free hard disk space   | 30+ GB SSD for better performance |

---
## Pre-requisites

Before using or installing Ubuntu, here are a few basic requirements and things you should be familiar with:

**Basic Computer Knowledge** – Understanding how to use a keyboard, mouse, and basic file navigation.

**Compatible Hardware** – At least 2 GB RAM, 25 GB storage, and a 64-bit processor.

**Bootable USB or DVD** – To install Ubuntu, you'll need a USB drive (4 GB or more) or DVD with the Ubuntu ISO image.

**Internet Connection** –  Needed for downloading updates, drivers, and software packages on a Ubuntu/Linux system.

---

## Installing Ubuntu

1. **Download ISO**

   - Go to https://ubuntu.com/download.
   - Choose Ubuntu Desktop or Server (LTS) version.

3. **Create Bootable USB**

   - On Linux: Use dd command.
     ```
     sudo dd if=ubuntu.iso of=/dev/sdX bs=4M status=progress
     ```
     
4. **Boot from USB**
      - Plug USB in and restart PC.
      - Press boot key (F2/F12/ESC/DEL depending on your computer brand).
      - Select USB to boot.
        
5. **Install Ubuntu**
      - Select language and keyboard layout.
      - Choose: “Erase disk and install Ubuntu”.
      - and than Create user, password and time zone.
      - Start installation.
      - After completing the installation step then reboot the system.
      - Done
 
---


## Conclusion

Ubuntu is a free and user-friendly operating system based on Linux. It offers a simple interface, regular updates, and a large collection of software, making it great for both beginners and advanced users. With different versions for desktops, servers, and even IoT devices, Ubuntu supports a strong open-source community and continues to grow with new features and support.

---

## Author

- **Name:** Sunny Kumar
- **Email:** sunny.kumar.snaatak@mygurukulam.co

---

## References

- [Ubuntu Official Documentation](https://documentation.ubuntu.com/core/)
- [Installing Ubuntu](https://ubuntu.com/download/desktop)

