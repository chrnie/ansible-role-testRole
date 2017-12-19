# ansible-role-testRole

[![Build Status](https://travis-ci.org/chrnie/ansible-role-testRole.svg?branch=master)](https://travis-ci.org/chrnie/ansible-role-testRole)

Some tests with variables and generic ini files

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):


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
