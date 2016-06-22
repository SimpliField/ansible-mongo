Mongo [![Build Status](https://travis-ci.org/SimpliField/ansible-mongo.svg?branch=master)](https://travis-ci.org/SimpliField/ansible-mongo) [![Ansible Role](https://img.shields.io/ansible/role/9884.svg?maxAge=2592000)](https://galaxy.ansible.com/SimpliField/mongo/)
=========

Setup mongodb server

Requirements
------------

Need ansible 2+

Role Variables
--------------

```yaml
mongodb_db_path: "/data/db"
mongodb_user: "mongodb"
mongodb_group: "mongodb"
# Support version 2.6, 3.0 and 3.2
mongodb_version: 2.6
mongo_replication_set: "myRs"
# Bind mongo on differents ips
mongo_interfaces: ["127.0.0.1", "10.0.0.1"]
```

If you want a single instance, to disable replica_set you can do :
```yaml
mongo_replication_set: !!null
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
