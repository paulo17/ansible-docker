paulboiseau.docker
=========

Install docker-ce and docker-compose on ubuntu

Requirements
------------

None.

Role Variables
--------------

| Name                          | Default  | Type  | Description                            |
| ----------------------------- | -------- | ----- | -------------------------------------- |
| `local_user`                  | $(whoami) | string | Local device user               |


Dependencies
------------

None.

Example
----------------

Put this in `inventory/hosts` if you want to run ansible on your local machine

`default ansible_host=127.0.0.1 ansible_connection=local`

and create this playbook

    - hosts: default
      gather_facts: yes
      roles:
         - { role: paulboiseau.docker }

License
-------

MIT

Author Information
------------------

Paul Boiseau (https://paulboiseau.com)
