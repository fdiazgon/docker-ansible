# Docker images for Ansible testing

The images are built and published to [Docker Hub](https://hub.docker.com/u/fdiazgon/) using an automated build mechanism.

## Available images

The following Linux distributions come with Ansible installed.

| Distribution      | Size   | Build     |
| ----------------- | ------ | --------- |
| [Debian 9 Stretch](https://hub.docker.com/r/fdiazgon/debian9-ansible/)  | 212MB  |  [![Docker Build Status](https://img.shields.io/docker/build/fdiazgon/debian9-ansible.svg)](https://hub.docker.com/r/fdiazgon/debian9-ansible/)  |
| [Ubuntu 16.04 Xenial Xerus](https://hub.docker.com/r/fdiazgon/ubuntu16-xenial/)  |  270MB  |  [![Docker Build Status](https://img.shields.io/docker/build/fdiazgon/ubuntu16-xenial.svg)](https://hub.docker.com/r/fdiazgon/ubuntu16-xenial/)  |

Most of the images also contains extra packages to be able to use some Ansible modules.

* `curl` to make requests and check that the services are running properly.
* `gnupg2` and `dirmngr` to use [apt_key](http://docs.ansible.com/ansible/latest/apt_key_module.html) module.
* `sudo` to run some tasks as root.
* `systemd` to use [systemd](http://docs.ansible.com/ansible/latest/systemd_module.html) module.

## License

This project is licensed under the MIT License.
