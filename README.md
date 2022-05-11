# Automated configuration for running a Unifi controller on a raspberry-pi

## Setup

1. Install Ubuntu on SD Card and boot the device
2. Change password for the default `ubuntu` account
3. Create DHCP reservation

```bash
cp ansible/secrets.yml.example ansible/secrets.yml
ansible-playbook -i ansible/hosts ansible/pi-setup.yml
```

### Ansible Tags
* apt
* update
* user
* system
* docker
