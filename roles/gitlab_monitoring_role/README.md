Sentry monitoring role
=========

This role installs monitoring agent and enable the status information handlers in Nginx and redis. The role also adds the keys of the required IAM user.



Role Variables
--------------

| Variable                      | Description                                          |
|-------------------------------|------------------------------------------------------|
| `ansible_user`                | Your Ansible user name.                              |
| `ansible_ssh_private_key_file`| Path to ssh private key.                             |

Example Playbook
----------------

    - hosts: gitlab
      become: true
      gather_facts: no
      roles:
         - { role: gitlab_monitoring_role }

License
-------

GNU General Public License v3.0

Author Information
------------------

https://www.sxvova.opensource-ukraine.org/ and Nikita Makarov
