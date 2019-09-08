Docker setup
=========

Install docker and docker compose on your system.

Requirements
------------

This role doesn't require any pre-requisites.

Role Variables
--------------

vars/main.yml

**remove_old_installation** 

This variables if set to "yes" will attempt to remove any previously installed docker version.
If you don't need this set the value to "no"

**docker_compose_version**

Set this variable to the exact version of docker compose you want.

Dependencies
------------

This role has no dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: bigpaulie.docker-setup }

License
-------

MIT
