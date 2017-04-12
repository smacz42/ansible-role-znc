# Ansible Role: `znc`

## Description

These tasks install ZNC, the bouncer.

ZNC is useful for keeping my nick while I'm out and about on IRC. There's not a whole lot of customization here, however this does make it trivially easy to add channels and networks to the default install, as well as get everything up and running.

## Requirements

* RHEL only

## Role Variables

```yaml
variable: value # comment
```

## Tags

### Role-Specific tags:

* `znc`
* `znc_install`
* `znc_config`

### Global tags:

* `install`
* `config`

## Dependencies

* `smacz42.common`
* `smacz42.iptables`

## Example Playbook

```yaml
- name: Roles in Common
  hosts: all
  gather_facts: true
  remote_user: root
  #no_log: true

  roles:
    - { role: common }
    - { role: iptables }
    - { role: znc }
```

## License

MIT / BSD

## Author Information

This role was created in 2017 by [Andrew Cz](https://andrewcz.com), a student at The Ohio State University.
