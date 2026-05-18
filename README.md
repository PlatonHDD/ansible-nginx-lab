# Ansible Nginx Lab

Simple DevOps pet project using Ansible from PlatonHDD

## What it does

- Installs nginx
- Creates a custom HTML page
- Starts and enables nginx
- Checks that the page is available

## Technologies

- Ansible
- Nginx
- Linux

## Run

```bash
ansible-playbook -i inventory.ini site.yml
