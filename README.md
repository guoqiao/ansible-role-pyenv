Ansible Role: pyenv
=========

This role can do these on target hosts:

- install and setup pyenv
- install python version if required
- create virtualenv with above python version if required
- install requirements in above virtualenv if required

Requirements
------------

The target hosts need to have `apt` to install deb packages.

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
          virtualenv_name: "py370",
          requirements_path: "files/requirements.txt"

Also refer to `tests/test.yml`

License
-------

MIT

Author Information
------------------

guoqiao, a Python Developer living in New Zealand.
