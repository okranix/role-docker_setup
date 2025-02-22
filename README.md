docker_setup
=========

Sets up docker with my desired user and directory structure.

Requirements
------------

None

Role Variables
--------------

| Name                         | Comment                                                   | Default value  |
|------------------------------|-----------------------------------------------------------|----------------|
| docker_setup_username        | Username of the docker_setup user                         | `ansible`      |
| docker_setup_comment         | Comment for the docker_setup user                         | `Ansible User` |
| docker_setup_groupname       | Name of the docker_setup user group                       | `ansible`      |
| docker_setup_ssh_keys_present| A list of SSH keys to be present for the docker_setup user| `[]`           |
| docker_setup_ssh_keys_absent | A list of SSH keys to be absent for the docker_setup user | `[]`           |

Dependencies
------------

None

Example Playbook
----------------

    - name: Docker setup
      hosts: docker_hosts
      roles:
        - role: role-docker_setup

License
-------

BSD
