docker_setup
=========

Sets up docker with my desired user and directory structure.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

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

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

    - name: Docker setup
      hosts: docker_hosts
      roles:
        - role: role-docker_setup

License
-------

BSD
