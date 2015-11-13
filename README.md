mongodb
=======

[![Ansible Role](https://img.shields.io/ansible/role/3287.svg)](https://galaxy.ansible.com/list#/roles/3287)

Installs and configures MongoDB

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name            | Default   | Description                     |
|-----------------|-----------|---------------------------------|
| mongodb_version | 3.0.7     | MongoDB version to install      |
| mongodb_port    | 27017     | TCP port MongoDB will listen on |
| mongodb_bind_ip | 127.0.0.1 | IP address MongoDB will bind to |

Dependencies
------------

None

Example Playbook
----------------

Install MongoDB
```
- hosts: all
  roles:
    - { role: kbrebanov.mongodb }
```

Install MongoDB specifying port
```
- hosts: all
  roles:
    - { role: kbrebanov.mongodb, mongodb_port: 38875 }
```

Install MongoDB specifying port and IP address
```
- hosts: all
  roles:
    - { role: kbrebanov.mongodb, mongodb_port: 38875, mongodb_bind_ip: 192.168.1.10 }
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
