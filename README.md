Ansible Role: Windows Base VM
=========

An Ansible role to prepare an base Windows VM template.

Requirements
------------

None.

Role Variables
--------------

```yml
enable_icmp: true
enable_rdp: true
```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
- hosts: servers
  roles:
    - role: xbufu.windows_base_vm
```

License
-------

MIT / BSD

Author Information
------------------

Created by xbufu.
