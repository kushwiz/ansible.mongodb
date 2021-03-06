kushwiz.mongodb
===============

Ansible role for MongoDB installation on a 32bit Debian machine

Requirements
------------

Ansible latest version

Role Variables
--------------

defaults/main.yml
-----------------
```
mongodb_datadir_prefix: /data/db
mongodb_log_path: /var/log/mongodb
mongod_keyfile: BdubBunlybr5JUIFD6tyO3es3hmuYnpurIVGuq1HCn63e9MB6RQL0cWZfNDE

mongodb_user: mongodb
mongodb_group: mongodb

mongodb_version: 3.0.4
mongodb_arch: i686
mongodb_port: 27017
mongodb_install_dir: /opt/mongodb
mongodb_config_path: /etc/mongod.conf
mongodb_directory: mongodb-linux-{{mongodb_arch}}-{{mongodb_version}}
mongodb_download_url: http://fastdl.mongodb.org/linux/{{mongodb_directory}}.tgz

mongodb_admin_user: dbadmin
mongodb_admin_pass: hmuYnpurIVGuq1HCn6
```

Dependencies
------------
None

Example Playbook
----------------

    - hosts: servers
      roles:
         - kushwiz.mongodb

License
-------

MIT

Author Information
------------------

Kushal Bhandari
