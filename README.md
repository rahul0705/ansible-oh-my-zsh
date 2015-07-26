[![Build Status](https://travis-ci.org/rahul0705/ansible-oh-my-zsh.svg?branch=master)](https://travis-ci.org/rahul0705/ansible-oh-my-zsh)

Ansible Oh-My-Zsh
=========

Ansible role to install and configure Oh-My-Zsh

Requirements
------------

Debian based system

Role Variables
--------------

```yaml
oh_my_zsh_user: rahul
oh_my_zsh_user_home: ~{{ oh_my_zsh_user_home }}
```

Dependencies
------------

None

Example Playbook
----------------

1) Install Oh My ZSH with default settings

```yaml
- hosts: all
  roles:
    - role: oh_my_zsh
```

2) Install Oh My ZSH with custom settings

```yaml
- hosts: all
  roles:
    - role: oh_my_zsh
      oh_my_zsh_user: rahul
      oh_my_zsh_home: /opt/rahul
```

License
-------

MIT
