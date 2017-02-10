# Ansible jenkins role 

Installs jenkins on a machine running within a docker container with slaves

## Usage

- This playbook can be used on centos-machines
- If you want to modify the playbook, you can test it by adding your vm's host to the staging inventory under jenkins-master
- When adding hosts to the inventory don forget to enable ssh-authentication via key : 
```bash
ssh-keygen -t rsa
ssh-copy-id user@123.45.56.78
```

```bash
ansible-playbook -i staging main.yml --become --ask-become-pass
```
