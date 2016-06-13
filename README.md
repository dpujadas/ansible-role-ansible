ansible
=======

This role installs ansible itself using pip package

Role Variables
--------------

- `ansible_role_version`: Ansible version to install (default: 'latest')
- `ansible_role_docker_connect`: If true, install docker-py library to allow docker connection (default: True)

Example Playbook
----------------

    - hosts: servers
      roles:
        - { 
          role: 'ansible',
          ansible_role_version: '1.9.6'
        }

License
-------

MIT

[![Build Status](https://travis-ci.org/dpujadas/ansible-role-ansible.svg?branch=master)](https://travis-ci.org/dpujadas/ansible-role-ansible)