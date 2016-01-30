# Debug-variable

[![Ansible Galaxy](http://img.shields.io/badge/galaxy-GROG.debug--variable-660198.svg?style=flat)](https://galaxy.ansible.com/GROG/debug-variable)
[![Build Status](https://travis-ci.org/GROG/ansible-role-debug-variable.svg?branch=master)](https://travis-ci.org/GROG/ansible-role-debug-variable)

A role for debugging ansible variables.

Inspired by [Lester Wade](https://coderwall.com/p/13lh6w).

This role dumps all ansible variables to a file for debugging. It is strongly
recommended to only use this role on development systems! Using it in a
production environment could result in serious security risks.

## Requirements

- Hosts should be bootstrapped for ansible usage (have python,...)

## Role Variables

| Variable | Description | Default value |
|----------|-------------|---------------|
| `debug_variable_dump_location` | Location for the dump file | '/tmp/ansible.dump' |


## Dependencies

None.

## Example Playbook

```yaml
---
- hosts: servers
  roles:
  - { role: GROG.debug-variable }
```

## Contributing

All assistance, changes or ideas [welcome](https://github.com/GROG/ansible-role-debug-variable/issues)!

## Author

By [G. Roggemans](https://github.com/groggemans)

## License
MIT
