# Ansible Nginx Lab

Simple DevOps pet project using Ansible and Nginx.

## Project Goal

Automate nginx deployment and configuration using Ansible roles.

---

# Features

- Install nginx
- Configure custom HTML page
- Use Ansible roles
- Use group variables
- Use handlers
- Use tags
- Validate service availability with uri module

---

# Project Structure

```text
ansible-nginx-lab/
├── group_vars/
│   └── web.yml
├── inventory.ini
├── site.yml
├── README.md
└── roles/
    └── nginx/
        ├── defaults/
        │   └── main.yml
        ├── handlers/
        │   └── main.yml
        ├── tasks/
        │   └── main.yml
        └── templates/
            └── index.html.j2
```

---

# Technologies

- Ansible
- Nginx
- Linux
- Git
- GitHub

---

# Run Playbook

```bash
ansible-playbook -i inventory.ini site.yml
```

---

# Run By Tags

## Install nginx

```bash
ansible-playbook -i inventory.ini site.yml --tags install
```

## Update configuration

```bash
ansible-playbook -i inventory.ini site.yml --tags config
```

## Restart service tasks

```bash
ansible-playbook -i inventory.ini site.yml --tags service
```

## Run checks

```bash
ansible-playbook -i inventory.ini site.yml --tags check
```

---

# Verify

```bash
curl http://localhost
```

---

# What I Learned

- Ansible playbooks
- Roles structure
- Variables and group_vars
- Jinja2 templates
- Handlers
- Tags
- Service management
- Nginx basics
- Git workflow
