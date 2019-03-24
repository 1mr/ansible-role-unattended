Unattended
==========

This role helps to install and configure unattended upgrade.

Requirements
------------

This role requires ansible 1.4 or higher.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows:

    unattended:
      blacklist:
        - mongodb
        - mongodb-10gen
        - mongodb-clients
        - mongodb-server
        - mysql-client
        - mysql-server
        - php5
        - php7.0
        - php-pear
        - supervisor

Variable 'unattended.blacklist' is default.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: unattended, tags: unattended }

License
-------

BSD

Author Information
------------------

Created by Viacheslav Kuzmenko
