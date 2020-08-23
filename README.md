# ansible_vault
This Running Only For Centos Operating System

Credential Management
Secure, store and tightly control access to tokens, passwords, certificates, encryption keys for protecting secrets and other sensitive data using a UI, CLI, or HTTP API.

## INSTALLATION
You must edit two variables on contained in the role directory (common and vault)

COMMON ROLE VARIABLE
```
---
# Host Profilling
hostname: "<fill_your_hostname>"
ip_address: "<fill_your_hostip>"

# Directories Profilling
dest_myhosts_file: /etc
ntp_configuration_path: /etc
```

VAULT ROLE VARIABLE
```
---
#Path Information
dest_myhosts_file: /etc

# VAULT INFORMATION
vault_version: "<fill_vault_version>"
vault_group: "vault"
vault_user: "vault"
vault_mode: "0775"
root_mode: "root"
root_group: "root"

# VAULT DIRECTORIES PROFILE
vault_binary_directory_path: "/usr/local/bin"
vault_directory_path: "/etc/vault.d"
vault_log_directory: "/var/log/vault-log"
vault_log_file_path: "/var/log/vault-log/vault-audit.log"
vault_configuration_file: "/etc/vault.d/config.json"
vault_autounseal_file: "/etc/vault.d/config-autoanseal.hcl"
vault_systemd_file: "/etc/systemd/system/vault.service"

# VARIABLE FOR VAULT CLUSTERING
vault_server_1: <FILL_VAULT_SERVER1>
vault_server_2: <FILL_VAULT_SERVER2>
vault_server_3: <FILL_VAULT_SERVER3>

bind_addr: <FILL_VAULTIP>
api_addr: <FILL_VAULTIP>
cluster_addr: <FILL_VAULTIP>
```
