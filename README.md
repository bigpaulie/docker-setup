Docker setup
=========

Install docker and docker compose on your system.

Requirements
------------

This role doesn't require any pre-requisites.

Role Variables
--------------

|variable name| description | default value|
|-------------|-------------|--------------|
|remove_old_installation|This variables if set to "yes" will attempt to remove any previously installed docker version. If you don't need this set the value to "no"|yes|
|docker_compose_version|Set this variable to the exact version of docker compose you want.|1.24.1|

Dependencies
------------

This role has no dependencies.

Example Playbook
----------------

    - hosts: servers
      vars:
        remove_old_installation: yes
        docker_compose_version: "1.24.1"
      roles:
         - { role: bigpaulie.docker_setup }

License
-------

MIT