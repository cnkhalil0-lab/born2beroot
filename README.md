*This project has been created as part of the 42 curriculum by kel-boud.*
# Born2BeRoot

## Description

Born2BeRoot is a system administration project focused on discovering how a Linux system works from the inside. 
The goal is to install and configure a secure virtual machine while applying basic server and security best practice.

This project introduces virtualization, user and permission management, disk partitioning, services, and system hardening.

---

## Instructions

### Setup
- Create a virtual machine using VirtualBox or UTM
- Install Debian or Rocky Linux (no graphical interface)
- Follow the subject rules for users, passwords, partitions, and security

### Usage
- Start the VM from your virtualization software
- Log in with the configured user
- The system is evaluated by checking configuration and security rules

---

## Operating System & Design Choices

This project was done using **Debian**.

**Why Debian?** 
Debian is stable, lightweight, well documented, and widely used for servers. It is beginner-friendly and enables AppArmor by default, which fits well with the project goals.

### Main Choices
- **Partitioning:** LVM used for flexibility and clean disk organization
- **Security:** Strong password policy, sudo restrictions, AppArmor enabled
- **Users:** Non-root user with sudo privileges, root access limited
- **Services:** SSH and firewall only, no unnecessary services

---

## Comparisons

**Debian vs Rocky Linux** 
Debian is community-driven and easier to learn, while Rocky Linux is more enterprise-oriented and uses SELinux by default.

**AppArmor vs SELinux** 
AppArmor is simpler and profile-based; SELinux is more powerful but complex.

**UFW vs firewalld** 
UFW is straightforward and easy to manage; firewalld is more advanced and zone-based.

**VirtualBox vs UTM** 
VirtualBox is cross-platform and common at 42; UTM is mainly used on macOS, especially Apple Silicon.

---

## Resources

- Debian & Rocky Linux official documentation 
- Linux man pages 
- 42 Born2BeRoot subject 

### AI Usage
AI was used to better understand Linux concepts, security mechanisms, and to help structure this README. 
All system configuration and commands were done manually.


