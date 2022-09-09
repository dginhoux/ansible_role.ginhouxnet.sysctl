ginhouxnet.sysctl
=========

This ansible role configure sysctl


Requirements
------------

This role is built to only run on platforms defined in `meta/main.yml`


Role Variables
--------------


```
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
