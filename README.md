ansible-venv-setup
==================

Role is used to setup ansible environment using venv pip.

Role Variables
--------------

### `ansible_release_version`
- Version of ansible software to install using pip
- **Default value**: '6.5.0'

### `group`
- Chown group for directory /app/venv
- **Default value**: "root"

Example Playbook
----------------

    - hosts: ansible_server
      become: yes
      roles:
        - ansible-venv-setup

`defaults/main.yml`:

    ansible_release_version: '6.5.0'
    group: "root"

License
-------

BSD

Author Information
------------------

airstream
