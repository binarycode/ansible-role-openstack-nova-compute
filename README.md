Ansible Role: OpenStack Nova Compute Node
=========================================

This role installs and configures OpenStack Nova Compute Node on EL7 system.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`)

    ip_address:

IP address in management network.

    controller_ip_address:

Controller Node IP address in management network.

    keystone_host: controller
    keystone_password:

Keystone credentials for Nova user.

    rabbitmq_host: controller
    rabbitmq_user:
    rabbitmq_password:

RabbitMQ credentials.

    glance_host: controller

Glance API host.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
        - binarycode.openstack-nova-compute

License
-------

BSD

Author Information
------------------

[Igor Sidorov](https://github.com/binarycode)
