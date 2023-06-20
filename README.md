# ROLE dginhoux.sysctl



## DESCRIPTION

This ansible role configure sysctl.



## REQUIREMENTS

#### SUPPORTED PLATFORMS

This role is tested on the following platforms.<br />

| Platform | Versions |
|----------|----------|
| Debian | buster, bullseye, bookworm |
| Fedora | 33, 34, 35, 36, 37, 38 |
| EL | 7, 8 |

You can set this variable `check_compatibility` to let the role skip nodes with unsupporteds platforms to avoid any compatibility problems.<br />


#### ANSIBLE VERSION

Ansible >= 2.13

#### DEPENDENCIES

None.



## INSTALLATION

#### ANSIBLE GALAXY

```shell
ansible-galaxy install dginhoux.sysctl
```
#### GIT

```shell
git clone https://github.com/dginhoux/ansible_role.sysctl dginhoux.sysctl
```


## USAGE

#### EXAMPLE PLAYBOOK

```yaml
- hosts: all
  roles:
    - name: start role dginhoux.sysctl
      ansible.builtin.include_role:
        name: dginhoux.sysctl
```


## VARIABLES

#### DEFAULT VARIABLES

Defaults variables defined in `defaults/main.yml` : 

```yaml
sysctl_settings:
  - name: vm.swappiness
    value: 60
    state: present
```

#### DEFAULT OS SPECIFIC VARIABLES

Those variables files are located in `vars/*.yml` are used to handle OS differences.<br />
One of theses is loaded dynamically during role runtime using the `include_vars` module and set OS specifics variable's.

`NOT USED BY THIS ROLE`



## AUTHOR

Dany GINHOUX - https://github.com/dginhoux



## LICENSE

MIT
