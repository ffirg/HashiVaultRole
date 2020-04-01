# Hashicorp Vault Setup/Config Ansible Role

Heavily based on the excellent work done by https://github.com/MiteshSharma/AnsibleVaultRole (many thanks!)

This Ansible Role for Hashicorp Vault will download/install/configure an initial Vault. 

It is designed to be used during Ansible Workshops so we can demonstrate the integration with Ansible Tower.

The first role will setup the accounts, download/install the application and setup/start the systemd service.

The second role will then do the initial Vault configuration.

The Vault will be installed/setup on your Ansible control node.

### Setup

```bash

cd && git clone https://github.com/ffirg/HashiVaultRole && cd HashiVaultRole
ansible-playbook hashivault.yml

```

#### Accessing Vault

By default we use http port 8000 on your Ansible control node, and listen on all interfaces.
We've installed the Vault UI which will be available on something like: http://student3.08b5.rhdemo.io:8000/ui/

