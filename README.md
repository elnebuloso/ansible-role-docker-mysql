# Ansible Role - Docker for Linux Server

[![Build Status](https://travis-ci.org/elnebuloso/ansible-role-docker-mysql.svg?branch=master)](https://travis-ci.org/elnebuloso/ansible-role-docker-mysql)

MySQL Server for Docker.

## Requirements

  - `docker` should be installed and working (you can use the `elnebuloso.docker` role to install).

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
docker_mysql_name: "mysql"
docker_mysql_state: "started"
docker_mysql_version: "5.7"
docker_mysql_root_password: "welcome"
docker_mysql_port: "3306"
```

## Example Playbook

```
- hosts: localhost
  roles:
    - { role: elnebuloso.docker-mysql }
```

##  License

MIT

##  Author Information

This role was created in 2016 by [elnebuloso](https://github.com/elnebuloso/)