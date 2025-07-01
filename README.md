## Basics
These scripts are intended to be run on the target itself.

Make sure ansible is installed on the target:
```bash
apt update
apt install ansible -y
```

Create the `.env.yml` file in the playbooks folder _(rename the `.env.example.yml` and adjust it to your specifications)_

Run the playbook of choice, example:
```bash
ansible-playbook -i inventory/hosts.yml -c local playbooks/debian-server.yml
#ansible-playbook -i "localhost," -c local playbooks/debian-server.yml
#ansible-playbook -i inventories/osiris/hosts.yml playbooks/debian-server.yml
```

