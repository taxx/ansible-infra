## Basics
These scripts are intended to be run on the target itself.

Make sure ansible is installed on the target:
```bash
apt update
apt install ansible -y
```

Run the playbook of choice, example:
```bash
ansible-playbook -i "localhost," -c local playbooks/osiris.yml
#ansible-playbook -i inventories/osiris/hosts.yml playbooks/osiris.yml
```

