# Ansible Role: Docker Installation (on Ubuntu)

This role can be used to install the Docker Engine on an Ubuntu system.


## Requirements

None


## Role Variables

The following variable is in defaults/main.yml:

- pre_installation_cleanup: false

Set this to true if you have any of the following packages installed on your
system:

- docker
- docker-engine
- docker.io
- containerd
- runc

If pre_installation_cleanup is set to true it will remove the mentioned
packages before the rest of the tasks are run. This is done to remove old or
incompatible versions of these packages.


## Dependencies

None


## Example Playbook

    - hosts: servers
      roles:
         - role: schuam.docker_installation

## License

MIT


## Author Information

This role was created in 2022 by [Andreas Schuster](https://www.schuam.de/).

