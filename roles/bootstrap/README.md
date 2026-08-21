# Bootstrap
Ansible bootstrapping role.

## Assumptions
- User "ansible" is defined in target hosts
- SSH server running

## Usage
1. Place ansible public key file in files/id_ansible.pub
2. Edit the inventory file accordingly
3. Run with:
```bash
ansible-playbook bootstrap.yml --become-method=su --ask-pass --ask-become-pass
```