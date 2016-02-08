# Debug-variable

[![Ansible Galaxy][galaxy_image]][galaxy_link]
[![Build Status][travis_image]][travis_link]
[![Latest tag][tag_image]][tag_url]
[![Gitter chat][gitter_image]][gitter_url]

A role for debugging ansible variables.

Inspired by [Lester Wade][lester_wade].

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
All assistance, changes or ideas [welcome][issues]!

## Author
By [G. Roggemans][groggemans]

## License
MIT

[galaxy_image]:         https://img.shields.io/badge/galaxy-GROG.debug--variable-660198.svg?style=flat
[galaxy_link]:          https://galaxy.ansible.com/GROG/debug-variable
[travis_image]:         https://travis-ci.org/GROG/ansible-role-debug-variable.svg?branch=master
[travis_link]:          https://travis-ci.org/GROG/ansible-role-debug-variable
[tag_image]:            https://img.shields.io/github/tag/GROG/ansible-role-debug-variable.svg
[tag_url]:              https://github.com/GROG/ansible-role-debug-variable/tags
[gitter_image]:         https://badges.gitter.im/GROG/chat.svg
[gitter_url]:           https://gitter.im/GROG/chat

[lester_wade]:          https://coderwall.com/p/13lh6w

[issues]:               https://github.com/GROG/ansible-role-debug-variable/issues
[groggemans]:           https://github.com/groggemans
