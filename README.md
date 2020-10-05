# vdzhorov.gerrit

[![Ansible Role](https://galaxy.ansible.com/vdzhorov/gerrit)
[![Build Status](https://travis-ci.org/vdzhorov/ansible-role-gerrit.svg?branch=main)](https://travis-ci.org/github/vdzhorov/ansible-role-gerrit)

Ansible role for basic Gerrit installation on RHEL 7/8 systems.

## Author Information

Valentin Dzhorov

## Company

Delta.BG

## Requirements

Ansible 2.6

## Role Variables

|Variable|Description|Default|
|---|---|:--|
|```gerrit_version```|Gerrit Version|3.2.3|
|```gerrit_user```||gerrit|
|```gerrit_group```||gerrit|
|```gerrit_home_dir```|Directory where Gerrit will be installed|```/opt/gerrit-{{ gerrit_version }}```|
|```gerrit_config```|```gerrit_config``` Object||
|```gerrit_database_type```||MYSQL|
|```gerrit_database_mysql```|```gerrit_database_mysql``` Object||
|```gerrit_index_type```||LUCENE|
|```gerrit_auth_type```||HTTP|
|```gerrit_container```|```gerrit_container``` Object||
|```gerrit_sshd```|```gerrit_sshd``` Object||
|```gerrit_httpd```|```gerrit_httpd``` Object||
|```gerrit_cache```|```gerrit_cache``` Object||
|```gerrit_receive```|```gerrit_receive``` Object||

## Objects

TODO

## Dependencies

- bertvv.mariadb
- robertdebock.java
- geerlingguy.git

## Example Playbook

    - hosts: servers
      roles:
         - role: vdzhorov.gerrit

## License

GNU General Public License v3.0
