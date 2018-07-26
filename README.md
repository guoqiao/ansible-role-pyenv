Ansible Role: pyenv
=========

This role will setup pyenv on a server, install required python version,
create virtualenv, and install requirements.

Requirements
------------

None

Role Variables
--------------

Refer to `defaults/main.yml`

Dependencies
------------

None

Example Playbook
----------------

    - name: setup pyenv and install python env
      hosts: ubuntu
      roles:
        - role: pyenv
          shell_rc: "~/.zshrc",
          python_version: "3.7.0",
          virutalenv_name: "py370",
          requirements_path: "files/requirements.txt"

Also refer to `tests/test.yml`

License
-------

MIT

Author Information
------------------

guoqiao, a Python Developer living in New Zealand.
