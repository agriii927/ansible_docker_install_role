# Ansible role for Docker installation

## About
This role is useful for installation ansible on machines of different Linux distributions

## Prerequisites
- Host-only network in Oracle VM VirtualBox or AWS/GCP etc. cluster

## How to configure it
- Set user and password params in group_vars/servers 
- Set remote machines addresses in hosts.txt
Also you may add your machines' SSH keys instead of passwords

## How to run it
If you add SSH keys:
```bash
ansible-playbook playbook_ready_role.yaml
```
If you don't add SSH keys:
```bash
ansible-playbook playbook_ready_role.yaml -kK
```
kK is for asking you to write down your password to connect / become a sudo

To use another inventory file:
```bash
ansible-playbook playbook_ready_role.yaml -i <new_inventory>
```
