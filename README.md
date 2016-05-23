Mongo [![Build Status](https://travis-ci.org/SimpliField/ansible-mongo.svg?branch=master)](https://travis-ci.org/SimpliField/ansible-mongo) [![Ansible Role](https://img.shields.io/ansible/role/9884.svg?maxAge=2592000)](https://galaxy.ansible.com/SimpliField/mongo/)
=========

Setup mongodb server

Requirements
------------

Need ansible 2+

Role Variables
--------------

```yaml
mongodb_storage_path: "/data/db"
mongodb_user: "mongodb"
mongodb_group: "mongodb"
```

Dependencies
------------

There is no dependency

Example Playbook
----------------

```
- hosts: servers
  roles:
  - { role: simplifield.mongo }

License
-------

BSD
