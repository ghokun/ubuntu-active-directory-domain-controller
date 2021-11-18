# Install Active Directory Domain Controller
This playbook installs AD DC using samba4. Tested on Ubuntu 20.04

Modify following items to run this playbook:
- inventory
- config.yaml

Run:
```bash
ansible-playbook -u <username> -K -k playbook.yaml
```
