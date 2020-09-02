# ansible-playbooks

Ansible playbooks for bug bounty

# Usage

## Install requirements
```
ansible-galaxy install -r requirements.yml
```

## Deploy on Linux  (Kali)

Install all playbooks with
```
$ ./install.sh
```

Install a specific playbook
```
ansible-playbook -i hosts.ini -l server playbooks/utilities.yml
```

Install a specific tool inside a playbook 
```
ansible-playbook -i hosts.ini -l server playbooks/utilities.yml --tags tooltag
```
