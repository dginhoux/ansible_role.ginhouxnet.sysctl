ginhouxnet.sysctl
=========

This ansible role configure sysctl


Requirements
------------

This ansible role will only run on identified OS defined on meta/main.yml


Role Variables
--------------

It's just a simple list like : 

```
sysctl_settings:
  - name: vm.swappiness
    value: 60
    state: present
```


Dependencies
------------




Example Playbook
----------------



License
-------

BSD


Author Information
------------------

Dany GINHOUX
