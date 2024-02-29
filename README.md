# Provision a host with Lingo package manager for Lingua Franca

Provision a system with Lingo package manager, the package manager for Lingua Franca applications.

Features

- lingo package manager (user install)

Platforms supported

- linux/amd64
- linux/arm64
- linux/arm/v7 (armhf)
- linux/riscv64

## Prerequisites

Provisionig system:

- Ansible 2.15

Remote system:

- Debian-based host accessible via SSH with apt-get and sudo available
- lfc
- rust

## Example playbook

```yaml
---
- name: Install Lingo
  hosts: myhosts
  gather_facts: true
  roles:
    - name: xronos_lingo_ansible
      role: xronos_lingo_ansible
```
