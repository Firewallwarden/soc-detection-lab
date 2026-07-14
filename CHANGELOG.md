# Changelog

All notable technical milestones for the SOC Detection Lab are documented in this file.

---

## July 2, 2026

### Infrastructure Preparation

- Installed Ubuntu Server 24.04 LTS in Oracle VirtualBox.
- Configured the virtual machine with:
  - 6 GB RAM
  - 2 vCPUs
  - 80 GB dynamically allocated storage
- Enabled OpenSSH Server during installation.
- Updated Ubuntu packages and applied available security updates.
- Downloaded and verified the official Wazuh installation script.
- Began documenting the deployment process.

---

## July 7, 2026

### SIEM Deployment

- Deployed a single-node Wazuh SIEM.
- Installed the Wazuh Manager.
- Installed the Wazuh Indexer.
- Installed the Wazuh Dashboard.
- Verified successful deployment.
- Added deployment screenshots and documentation.

## 2026-07-13

### Endpoint Monitoring

- Created a Windows 11 virtual machine in Oracle VirtualBox.
- Installed Windows 11 Pro using a local account.
- Installed VirtualBox Guest Additions.
- Installed and registered the Wazuh Windows Agent.
- Verified successful communication between the Windows endpoint and the Wazuh Manager.