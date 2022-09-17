Ansible Role : dginhoux.sysctl
=========

This ansible role configure sysctl


Requirements
------------

This role require a supported platform defined in `meta/main.yml`.
It will skip node with unsupported platform ; this behaviour can be bypassed by settings this variable `asserts_bypass=True`.


Role Variables
--------------

```yaml
sysctl_settings:
  - name: vm.swappiness
    value: 60
    state: present
```


Dependencies
------------

none


Example Playbook
----------------



License
-------

BSD


Author Information
------------------

https://github.com/dginhoux/
