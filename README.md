syslog
======
[![Ansible Lint](https://github.com/oxivanisher/role-syslog/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/oxivanisher/role-syslog/actions/workflows/ansible-lint.yml)

Configure rsyslog to send all messages to a server.

Role Variables
--------------

| Name          | Comment                              | Default value |
|---------------|--------------------------------------|---------------|
| syslog_server_address | The syslog server address  |           |
| syslog_server_port | The syslog server port  | `514`          |

Example Playbook
----------------
```yaml
- name: Configure syslog
  hosts: all
  collections:
    - oxivanisher.linux_base
  roles:
    - role: oxivanisher.linux_base.syslog
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_base](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_base/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_base).
