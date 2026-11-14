Ansible Role: Windows Base VM
=========

An Ansible role to prepare a base Windows VM template: Explorer, console and power
settings, local admin passwords that never expire, ping and RDP, no automatic Windows
Update, Sysinternals in `C:\Tools\Sysinternals` and Chocolatey packages.

Requirements
------------

Collections `ansible.windows`, `community.windows` and `chocolatey.chocolatey`.

Role Variables
--------------

```yml
windows_base_vm_enable_icmp: true
windows_base_vm_enable_rdp: true
windows_base_vm_disable_auto_updates: true
windows_base_vm_sysinternals: true
windows_base_vm_sysinternals_path: C:\Tools\Sysinternals
windows_base_vm_choco_packages:   # empty list skips Chocolatey
  - 7zip
  - notepadplusplus
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
