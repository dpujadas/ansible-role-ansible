ansible
=======

This role installs ansible itself using pip package

Role Variables
--------------

- `ansible_role_version`: Ansible version to install. If not set, latest will be installed (Ex: '2.1.0')
- `ansible_role_extra_pip_packages`: List of additional pip packages to install (default: Empty list)

Example Playbook
----------------

    - hosts: servers
      vars:
        ansible_role_extra_pip_packages:
          - name: 'boto'
            version: '2.42.0'
          - name: 'docker-py'
      roles:
        - { 
          role: 'ansible',
          ansible_role_version: '2.1.0'
        }

License
-------

MIT

[![Build Status](https://travis-ci.org/dpujadas/ansible-role-ansible.svg?branch=master)](https://travis-ci.org/dpujadas/ansible-role-ansible)