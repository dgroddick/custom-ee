# Custom EE

A custom Ansible Execution Environment for running Ansible jobs.

## Requirements

- Python 3.9+
- Python Pip
- Podman
- Ansible
- Ansible Builder

## Building

```
$ ansible-builder build --tag=custom-ee:1.1
```

## Running

With Ansible Navigator and an accessible remote host under Ansible control:

```
$ ansible-navigator run playbook.yml -m stdout --eei custom-ee:1.1
```
