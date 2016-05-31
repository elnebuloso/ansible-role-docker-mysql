# Ansible Role - MySQL Server for Docker

[![Build Status](https://travis-ci.org/elnebuloso/ansible-role-docker-mysql.svg?branch=master)](https://travis-ci.org/elnebuloso/ansible-role-docker-mysql)

## Requirements

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
docker_mysql_state: "started"
docker_mysql_version: "5.7"
docker_mysql_container_name: "mysql"
docker_mysql_container_volume_base: "/opt/docker"
docker_mysql_config_template: "config.tpl"
docker_mysql_port: "3306"
docker_mysql_root_password: "welcome"
```

## Example Playbook

```
- hosts: localhost
  roles:
    - { role: elnebuloso.docker-mysql }
```

## Dependencies

- `docker` should be installed and working (you can use the `elnebuloso.docker` role to install).

##  License

MIT

##  Author Information

This role was created in 2016 by [elnebuloso](https://github.com/elnebuloso/)