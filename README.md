pbos.neutron
=============

Ansible role to install and setup Neutron for OpenStack 

Requirements
------------

This role requires Ansible 2.11 or higher.

This role supports:

  - Debian 11 (bullseye)

Role Variables
--------------

[defaults/main.yml](defaults/main.yml)

Dependencies
------------

[ansible-galaxy-requirements.yml](ansible-galaxy-requirements.yml)

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    hosts: openstack
    roles:
      - {role: pbos.neutron, tags: neutron}

Neutron is installed on the node in openstack inventory group:

    [controller]
    host-1
    host-2
    host-3
    [compute]
    host-4
    host-5
    host-6
    [openstack:children]
    controller
    compute

License
-------

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

  - Heechul Kim @iOrchard
      - <https://github.com/iorchard>

