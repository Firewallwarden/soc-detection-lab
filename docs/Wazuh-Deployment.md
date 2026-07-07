# Wazuh Deployment

## Objective

Deploy and verify a functioning single-node Wazuh Security Information and Event Management (SIEM) platform.

---

## Components Installed

- Wazuh Manager
- Wazuh Indexer
- Wazuh Dashboard

---

## Service Verification

After deployment, each core Wazuh service was verified using `systemctl`.

### Commands

```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-indexer
sudo systemctl status wazuh-dashboard
```

### Verification

All three services reported:

```
Active: active (running)
```

This confirms that the SIEM platform was successfully installed and all core components are operational.

## Post-Deployment Security

### Administrative Credentials

After verifying successful deployment, the default administrative password was replaced with a new strong password using the Wazuh password management tool.

### Why

Changing the default credentials immediately after deployment reduces the risk of unauthorized access and follows security best practices.

### Skills Demonstrated

- Identity and access management
- Security hardening
- Linux administration