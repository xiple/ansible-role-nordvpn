Ansible role: NordVPN
=========

[![CI](https://github.com/xiple/ansible-role-nordvpn/actions/workflows/ci.yml/badge.svg)](https://github.com/xiple/ansible-role-nordvpn/actions/workflows/ci.yml)

An ansible role that installs NordVPN CLI on Linux.

Requirements
----------------

None.

Role Variables
----------------

```yaml
nordvpn_users:
  - user1
  - user2
```

A list of system users to be added to the nordvpn group (so they can use nordvpn on the server).

Supported distributions
----------------

This role has been been developed and tested on the following distributions :

- Fedora 43
- Fedora 42

Example Playbook
----------------

```yaml
- hosts: all
  vars:
    nordvpn_users:
      - usr1
      - usr2
  roles:
    - xiple.nordvpn
```

License
-------

MIT
