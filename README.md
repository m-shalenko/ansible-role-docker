# ansible-role-docker

## Purpose
This ansible role installs Docker Engine.

## Install
```bash
ansible-galaxy role install m-shalenko.docker
```

## Example of playbook
```yaml
---
- name: Install Docker Engine
  hosts: localhost
  connection: local
  become: true
  gather_facts: false
  roles:
    - role: m-shalenko.docker
      tags:
        - docker
```
