# Install Active Directory Domain Controller
This playbook installs AD DC using samba4. Tested on Ubuntu 20.04

Modify following items to run this playbook:
- inventory
- config.yaml

## Run
```bash
ansible-playbook -u <username> -K -k playbook.yaml
```

## Add a Windows Client
- Open a Windows client and make sure DNS is set accordingly. (If you have no DNS server use DC as DNS)
- Find [required menu](https://user-images.githubusercontent.com/3802058/142480628-af3233a0-7688-4bbd-acc0-9afa3beed7ed.png) to connect to domain
- Domain name is `workgroup` inside `config.yaml`.
- Enter Administrator as username and `admin_password` as password. (This is also set inside `config.yaml`)
- Skip account add step.
- Login with users defined in `config.yaml`
