<p align="center"> <img src="https://img.shields.io/badge/OS-Debian/CentOS-blue?style=for-the-badge&logo=linux" alt="OS"> <img src="https://img.shields.io/badge/VirtualBox-UTM-orange?style=for-the-badge&logo=virtualbox" alt="VirtualBox"> <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status"> </p> <h1 align="center">🚀 Born2beroot 🚀</h1> <p align="center"> <i>A system administration project from 42 School where you configure a secure virtual machine using Debian or CentOS.</i> </p>



## Table of Contents
1. [Introduction](#introduction)
    - [What is a Virtual Machine?](#what-is-a-virtual-machine)
    - [How do Virtual Machines work?](#how-do-virtual-machines-work)
    - [What is LVM?](#what-is-lvm)
    - [What is AppArmor?](#what-is-apparmor)
    - [Difference between Apt and Aptitude](#difference-between-apt-and-aptitude)
    - [How to use SSH?](#how-to-use-ssh)
    - [How to implement UFW with SSH?](#how-to-implement-ufw-with-ssh)
    - [What is cron and what is wall?](#what-is-cron-and-wall)
2. [Installation](#installation)
3. [sudo Configuration](#sudo-configuration)
    - [Step 1: Installing sudo](#installing-sudo)
    - [Step 2: Adding User to sudo Group](#adding-user-to-sudo-group)
    - [Step 3: Running root-Privileged Commands](#running-root-privileged-commands)
    - [Step 4: Configuring sudo](#configuring-sudo)
4. [SSH Configuration](#ssh-configuration)
    - [Step 1: Installing & Configuring SSH](#installing-configuring-ssh)
    - [Step 2: Installing & Configuring UFW](#installing-configuring-ufw)
    - [Step 3: Connecting via SSH](#connecting-via-ssh)
5. [User Management](#user-management)
    - [Step 1: Password Policy](#password-policy)
    - [Step 2: Creating a New User](#creating-new-user)
    - [Step 3: Creating a New Group](#creating-new-group)
6. [cron Configuration](#cron-configuration)
7. [Monitoring Script](#monitoring-script)
8. [Bonus](#bonus)
    - [WordPress Installation](#wordpress-installation)
    - [FTP Configuration](#ftp-configuration)
9. [Submission](#submission)
10. [Evaluation Knowledge](#evaluation-knowledge)


---

1️⃣ Introduction

Born2beroot is a system administration project from 42 School. The goal of this project is to create a secure virtual machine using Debian or Rocky within a virtual environment like VirtualBox or UTM.

🔍 What You'll Do:

✅ Set up user privileges and security measures

✅ Configure SSH access and firewall rules

✅ Set up password policies and sudo configuration

✅ Monitor system resources and automate services


This README will guide you through the setup process step-by-step to help you build a functional and secure server environment.

---

What is a Virtual Machine? <a name="what-is-a-virtual-machine"></a>

A Virtual Machine (VM) is a software-based computer that runs an operating system (OS) inside another OS, using shared hardware resources (CPU, RAM, storage).

Key Properties:

➡️ Hypervisor: Software (e.g., VirtualBox, UTM) that creates/manages VMs.

➡️ Isolation: VM crashes won’t affect the host machine.

➡️ Snapshots: Save/restore VM state at any point.


Types of VMs:

➡️ Type 1 (Bare-metal): Runs directly on hardware (e.g., VMware ESXi).

➡️ Type 2 (Hosted): Runs on top of an OS (e.g., VirtualBox).


Why Use VMs?

✔ Test software safely

✔ Run multiple OSes (Linux/Windows/macOS) on one machine

✔ Clone/backup entire systems

---
