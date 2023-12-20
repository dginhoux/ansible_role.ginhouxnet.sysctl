# ROLE dginhoux.sysctl



## DESCRIPTION

This ansible role configure sysctl.



## REQUIREMENTS

#### SUPPORTED PLATFORMS

| Platform | Versions |
|----------|----------|
| Debian | all |
| EL | all |
| Fedora | all |
| Ubuntu | all |

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
- name: Playbook
  hosts: all
  tasks:
    - name: Start role dginhoux.sysctl
      ansible.builtin.include_role:
        name: dginhoux.sysctl
```


## VARIABLES

#### DEFAULT VARIABLES

Defaults variables defined in `defaults/main.yml`


#### EXAMPLES VARIABLES

```yaml
sysctl_list:
  - name: vm.swappiness
    value: 60
    state: present

sysctl_list_host: []
sysctl_list_group: []
```

NOTE : Theses 3 lists `sysctl_list`, `sysctl_list_group` and `sysctl_list_host` are merged. <br />
You can use the `_host` and `_group` lists to specify per host and/or per group content.


#### DEFAULT OS SPECIFIC VARIABLES

Those variables files are located in `vars/*.yml` are used to handle OS differences.<br />
One of theses is loaded dynamically during role runtime using the `include_vars` module and set OS specifics variable's.

`NOT USED BY THIS ROLE`



## AUTHOR

Dany GINHOUX - https://github.com/dginhoux



## LICENSE

MIT
