# Debian 9 Stretch image for Ansible testing

[![Docker Automated build](https://img.shields.io/docker/automated/fdiazgon/debian9-ansible.svg)](https://hub.docker.com/r/fdiazgon/debian9-ansible/)
[![Docker Build Status](https://img.shields.io/docker/build/fdiazgon/debian9-ansible.svg)](https://hub.docker.com/r/fdiazgon/debian9-ansible/)

Apart from the dependencies needed by Ansible, this image includes the following packages:
* `gnupg2` and `dirmngr` to use [apt_key](http://docs.ansible.com/ansible/latest/apt_key_module.html) module.
* `sudo` to run some tasks as root.
* `systemd` to use [systemd](http://docs.ansible.com/ansible/latest/systemd_module.html) module.
* `curl` to make requests and check that the services are running properly.
