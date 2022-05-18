# Automated configuration for running a Unifi controller on a raspberry-pi

## Setup

1. Install Ubuntu on SD Card and boot the device
2. Change password for the default `ubuntu` account
3. Create DHCP reservation

Create and update `secrets.yml` with your values

```bash
cp ansible/secrets.yml.example ansible/secrets.yml
```

Install Ansible module

`ansible-galaxy collection install -i community.general`

Run the playbook

```bash
ansible-playbook -i ansible/hosts ansible/pi-setup.yml
```

### Ansible Tags
* apt
* update
* user
* system
* docker


