# ansible-role-testRole

[![Build Status](https://travis-ci.org/chrnie/ansible-role-testRole.svg?branch=master)](https://travis-ci.org/chrnie/ansible-role-testRole)

Some tests with variables and generic ini files

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yml
# Override default for base.ini
baseIni:
  sectionC:
    key1: default1
    key2: default2
    key3: default3
```

```yml
# Override pgsql credentials
pgsql_db_rdbs: pgsql
pgsql_db_host: "127.0.0.1"
pgsql_db_port: "5432"
pgsql_db_name: "importantDB"
pgsql_db_user: user42
pgsql_db_password: securepasswd
```

```yml
# Override mysql credentials
mysql_db_rdbs: mysql
mysql_db_host: localhost
mysql_db_port: ""
mysql_db_dbname: "another_db"
mysql_db_user: user43
mysql_db_password: SecurePassword
```

## Dependencies


## Example Playbook
You can find an example playbook for testing purposes on https://github.com/chrnie/ansible-role-testRole

```yml
- hosts: all
  vars:
    baseIni:
      sectionC:
        key1: override1
        key2: override2
  roles:
     - { role: chrnie.testRole }
```

## License

Apache License 2.0

## Author Information

Created in 2017 by Christoph Niemann, https://github.com/chrnie/ansible-role-testRole
