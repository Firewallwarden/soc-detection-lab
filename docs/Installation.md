# Installation

## Objective

Deploy the infrastructure required for a home Security Operations Center (SOC) lab.

---

## Environment

| Component | Configuration |
|-----------|---------------|
| Hypervisor | Oracle VirtualBox |
| Operating System | Ubuntu Server 24.04 LTS |
| Memory | 6144 MB (6 GB) |
| Processors | 2 vCPUs |
| Storage | 80 GB Dynamic VDI |
| Network | NAT |

---

## Ubuntu Server Installation

### Configuration

- Installed Ubuntu Server 24.04 LTS
- Enabled OpenSSH Server
- Used automatic storage configuration
- Left proxy configuration blank
- Used the default Ubuntu package mirror
- No optional server snaps installed

### Result

Ubuntu Server installed successfully and booted to the login prompt.

### Evidence

- Screenshot: `screenshots/installation/01-first-login.png`

---

## Update the Operating System

### Objective

Update the operating system before installing Wazuh to ensure all packages are current and any available security updates are applied.

### Why

Updating the system before deploying security software helps ensure compatibility with dependencies and reduces exposure to known vulnerabilities.

### Commands

```bash
sudo apt update
sudo apt upgrade -y
```

### Result

- Successfully updated the package index.
- Installed all available package updates.
- No services required restarting after the upgrade.
- Returned to the shell prompt without errors.

### Evidence

Screenshot:
`screenshots/installation/03-system-updated.png`

## Download Wazuh Installer

### Objective

Download the official Wazuh installation script from the Wazuh package repository.

### Command

```bash 
curl -sO https://packages.wazuh.com/4.14./wazuh-install.https
```

### Purpose

The installation script automates the deployment of the Wazuh Manager, Indexer, and Dashboard components.

### Verification

Confirmed that the `wazuh-install.sh` file was successfully downloaded to the working directory and inspected the beginning of the script before executing to confirm its contents.